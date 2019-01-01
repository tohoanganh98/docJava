**1. Write a program in “QUANT.C” which “quantifies” numbers.**

**Read an integer “x” and test it, producing the following output:**

**x greater than or equal to 1000 print “hugely positive”**

**x from 999 to 100 (including 100) print “very positive”**

**x between 100 and 0 print “positive” x exactly 0 print “zero”**

**x between 0 and -100 print “negative”** 

**x from -100 to 999 (including 100) print “very negative”**

**x less than or equal to -1000 print “hugely negative”**

**Thus -10 would print “negative”, -100 “very negative” and 458 “very positive”.** 

**In the following solution the words “very” and “hugely” are printed separately from “positive” and “negative”.**

```
#include <stdio.h> 
 int main(void) { 
 int i; 
 printf("Enter an integer "); 
 scanf("%i", &i); 
 if(i >= 1000 || i <= -1000)
    printf("hugely ");
 else if(i >= 100 || i <= -100)
    printf("very "); 
 if(i > 0)
    printf("positive\n");
 else if(i == 0)
    printf("zero\n");
 else if(i < 0)
    printf("negative\n"); 
 return 0; 
 } 
```
**2. Write a program in “POW.C” which reads two numbers, the first a real, the second an integer. 
The program then outputs the first number raised to the power of the second.**
```
#include <stdio.h> 
 int main(void) 
 {
 int  count = 1; 
 int  p = 0; 
 double  n = 0.0L;
 long double answer = 0.0L; 
 printf("enter the number ");
 scanf("%lf", &n); 
 printf("enter the power ");
 scanf("%d", &p); 
 for(answer = n; count < p; count++){
      answer = answer * n; 
 }
 printf("%.3lf to the power of %d is %.9Lf\n", n, p, answer); 
 return 0;
 } 
```
**3. Write a program in “DRAWX.C” which draws an “x” of user specified height.**
```
#include <stdio.h> 
 int main(void) 
 {
 int height;
 int row;
 int column; 
 printf("Enter height of 'x' ");
 scanf("%i", &height); 
 for(row = 1; row <= height; row++)
 { 
    for(column = 1; column <= height; column++)
    {
       if(row == column || column == height - row + 1)
          printf("*");
       else
          printf(" ");
     }
printf("\n");
} 
return 0;
} 
```
