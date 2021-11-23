# SLDB

SLDB - string lightweight database. 

This db is oriented to work with SLQL: https://github.com/ZikkeyLS/SLQL

## Example:

```
TEST1
user_token(U) | user_name(U, Min(4), Max(16)) | user_password(Min(6), Max(20)))
-------------------------------------------------------------------------------
0             | "Test"                        | "Password"
1             | "Test2"                       | "Password1"
```

## Description:

  We are using first line for writing name of db. 
  
  **----** - horizontal separator.
  
  **|** - vertical separator. We are usually using this separator with " "(space) mark on both sides.
  
  Second line sets default parametres with names and limits.
  
  Third line is horizontal separator line between config and table elements.
  
  Fourth+ line - table elements. First parameter is always number(indicates connectable token). Second+ parameter is a string value.
