
# Check Code Duplication
## Unatar and Install txl
Based on your environment, choose the right tar/zip. Double-click the tar/zip file or run the command:  
```sh
tar xvzf txlxxxx.tar.gz
```
Under the TXL distribution directory, run:
```sh
sudo ./InstallTxl
```
## Nicad
Untar Nicad
Under the distribution directory
```sh
make
```
To run it:
```sh
./nicard functions c ${/Path/of/the/test/file} default-report
```


>-   To detect type 1     (exact) clones,                           set threshold=0.0
>-   To detect type 2     (renamed) clones,                         set threshold=0.0 and rename=blind
>-   To detect type 2c    (consistently renamed) clones,            set threshold=0.0 and rename=consistent
>-   To detect type 3-1   (near-miss exact) clones,                 set threshold=0.3
>-   To detect type 3-2   (near-miss renamed) clones,               set threshold=0.3 and rename=blind
>-   To detect type 3-2c  (near-miss consistently renamed) clones,  set threshold=0.3 and rename=consistent  
Example:
```sh
./nicard functions c ${/Path/of/the/test/file} default-report type1
```  


More informations in [Nicad](https://www.txl.ca/txl-nicaddownload.html)
