creating a table
symbols: #t t#

#t name | fields  #t

field description

name : data type:constraint

name cannot contain following symbols : $#*!-=>

full syntax

constraint syntax
columnname:constraint_type:referenced_column if any

#t tablename | fieldname:datatype:constraint, fieldname:datatype:constraint t#

alternate

#table tablename | fieldname:datatype:constraint, fieldname:datatype:constraint table#

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
-----
remove table

!tt! @tablename
!table!  @tablename
------
create namespace
------
rename namespace
------
remove namespace
------
crate database
------
alter database
------
remove database