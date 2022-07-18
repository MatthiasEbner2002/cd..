# cd..
Meme like sl for cd ..

default image: 
![image](https://user-images.githubusercontent.com/77750231/179476075-2a9b5948-98d0-45f0-b1b1-4051943232bd.png)


# Tech
- bashscript
# Installation
 after Project is cloned.
change forlder:
```
cd cd..
```
start installation script:
```
./icd..
```
`icd..` does :
- creat new folder in the same folder as the git repo called .cd..
- file cd.. is moved to the new folder
- a softlink is made to the bin folder
- the repo gets delted (including the icd file)
> Note 1: `./icd..` will use rm -rf on the git folder.
> Note  2: folder `.cd..` is not visible under normal circumstances (in terminal use `ls -l` or `ll` to see folder).

installation is finished and 
```
cd..
```
can be used.

# Options

-e, --exitenabled               ctrg+c can be used <br/>
-m, --message <message>         write message bevor File <br/>
-t, --times <int>               amount of lines getting deleted <br/>
-f, --file filename             content of file is getting used <br/>


  
# Usage
$0 [-e] [-m <message>] [-t <+int>] [-f <filename>]
