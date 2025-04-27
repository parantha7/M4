# REG NO: 212224040232
# DATE  : 27-04-25
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
int main() {
    int num = 44;
    int shifts = 3;
    printf("Original number: %d\n", num);
    int result = num << shifts;
    printf("Number after left shift by %d: %d\n", shifts, result);
    return 0;
}
```


## OUTPUT
![Screenshot 2025-04-27 143144](https://github.com/user-attachments/assets/4e164588-ccd5-407b-a858-4353969f03b0)


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
int main() {
    int num1, num2;
    printf("Enter first number: ");
    scanf("%d", &num1);
    printf("Enter second number: ");
    scanf("%d", &num2);
    if (num1 == num2) {
        printf("The two numbers are equal.\n");
    }
    if (num1 != num2) {
        printf("The two numbers are not equal.\n");
    }
    return 0;
}
```



## OUTPUT

![Screenshot 2025-04-27 143544](https://github.com/user-attachments/assets/96d108c9-0354-402d-9cd7-fb5b2bba4176)

           
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
int main() {
    char str[100];
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);
    for (int i = 0; str[i] != '\0'; i++) {
        str[i] = tolowera(str[i]);
    }
    printf("String in lowercase: %s\n", str);
    return 0;
}
```


## OUTPUT

![Screenshot 2025-04-27 144252](https://github.com/user-attachments/assets/8a23de89-158c-4bd1-8dae-73308d41477b)




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
#include <ctype.h>
int main() {
    char str[100];
    int word_count = 0, i = 0;
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);
    do {
        if (i == 0 && !isspace(str[i])) {
            word_count++;
        } else if (isspace(str[i - 1]) && !isspace(str[i])) {
            word_count++;
        }
        i++;
    } while (str[i - 1] != '\0');

    if (isspace(str[i - 2])) {
        word_count--;
    }
    printf("Total number of words: %d\n", word_count);
    return 0;
}
```
## OUTPUT
![Screenshot 2025-04-27 145248](https://github.com/user-attachments/assets/7c1ebb23-306d-41d8-bcfa-fba1eb6206b2)





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
int main() {
    char str1[100], str2[100];
    int i = 0, isEqual = 1;
    printf("Enter first string: ");
    fgets(str1, sizeof(str1), stdin);
    printf("Enter second string: ");
    fgets(str2, sizeof(str2), stdin);
    while (str1[i] != '\0' || str2[i] != '\0') {
        if (str1[i] != str2[i]) {
            isEqual = 0;
            break;
        }
        i++;
    }
    if (isEqual) {
        printf("The strings are equal.\n");
    } else {
        printf("The strings are not equal.\n");
    }
    return 0;
}
```


## OUTPUT
![Screenshot 2025-04-27 145734](https://github.com/user-attachments/assets/88409ca2-371f-4c49-bc61-298dfb77994a)

 

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

