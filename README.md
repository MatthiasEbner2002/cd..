# cd..

Meme like sl for cd ..

default image:

```
──────▄▌▐▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▌
───▄▄██▌█ BEEP BEEP
▄▄▄▌▐██▌█ -5 LINES DELIVERY
███████▌█▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▌
▀(⊙)▀▀▀▀▀▀▀(⊙)(⊙)▀▀▀▀▀▀▀▀▀▀(⊙
```


## Tech

- bashscript

## Installation

after Project is cloned.
change forlder:

```shell
cd cd..
```

start installation script:

```shell
./install
```

`install` does :

- creat new folder in the same folder as the git repo called .cd..
- file **cd..** and **remove** is moved to the new folder
- creat folder **/lib/cd..**
- move **color_print** and **default.txt** to **/lib/cd../**
- a softlink is made to the bin folder
- the repo gets delted (including the **install** file)

> Note 1: `./install` will use rm -rf on the git folder.

> Note  2: folder `.cd..` is not visible under normal circumstances (in terminal use `ls -l` or `ll` to see folder).

installation is finished and can be used.

```shell
cd..
```

## Remove

To delete all files from cd.. go to folder .cd.. and use command

```shell
./remove
```

`remove` does :

- removes softlink /bin/cd..
- removes file **/lib/cd../default.txt**, **/lib/cd../colorful_print** and folder /lib/cd..
- removes .cd..

## Options

| Option      | Description |
| ----------- | ----------- |
|**-e**, **--exitenabled** | ctrg+c can be used |
|**-t**, **--times** \<int> | amount of lines getting deleted |
|**-f**, **--file** filename | content of file is getting used |

<!--|**-m**, **--message** \<message> | write message bevor File |-->
## Usage

<!--/usr/bin/cd.. [-e] [-m \<message>] [-t <+int>] [-f \<filename>] -->
/usr/bin/cd.. [-e] [-t <+int>] [-f \<filename>]
