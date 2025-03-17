1) pwd(print working directory) => Machine me users me jaake bata dega unke naam , jaise isme sirf nikhil hai to it will show users/nikhil/

Terminal is nothing but another interface to do things on your machine

2) cd(change directory) => cd Desktop/ Terminal would like to access files in desktop folder and we get now desktop in terminal and now if we type pwd , we get /users/nikhil/Desktop 
cd let's you navigate your file system


if we type cd.. we get one folder back 
cd../.. will take me 2 folders back
3) ls(listing files in your current folder) => ls daabate hi desktop ke andar ki files dikha dega

4) mkdir(make directory) => a new folder can be created by it
to create directories recuresively mkdir -p frontend/scripts
mkdir -p frontend/img
...


5) touch => Let's you create an empty file , if I write in desktop to be touch index.js , then a file named index.js will be formed

6) cat => It prints the content of a file by wrting cat index.txt
we can add content also in to an exmpty file by cat > newfile.txt 
And now add the content
add content to an already existing file is by cat >> newfile.txt
dsndns


7) vi(vim) => Lst's you edit files , Not recommended for begineers
if we write vi a.txt , then that file will get opened and we will edit that by pressing I button
press escape to escape insert mode and then write :wq! to leave the file and save too the written content


8) mv(let's you move file ) => mv a2.txt new-folder/(second folder name is that where we want to shift the file)
mv test test2/new-folder
also let's you rename your file mv script.js runtime_script.js


9) cp(copy files) => cp a3.js test2 [ it will copy the a3.js file into test2 folder]
if we have to copy folders then write cp -r test3 test2
cp -r circuits/test contracts

10) clear => to clear your terminal 

11) chmod(change the file permissions) => 
chmod ugo+(adding permissions)
chmod ugo-(subtracting permissions) r-read,w-write,x-execute
if it's a folder chmod -R ugo-rwx

chmod u+x newscript.sh  ( So , now execute permissions are added to it)

____   head newfile.txt will give the first ten rows of the file
       tail newfile.txt will give the last ten rows of the file

we can use &&(and operator to combine a bunch of commands)
|(pipe charcter)  command 1 | command 2 [Whatever the output from command 1 will flow into command 2]


if we write grep "one" newfile.txt => we will get ki konn konsi line me one aa raha hai
grep -c "one" newfile.txt => isme numeric me aajeyga ki 3 baar one aaya tha
grep -hinw "one" a.txt [Here we are only looking for the word one not be a subpart of any word]

ls -lt newdir [ saari files ki details aajayengi ki kitne bytes ki hai , last modified date and their names]
ls -l newdir => gives the files
ls -la newdir/snake_game => gives the hidden files too

ls -lR | grep.json(saari jSon files aajayengi)
ls *.js(will give .js files)


nvm(node version manager)
npm(node package manager)
