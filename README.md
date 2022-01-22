#include <stdio.h>  
#include <math.h>  
#include <stdlib.h>  
  
int main()  
{  
    // declaration of local variable op;  
    int op, n1, n2;  
    float res;  
    char ch;  
    do  
    {  
        // displays the multiple operations of the C Calculator  
        printf (" Select an operation to perform the calculation in C Calculator: ");  
        printf (" \n 1 Addition  \t \t 2 Subtraction \n 3 Multiplication \t 4 Division \n 5 Square \t \t     6 Square Root \n 7 Sin \t \t         8 Cos \n 9 Tan\t \t         10 Sinh \n 11 Cosh \t \t     12 Tanh \n 13 Log10\t \t     14 Exponent\n 15 EXIT\n\nPlease, Make a choice ");      
          
        scanf ("%d", &op); // accepts a numeric input to choose the operation  
      
      
    // use switch statement to call an operation  
    switch (op)  
    {  
        case 1:  
            // Add two numbers  
            printf (" You chose: Addition");  
            printf ("\n Enter First Number: ");  
            scanf (" %d", &n1);  
            printf (" Enter Second Number: ");  
            scanf (" %d", &n2);  
            res = n1 + n2; // Add two numbers  
            printf (" Addition of two numbers is: %.2f", res);  
            break; // break the function  
              
        case 2:  
            // Subtract two numbers  
            printf (" You chose: Subtraction");  
            printf ("\n Enter First Number: ");  
            scanf (" %d", &n1);  
            printf (" Enter Second Number: ");  
            scanf (" %d", &n2);  
            res = n1 - n2; // subtract two numbers  
            printf (" Subtraction of two numbers is: %.2f", res);  
            break; // break the function  
              
        case 3:  
            // Multiplication of the numbers  
            printf (" You chose: Multiplication");  
            printf ("\n Enter First Number: ");  
            scanf (" %d", &n1);  
            printf (" Enter Second Number: ");  
            scanf (" %d", &n2);  
            res = n1 * n2; // multiply two numbers  
            printf (" Multiplication of two numbers is: %.2f", res);  
            break; // break the function  
              
        case 4:  
            // Division of the numbers  
            printf (" You chose: Division");  
            printf ("\n Enter First Number: ");  
            scanf (" %d", &n1);  
            printf (" Enter Second Number: ");  
            scanf (" %d", &n2);  
            if (n2 == 0)  
                {  
                    printf (" \n Divisor cannot be zero. Please enter another value ");  
                    scanf ("%d", &n2);        
                }  
            res = n1 / n2; // divide two numbers  
            printf (" Division of two numbers is: %.2f", res);  
            break; // break the function  
              
        case 5:  
            // getting square of a number  
            printf (" You chose: Square");  
            printf ("\n Enter First Number: ");  
            scanf (" %d", &n1);  
  
            res = n1 * n1; // get square of a number  
            printf (" Square of %d number is: %.2f", n1, res);  
            break; // break the function  
              
        case 6:  
            // getting the square root of the number  
            printf (" You chose: Square Root");  
            printf ("\n Enter First Number: ");  
            scanf (" %d", &n1);  
              
            res = sqrt(n1); // use sqrt() function to find the Square Root   
            printf (" Square Root of %d numbers is: %.2f", n1, res);  
            break; // break the function  
        
         case 7:  // getting the sin of the number
            printf (" You chose: sin funtion");  
            printf ("\n Enter the Number: ");  
            scanf (" %d", &n1);  
            res=sin (n1*3.1415926/180);
            printf (" sin %d is: %.2f",n1,res);  
            break; // break the function  
          case 8:  // getting the cos of the number
            printf (" You chose: cos funtion");  
            printf ("\n Enter the Number: ");  
            scanf (" %d", &n1);  
            res=cos (n1*3.1415926/180);
            printf (" cos %d is: %.2f",n1,res);  
            break; // break the function  
        case 9:  // getting the tan of the number
            printf (" You chose: tan funtion");  
            printf ("\n Enter the Number: ");  
            scanf (" %d", &n1);  
            res=tan (n1*3.1415926/180);
            printf (" tan %d is: %.2f",n1,res);  
            break; // break the function  
         case 10:  // getting the sinh of the number
            printf (" You chose: sinh funtion");  
            printf ("\n Enter the Number: ");  
            scanf (" %d", &n1);  
            res=sinh(n1);
            printf (" sinh %d is: %.2f",n1,res);  
            break; // break the function  
         case 11:// getting the cosh of the number  
            printf (" You chose: cosh funtion");  
            printf ("\n Enter the Number: ");  
            scanf (" %d", &n1);  
            res=cosh(n1);
            printf (" cos h %d is: %.2f",n1,res);  
            break; // break the function  
        case 12:  // getting the tanh of the number
            printf (" You chose: tanh funtion");  
            printf ("\n Enter the Number: ");  
            scanf (" %d", &n1);  
            res=tanh(n1);
            printf (" tanh %d is: %.2f",n1,res);  
            break; // break the function  
        case 13: // getting the log10 of the number 
            printf (" You chose: log 10 funtion");  
            printf ("\n Enter the Number: ");  
            scanf (" %d", &n1);  
            res=log(n1);
            printf (" log10 %d is: %.2f",n1,res);  
            break; // break the function  
         case 14:  // getting the power of the number
            printf (" You chose: power funtion");  
            printf ("\n x^y ");  
            printf ("\n Enter the Number x "); 
             scanf (" %d", &n1); 
             printf ("\n Enter the Number y ");  
            scanf (" %d", &n2);  
            res=pow(n1,n2);
            printf (" %d^%d is: %.2f",n1,n2,n1,res);  
            break; // break the function  
                      
          case 15: //exit
            printf (" You chose: Exit");  
            exit(0);   
            break; // break the function  
        
            
        default:  
            printf(" Something is wrong!! ");  
            break;                        
    }  
    printf (" \n \n ********************************************** \n ");  
    } while (op != 15);  
  
    return 0;        
}  //program by Rakesh RA2111004010259
