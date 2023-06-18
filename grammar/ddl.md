creating a table
symbols: #t t#

#t name | fields | constraints  #t

field description

name : data type

name cannot contain following symbols : $#*!-=>

full syntax

constraint syntax
columnname:constraint_type:referenced_column if any

#t tablename | fieldname:datatype, fieldname:datatype: t#

alternate

#table tablename | fieldname:datatype, fieldname:datatype table#

alternate

#table tablename, fieldname:datatype, fieldname:datatype t#

------
alter table
*t t*
*table table*

drop column name 
*table -personalid table* @students;

rename column name newname 
rename personalid to pid
*table personalid->pid *table @students;

more changes with one command
*t personalid->pid, -birth_year t* @students;

add column
+age:int

more changes with one command
*t personalid->pid, -birth_year,+age:int t* @students;

drop constraint
-c .columnname constrainttype

add constraint
+c .columnname constrainttype

example
//add pid as primary key column for a table
*t +c pid p *t @students

-----
remove table

!tt! @tablename
!table!  @tablename
------
add namespace
------
rename namespace
*n oldname -> newname n* @database;
------
remove namespace
!n namespace n! @database;
------
add database
------
change database
------
remove database