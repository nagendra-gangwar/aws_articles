# variables 

myVariable1='Test'  
echo $myVariable1;

* variables can be read only and unset using following commands

readonly myVariable1  
unset myVariable1

* use local to define local varibales within a method 

setAge() {  
    local AGE=25  
    echo "Local Variable Age: $AGE"  
}

# comments

* Single line comments starts with #
* multi line comments starts with : ' and ends with '

# arrays 
* iterate all values
num=(1 3 5 9 10)  

for i in "${num[@]}"  
do   
  echo "$i"  
done  

* iterate all indexes

num=(1 3 5 9 10) 

for i in "${!num[@]}" 
do   
  echo "${num[$i]} \n"  
done  

array[-1]=22	Add element to array at last position.  
array+=(11)	Append value to an array  

# Strings 

var1='hello'  
var2="nagendra"  

echo "${var1}, ${var2} to the shell programming"  

# conditions

<img width="536" alt="image" src="https://user-images.githubusercontent.com/58660785/158052059-44ce3b3d-50e4-4ce6-b59a-ed669ad6cd62.png">

# find out file details 

filepath="/home/kbabu/run.sh"  
filename=$(basename "$filepath")  
echo "File :$filename"  
echo "File Name: ${filename%.*}"  
echo "File Extension: ${filename##*.}"  

# spliting string 

input="one-two-three"  
IFS='-' array=($input)  
for element in ${array[@]}  
do  
    echo $element  
done  

# Joining array

nums=(1 3 10 7 6 9 15)  
All=""  
for ((i=0;i<${#nums[@]};i++))  
do  
    All="$All,${nums[$i]}"  
done  
echo "${All:1}"  

# additional notes

* no white space with assignment operator
* no comma between elements of arrays
* 
