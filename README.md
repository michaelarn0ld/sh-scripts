# POSIX Shell Scripts
----
The scripts in this repository are POSIX compliant for maximum portability. They
should be "plug and play" but you should stil audit the code for your own
understanding.

If you intend to use any of these scripts, it is important to ensure that they
are accessible by your ```$PATH```.

Make sure you ```shellcheck``` all scripts before using them.


# Table of Contents
----
1. [cmt](#cmt)
1. [chmox](#chmox)
1. [makemvn](#makemvn)
1. [path](#path)
1. [ucmt](#ucmt)

|   Scripts   |   Summary
|   :-:       |   -
|   cmt       |   Makes lines or code blocks into commments in vi
|   chmox     |   Adds execution permissions to files
|   makemaven |   Creates a barebone directory structure for maven projects
|   path      |   Prints an easy-to-read version of ```$PATH```
|   ucmt      |   Removes comments from code blocks in vi


## cmt
----
Cmt is a script that allows you to turn lines/blocks of code into comments while
in the vi editor. Since some languages use ```#``` for comments and others use
```//```, you will need to specify the ```-ht``` option if you want to use the
latter; ```// is the default

### USAGE
```sh
$ cmt [-fs] < FILE
```
<br><br>

## chmox
----
Chmox is a script that adds execution privileges to an arbitrary number of files;
it is intended to replace ```chmod +x [FILES...]```

### USAGE
```sh
$ chmox [FILES...]
```
<br><br>

## makemvn
----
Makemvn is a command line tool for you to easily setup a barebones maven
project. Remember the java convention for naming packages:
***Organization -> Project -> Category***

### USAGE
```sh
$ makemvn [ORG.PROJECT.CATEGORY] [GROUP_ID] [ARTIFACT_ID]
```
<br><br>

## path
----
Path is a simple one-liner script for displaying your ```$PATH``` environment
variable in a way that is easier to read.

### USAGE
```sh
$ path
---------------------
/part/of/your/path
/another/part/of/path
/whatever/you/want
---------------------
```
<br><br>

## ucmt
----
Ucmt is a script that allows you to remove comment indicators from lines or 
blocks of code while in the vi editor.

### USAGE
```sh
$ ucmt < FILE
```
<br><br>

# Contributors
----
@author: Michael Arnold \
@contact: me@michaelarnold.io


# License
----
Copyright © 2021 Michael Arnold

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

