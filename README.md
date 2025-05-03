# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main(){
    
    int i,num;
    for(i=0;i<60;i++){
        num=i;
    }
    printf("After Right Shift Operation value of a is:%d",num>>3);
    return 0;
}
```

## OUTPUT
![438647562-c7f129f2-c0b3-422b-8d40-dbab0799b361](https://github.com/user-attachments/assets/0ba0d3a4-949f-49d6-b5a2-d54f20600f87)










## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main(){
    int a,b,c;
    scanf("%d%d%d",&a,&b,&c);
    if(a<b && a<c){
        printf("%d is the smallest number.",a);
    }
    else if(b<a && b<c){
           printf("%d is the smallest number.",b);
    }
    else{
           printf("%d is the smallest number.",c);
    }
}
```

## OUTPUT
![438649099-f058e602-ca29-4895-b80a-46fd042a8e62](https://github.com/user-attachments/assets/078e38c7-9f50-474b-b571-d09f0d6a7cd7)

           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <ctype.h>
#include <string.h>

int main() {
    char str[100];
    scanf("%s", str);
    for (int i = 0; str[i]; i++) {
        str[i] = tolower(str[i]);
    }
    printf("Lower case String is:%s\n", str);

    return 0;
}
```

## OUTPUT
![438650090-7e02c218-2635-443a-ac8c-dfb22851be64](https://github.com/user-attachments/assets/bb74a8ef-c6fc-4434-a25b-9fe78b20b8fa)





## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <string.h>
int main(){
   char str1[100],str2[100],merged[200];
   int i=0,j=0,count=0;
   scanf("%s %s",str1,str2);
   do
   {
       merged[i]=str1[i];
   }while(str1[i++] != '\0');
   i--;
   do{
      merged[i++] = str2[j];
   }while(str2[j++] != '\0');
   i=0;
   do{
       if (merged[i] != '\0')
       count++;
   }while(merged[i++] !='\0');
   printf("%s\n%d",merged,count);
   return 0;
}
```

## OUTPUT
![438652156-42d0a93e-71c7-4751-950d-75bf128b87f3](https://github.com/user-attachments/assets/4ab2b36b-b92e-402b-866a-d30b1e67234e)





## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
#include <stdio.h>
#include <string.h>
int main(){
    char str1[100],str2[100];
    int i=0,count=0;
    fgets(str1,sizeof(str1),stdin);
     fgets(str2,sizeof(str2),stdin);
     
    while(str1[i] != '\0' || str2[i] != '\0'){
        if(str1[i]  != str2[i]){
            count =1;
            break;
        }
        i++;
        
    }
    if(count ==0){
        printf("strings are same");
    }
    else{
        printf("strings are not same");
    }
}
```


## OUTPUT
![438652939-cd7c65a7-1b30-48eb-85c8-8c88dc1a586b](https://github.com/user-attachments/assets/08b2174c-4f4d-4082-bd93-5a461473da3e)

 

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

