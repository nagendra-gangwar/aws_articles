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



# additional notes

* no white space with assignment operator
* 
