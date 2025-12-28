# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:

    #include <stdio.h>
    
    int main() {
    
    int i;
    
    float f;
    
    char ch,str[100];
    
    printf("Enter your literal values:\n");
    
    scanf("%d %f %c %s",&i,&f,&ch,str);
    
    printf("Integer = %d,  size = %d\n",i,sizeof(i));
    
    printf("Float = %.2f,  size = %d\n",f,sizeof(f));
    
    printf("Character = %c,  size = %d\n",ch,sizeof(ch));
    
    printf("String = %s,  size = %d\n",str,sizeof(str));
    
    return 0;
}

# Output:
    
<img width="388" height="286" alt="Screenshot 2025-12-28 095515" src="https://github.com/user-attachments/assets/b5fece2e-e43b-4bac-9a18-9cecbff2a73b" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:

     #include <stdio.h>
     
     #define PI 3.14159
     
     int main() {
     
     const int DAYS = 7;
     
     printf("The value of PI (Macro Constant) = %.5f\n", PI);
     
     printf("The value of DAYS (Constant Variable) = %d\n", DAYS);
    
    return 0; 
}
# Output:

<img width="484" height="171" alt="image" src="https://github.com/user-attachments/assets/da70bf1e-4951-4704-9aaa-4209d3144a3a" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
   
    #include <stdio.h>
    
    int main() {
    
    int n;
    
    float f;
    
    double lar;
    
    char ch;
    
    printf("Enter your vales\n");
    
    scanf("%d %f %lf %c",&n,&f,&lar,&ch);
    
    printf("Integer = %d\nFloat = %.2f\nDouble = %.4lf\nCharacter = %c\n",n,f,lar,ch);
    
    return 0;
}
# Output:

<img width="309" height="299" alt="Screenshot 2025-12-28 101602" src="https://github.com/user-attachments/assets/94a0b8a5-df64-4269-bdb7-b4ebcf7e9709" />

# Result: 

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
    
    #include <stdio.h>
    
    int main() {
    
    int a, b;
    
    printf("Enter two values:a,b\n");
    
    scanf("%d %d",&a,&b);
    
    printf("Arithmetic Operations\n");
    
    printf("Addition  = %d\nSubtract= %d\nMultiply = %d\n",a+b,a-b,a*b);
    
    if (b != 0) {
    
        printf("Divide = %d\nRemainder = %d\n", a/b,a%b);
   
    } else {
    
        printf("Division and Remainder not possible (b = 0)\n");
    } 
    
    printf("\nBitwise Operations\n");
    
    printf("AND = %d\nOR = %d\nXOR = %d\nLeft Shift = %d\nRight Shift = %d\nNOT (~a) = %d\nNOT (~b) = %d\n",a&b, a|b, a^b,  a <<1,a>>1,~a, ~b);
    
    return 0;
}
# Output:

<img width="290" height="532" alt="Screenshot 2025-12-28 103649" src="https://github.com/user-attachments/assets/f71ef4ce-de2f-4548-8180-1b886fcab5af" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
    
    #include <stdio.h>
    
    int main() {
    
    char ch;
    
    printf("Enter a character:\n");
    
    scanf("%c", &ch);
    
    (ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z') ?
    
        ((ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U'||
        
          ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u') ?
          
            printf("It is a Vowel.\n") :
            
            printf("It is a Consonant.\n")) :
   
    (ch >= '0' && ch <= '9') ?
    
        printf("It is a Digit.\n") :
        
        printf("It is a Special Symbol.\n");
    
    return 0;
}

# Output:
<img width="368" height="116" alt="image" src="https://github.com/user-attachments/assets/3044eff4-18a2-4089-804a-3b4e34029e61" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


