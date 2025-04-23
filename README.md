# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1

![image](https://github.com/user-attachments/assets/f6d68994-9f4f-4428-8ab2-b46cbaae3228)

cat > file2

![image](https://github.com/user-attachments/assets/62d33d86-ecdb-4e89-b2e1-4b8ea546d5cd)

### Display the content of the files
cat < file1
## OUTPUT

![image](https://github.com/user-attachments/assets/aec01fe1-70fb-466d-b3f7-1537a61a4919)


cat < file2
## OUTPUT
![image](https://github.com/user-attachments/assets/8e14244a-0058-48e6-873c-0eb8ecb33555)


# Comparing Files
cmp file1 file2
## OUTPUT
 ![image](https://github.com/user-attachments/assets/c00a34ca-1efa-4f0d-9d7f-e9af72f3e63b)

comm file1 file2
 ## OUTPUT

 ![image](https://github.com/user-attachments/assets/67a8986d-3e88-40d0-bd5b-016cfc6eff3e)

diff file1 file2
## OUTPUT

![image](https://github.com/user-attachments/assets/523d1dd8-4068-4ae8-9b53-313e6684afa3)




#Filters

### Create the following files file11, file22 as follows:

cat > file11

![image](https://github.com/user-attachments/assets/521509dd-ddb1-42a4-a037-5a3da719d6c4)

cat > file22

![image](https://github.com/user-attachments/assets/52fac54a-82f7-4f32-af27-6bf09e36e6d7)

cut -c1-3 file11
## OUTPUT

![image](https://github.com/user-attachments/assets/5a439581-6ac9-4cc6-ab41-646ec342023b)



cut -d "|" -f 1 file22
## OUTPUT

![image](https://github.com/user-attachments/assets/57316f49-d38a-41a9-8aaf-e5254df1310b)


cut -d "|" -f 2 file22
## OUTPUT

![image](https://github.com/user-attachments/assets/8cf50b98-6e00-4306-9fec-6456c1df607c)


cat < newfile 

![image](https://github.com/user-attachments/assets/7437cbad-1c65-4381-96f0-9c188368b57a)

cat > newfile 
``
Hello world
hello world
``
grep Hello newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/582ad0ad-b512-46dd-b464-597d49ec8626)


grep hello newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/24365576-c332-43af-bd5d-c783c4df3a23)


grep -v hello newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/79f0381f-0dbd-4cc9-a6f3-e15ed26d2c3d)


cat newfile | grep -i "hello"
## OUTPUT

![image](https://github.com/user-attachments/assets/b87d7bf3-1bcd-4fb5-85c3-60a1e66e9309)

cat newfile | grep -i -c "hello"
## OUTPUT

![image](https://github.com/user-attachments/assets/9d581bbf-d0c1-4ccd-8355-988377ce38cd)

grep -R ubuntu /etc
## OUTPUT

![image](https://github.com/user-attachments/assets/e92e9470-5a0b-40bf-95d4-25ea0d7a21bb)


grep -w -n world newfile   
## OUTPUT

![image](https://github.com/user-attachments/assets/95288062-8164-4ff3-b9cb-7867b4378362)


cat < newfile 

![image](https://github.com/user-attachments/assets/b5dae89b-9567-4797-bbe1-6ea7c6b8bc66)

cat > newfile

![image](https://github.com/user-attachments/assets/a43bb191-eb80-4a05-be38-590c8787c1fb)

egrep -w 'Hello|hello' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/03d5f680-df8e-4525-bef8-ed39593300e9)


egrep -w '(H|h)ello' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/7d9e1598-1261-450e-ae49-efefcac94ab3)


egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/701d86d8-a771-4fc2-b923-15b25e37d44c)


egrep '(^hello)' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/7b340e2a-5ca6-4e60-b999-b304b2b03a01)


egrep '(world$)' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/dae0c3a8-3e61-411a-878e-96a893a937c8)



egrep '(World$)' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/e78642d0-e62f-44e1-8046-38b5b3c2057c)

egrep '((W|w)orld$)' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/1ff2b003-665f-4d60-ba00-8c5af9c1a127)



egrep '[1-9]' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/d56e13f8-4a75-4fe3-bfdd-309d41068e3f)


egrep 'Linux.*world' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/528e181a-f85e-42d6-bdc9-89fb6353b279)

egrep 'Linux.*World' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/17fb5faa-7557-44d1-845a-3e71eaaee369)

egrep l{2} newfile
## OUTPUT

![image](https://github.com/user-attachments/assets/4b9298d4-1aa4-4b02-9219-db9279450036)


egrep 's{1,2}' newfile
## OUTPUT 

![image](https://github.com/user-attachments/assets/40438d04-215e-43d6-b9f2-58031d1d23bd)


cat > file23

![image](https://github.com/user-attachments/assets/64a7d4be-0b26-4d1e-8ca4-27dce3e0c654)


sed -n -e '3p' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/c838b70d-701e-4449-94a0-f1fbd05827eb)

sed -n -e '$p' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/ab626de2-1695-4bb8-9fbc-338bfa481d2e)


sed  -e 's/Ram/Sita/' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/849a06dd-1368-4c46-9096-43b5b3274b4e)


sed  -e '2s/Ram/Sita/' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/69834117-d106-4bb6-8763-5c79e4f9a8ac)


sed  '/tom/s/5000/6000/' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/90af0a24-86ca-40bd-a7b0-f9d2cf8557a8)


sed -n -e '1,5p' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/2f7f17ac-5448-415a-8335-d04512ba5b5b)


sed -n -e '2,/Joe/p' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/63710572-e053-4d0f-90d6-33c2923902d5)



sed -n -e '/tom/,/Joe/p' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/888ff5cd-e638-488c-85d6-779002a9c75f)


seq 10 
## OUTPUT

![image](https://github.com/user-attachments/assets/4e42c455-ad40-47e4-9d52-fec9f75a4c4d)



seq 10 | sed -n '4,6p'
## OUTPUT

![image](https://github.com/user-attachments/assets/28b1a2dc-0fe1-4c3f-bf06-79ab8f08cebf)


seq 10 | sed -n '2,~4p'
## OUTPUT

![image](https://github.com/user-attachments/assets/6643dec4-314e-469b-bd95-9f7eecf9a1ad)


seq 3 | sed '2a hello'
## OUTPUT

![image](https://github.com/user-attachments/assets/c8728325-0805-4ef1-a453-780cf493eeeb)


seq 2 | sed '2i hello'
## OUTPUT

![image](https://github.com/user-attachments/assets/143fcf44-dae5-4f8a-a0e4-928944f382ef)


seq 10 | sed '2,9c hello'
## OUTPUT

![image](https://github.com/user-attachments/assets/c7077efb-659c-4923-826f-2ddef1c07799)


sed -n '2,4{s/^/$/;p}' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/ca231258-a793-4988-b580-0eb4c5fecdb8)


sed -n '2,4{s/$/*/;p}' file23
## output

![image](https://github.com/user-attachments/assets/fe4adbe9-625f-4c82-ab48-c846ba90868b)


#Sorting File content
cat > file21

![image](https://github.com/user-attachments/assets/37562e80-6401-4d45-8934-6f147e4e9a3f)

sort file21
## OUTPUT


cat > file22

![image](https://github.com/user-attachments/assets/d56f5465-2528-4e8e-9b48-bac2826ed41b)

uniq file22
## OUTPUT

![image](https://github.com/user-attachments/assets/131f961d-6910-438c-80a3-388e0e94edf6)



#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
 
 ![image](https://github.com/user-attachments/assets/d5495113-89e0-4f2a-b23a-035f922ccfbb)


cat < urllist.txt

![image](https://github.com/user-attachments/assets/ebeacd13-d006-4b89-9fd2-18f7f492b557)

cat > urllist.txt

![image](https://github.com/user-attachments/assets/ae5b9c5a-5af4-4621-9dfa-fab2d73d2ead)

cat urllist.txt | tr -d ' '
 ## OUTPUT

![image](https://github.com/user-attachments/assets/a1ab3eb4-286e-4f60-9a88-3ff80b01dff5)

 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT

![image](https://github.com/user-attachments/assets/530874ea-db69-4077-aaf0-423335d5e053)


#Backup commands
tar -cvf backup.tar *
## OUTPUT

![image](https://github.com/user-attachments/assets/ab8d2c21-4ef5-4e7d-8f6d-d7080e55c2d9)

mkdir backupdir
 
mv backup.tar backupdir
 
tar -tvf backup.tar
## OUTPUT

![image](https://github.com/user-attachments/assets/adf1f476-3321-4553-a18d-efa318763f25)

tar -xvf backup.tar
## OUTPUT

![image](https://github.com/user-attachments/assets/b3d7de72-5e8d-4ac4-b6d3-d14561ad2a12)

gzip backup.tar

ls .gz
## OUTPUT
![image](https://github.com/user-attachments/assets/e533c57d-d684-4fda-bda2-730054d94fa3)

gunzip backup.tar.gz
## OUTPUT
![image](https://github.com/user-attachments/assets/b43134ab-45c8-4f82-840b-b3d0cc6e3bf2)

 
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT
![image](https://github.com/user-attachments/assets/fb771271-1acb-4e7f-8c76-4317b2da2edc)

 
cat << stop > herecheck.txt
```
	hello in this world
	i cant stop
	for this non stop movement
	stop
```

cat herecheck.txt
## OUTPUT

![image](https://github.com/user-attachments/assets/59327df5-9e96-4ffd-a56f-e6a147d44e46)

cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT

![image](https://github.com/user-attachments/assets/9f2bb8d9-c142-40fc-9bdf-2dc17ed04620)

ls file1
## OUTPUT
![image](https://github.com/user-attachments/assets/51b6df82-edab-46a0-a9a0-2267d60a08ae)

echo $?
## OUTPUT 
./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 ![image](https://github.com/user-attachments/assets/b9e13e74-b138-40d6-b4e0-3ff45915b7f2)

abcd
 
echo $?
 ## OUTPUT
 
![image](https://github.com/user-attachments/assets/beacb29f-d725-47c1-9f27-a875a6e6d3a7)


 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
##OUTPUT

![image](https://github.com/user-attachments/assets/c8288f2b-f7dc-4e10-b6e8-6de67257a586)

chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT

![image](https://github.com/user-attachments/assets/e4a44094-1e54-4723-b10f-4c3c84617c63)


# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT
![image](https://github.com/user-attachments/assets/4c468ffe-1c3c-448b-b8e1-2c9073bbd497)

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
 ifnested.sh cat
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT

![image](https://github.com/user-attachments/assets/d0e61ca8-a8d5-4d0a-82cb-967f37adbfe9)


# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT
![image](https://github.com/user-attachments/assets/4758e6fe-62f0-4773-9572-f65ab17a1d26)

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT
![image](https://github.com/user-attachments/assets/5cf6546e-fef5-4989-a0be-78ff87394d13)

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT

![image](https://github.com/user-attachments/assets/f2d0cd9a-d5cc-4ed4-a193-4947fc317703)

# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT
![image](https://github.com/user-attachments/assets/d5d65589-fbbb-439b-b782-8326b5882b44)

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 
 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 
 
cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 
 
 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
 
cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT
![image](https://github.com/user-attachments/assets/86a517d9-cea6-4199-8232-42368a69676d)

cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT

![image](https://github.com/user-attachments/assets/b6dc4041-5bd0-45f3-a341-c6f9c13b7df5)

cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT
![image](https://github.com/user-attachments/assets/2bfad863-3cb4-42ab-943d-603a8be06772)

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT
![image](https://github.com/user-attachments/assets/59b2773a-9b2b-4eea-afef-56e2720ac32f)

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT

 ![image](https://github.com/user-attachments/assets/ca147dae-d6b6-41de-8f90-5424d0231505)

cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT
![image](https://github.com/user-attachments/assets/07f8d2d9-46c4-4264-9850-ff7d748cc81d)

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 ![image](https://github.com/user-attachments/assets/80121648-4b08-40b7-a391-5d61c25642eb)

cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT

![image](https://github.com/user-attachments/assets/4b8c1300-4876-466e-88ab-f4db053e9a3c)

 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT

![image](https://github.com/user-attachments/assets/4689a7bc-410c-499b-a7cb-3180b3958b30)


$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
![image](https://github.com/user-attachments/assets/09abab30-71d0-45af-ae93-63e0375db8f7)

 ./funcex.sh 

 
 ./funcex.sh 1 2

 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
![image](https://github.com/user-attachments/assets/bed2b77a-0efe-42ae-aba7-d1f215e130e1)

$ ./argshift.sh 1 2 3
 
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
![image](https://github.com/user-attachments/assets/f283724c-a1dd-4e84-9e11-8a48f9cbf2ab)

 ./argshift.sh 1 2 3
 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
![image](https://github.com/user-attachments/assets/b61ef45e-6550-4747-ad60-e47797ec7682)

 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 
![image](https://github.com/user-attachments/assets/12a4bd44-90e0-4479-8cbe-c31044aec02b)


# RESULT:
The Commands are executed successfully.
