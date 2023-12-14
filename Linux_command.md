## Linux Commands

**1. How to make a directory**

**mkdir**:This command is used to create a new directory.
```
mkdir sample
```
Mkdir:it is used for creating new directory

Sample: it is the name of the newly created directory.

Output:

brijesh@brijesh-Aspire-Lite-AL15-51:~$ mkdir sample

brijesh@brijesh-Aspire-Lite-AL15-51:~$ ls

Desktop    Downloads   new.java           Pictures  sample.txt  test

docsify    index.html  package.json       Public    snap        Videos

Documents  Music       package-lock.json  **sample**    Templates

![image](https://github.com/b02k11/Linux-Commands/assets/132880648/a836aad3-2230-45f8-82a9-65b0e410763e)  

ls command is used to display all the directory and files.

**2. Remove a directory**

**rmdir**: This command is used to remove the empty directory.
```
rmdir sample
```
rmdir: it is used for removing the empty directory.

sample: it is the name of the empty directory.

brijesh@brijesh-Aspire-Lite-AL15-51:~$ rmdir sample

brijesh@brijesh-Aspire-Lite-AL15-51:~$ ls

Desktop    Downloads   new.java           Pictures    snap       Videos

docsify    index.html  package.json       Public      Templates

Documents  Music       package-lock.json  sample.txt  test

![image](https://github.com/b02k11/Linux-Commands/assets/132880648/cab1c96c-ffd6-4521-9a63-20b8a9569779)


**3. Make a copy of a file**

**cp**: This command is used to copy a file to a new location.
```
cp sample.txt Downloads
```
cp: it copies the file to a new location

sample.txt: This is the name of the file to be copied

Downloads : This is the location of the directory where the file will be copied.

brijesh@brijesh-Aspire-Lite-AL15-51:~$ cp sample.txt Documents

brijesh@brijesh-Aspire-Lite-AL15-51:~$ cd Documents 

brijesh@brijesh-Aspire-Lite-AL15-51:~/Documents$ ls

document.md  **sample.txt**

brijesh@brijesh-Aspire-Lite-AL15-51:~/Documents$ 

![image](https://github.com/b02k11/Linux-Commands/assets/132880648/60f98163-7e19-4f82-bbc1-a5ca5c97fb7a)

**4. Move or rename a file**

**mv**: this command is used to move a file from one location to another but it can also be used to rename the file.
```
mv sample.txt /home/brijesh/test/newname.txt
```
mv : it moves the file from one location to another

sample.txt: This is the name of the file which will be moved.

/home/brijesh/test/ : this is the location where file will be moved

newname.txt: This is the new name of the file.


brijesh@brijesh-Aspire-Lite-AL15-51:~$ mv sample.txt /home/brijesh/test/newname.txt

brijesh@brijesh-Aspire-Lite-AL15-51:~$ cd test

brijesh@brijesh-Aspire-Lite-AL15-51:~/test$ ls

newdira  newdire  newdiri  newdirm  newdirq  newdiru  newdiry

newdirb  newdirf  newdirj  newdirn  newdirr  newdirv  newdirz

newdirc  newdirg  newdirk  newdiro  newdirs  newdirw  **newname.txt**

newdird  newdirh  newdirl  newdirp  newdirt  newdirx

![image](https://github.com/b02k11/Linux-Commands/assets/132880648/1cad2b5c-0b12-436d-8c5d-236117b926a7)

**5.Create an empty file**

touch : This command is used to create an empty file.
```
touch textfile.txt
```
touch: This command is used to create an empty file.

textfile.txt : This is the name of the new file.

brijesh@brijesh-Aspire-Lite-AL15-51:~/Documents$ touch textfile.txt

brijesh@brijesh-Aspire-Lite-AL15-51:~/Documents$ ls

document.md  newfile.txt  **textfile.txt**

![image](https://github.com/b02k11/Linux-Commands/assets/132880648/2a52eb14-5d82-40cf-9b5e-6ae4687b4a1c)

**6.Remove multiple files with a single command**

rm filename{1..5}: This command is used to remove multiple files simultaneously.
```
rm new{1..5}.txt
```
rm : This command is used to delete file

new{1..5}: This will remove 5 files named as new1.txt,  new2.txt, new3.txt, new4.txt ,new5.txt

brijesh@brijesh-Aspire-Lite-AL15-51:~/test$ ls

new1.txt  new2.txt  new3.txt  new4.txt  new5.txt

brijesh@brijesh-Aspire-Lite-AL15-51:~/test$ rm new{1..5}.txt

brijesh@brijesh-Aspire-Lite-AL15-51:~/test$ ls

brijesh@brijesh-Aspire-Lite-AL15-51:~/test$

![image](https://github.com/b02k11/Linux-Commands/assets/132880648/297aaa98-9632-4e1f-9470-cc0ad3e20125)

**7.Remove content from the folder without removing folder**

rm -r /path/to/file/\* : This command is used to remove all the contents inside a directory without deleting the directory.
```
rm -r /home/brijesh/test/*
```
rm -r : This command is used to delete all the files of a directory recursively.

/home/brijesh/test/\*: This command specifies the path of the directory whose content is to be removed. \* indicate that all the contents are to be removed.

brijesh@brijesh-Aspire-Lite-AL15-51:~$ rm -r /home/brijesh/test/\*

brijesh@brijesh-Aspire-Lite-AL15-51:~$ cd test

brijesh@brijesh-Aspire-Lite-AL15-51:~/test$ ls

brijesh@brijesh-Aspire-Lite-AL15-51:~/test$

![image](https://github.com/b02k11/Linux-Commands/assets/132880648/d50581de-fe1f-469d-be8d-d5713cc5580d)
  
**8.Create multiple folder(a-z) with a single command**

mkdir newdir{a..z} : This command is used to create multiple directories simultaneously.
```
mkdir newdir{a..z}
```
mkdir : This command is used to make a new directory.

newdir{a..z}: This command will give the name newdira, newdirb, newdirc, …....newdiry, newdirz.

brijesh@brijesh-Aspire-Lite-AL15-51:~/test$ mkdir newdir{a..z}

brijesh@brijesh-Aspire-Lite-AL15-51:~/test$ ls

newdira  newdird  newdirg  newdirj  newdirm  newdirp  newdirs  newdirv  newdiry

newdirb  newdire  newdirh  newdirk  newdirn  newdirq  newdirt  newdirw  newdirz

newdirc  newdirf  newdiri  newdirl  newdiro  newdirr  newdiru  newdirx

![image](https://github.com/b02k11/Linux-Commands/assets/132880648/39cbeac3-cab7-43c1-8d96-3b9716df6bcd)
