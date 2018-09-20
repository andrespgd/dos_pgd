
When Microsoft launched Windows Vista in 2007 with all of its newfangled user interface features, it enhanced the Format command by adding the /P parameter. This new parameter allows you to overwrite every sector on a disk with 0's during the format procedure. The actual syntax of the parameter is
```
Format volume /P:passes
```
The /P parameter allows you to specify the number of passes, or in other words, the number of times that you want to overwrite every sector with 0's. By doing so, you decrease the likelihood that anyone would be able to retrieve any sensitive data. Even if you don't specifically use the /P parameter, the Format command will by default make one pass of the overwrite operation, unless you use the /Q parameter to perform a quick format.

Example:
```
Format D: /P:4
```
