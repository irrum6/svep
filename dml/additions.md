Adding records
insert is denoted with following symbols: ##

The symbols embed insert parameters within themselves.
So full description of it is the following

# value,value2,value3,,,valuen #
example:
Insertin 4 records in studs table on database sys within namespace other

# 19,1300,gela # @sys::other::studs ;
# 20,1301,vaja # @sys::other::studs ;
# 21,1302,irakli # @sys::other::studs ;
# 22,1303,davit # @sys::other::studs ;


when adding multiple records(rows), you can seperate them with |

The examples above can be written as single query;

@sys::other::studs

# 19,1300,gela |
20,1301,vaja |
21,1302,irakli |
22,1303,davit  # ;
