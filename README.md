# rgb(9, 105, 218) This is to make note of all the linux commands used on daily basis 

## * To locate a file
### 1. Find command can be used with certain custom rules to locate files based on name, size, modify time , permissoins etc . However this command is I/O intensive/ slow 
`find /dir -name *filenam*`

### 2. Locate is faster as it looks for filename in the DB. Its important to do updatedb inorder to lookup the file in latest file structure as new files would have been created after the last auto updatedb by system 
locate filename


## * Adding log message to the /var/log/messages file. This would useful while reproducing certain application or product issues 
```
logger "Start of the issue" 

tail /var/log/messages 
```
