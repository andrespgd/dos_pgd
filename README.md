
Format command by adding the /P parameter. This new parameter allows you to overwrite every sector on a disk with 0's during the format procedure:
```
Format volume /P:passes
```
The /P parameter allows you to specify the number of passes or # overwrites every sector with 0's.
```
Format D: /P:4
```




Compare 2 files:
```
FC file1 file2
```
Compare 2 binary files:
```
FC /B file1 file2
```
