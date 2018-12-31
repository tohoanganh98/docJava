# Control Flow
- Decisions - if then else
- More decisions - switch
- Loops - while, do while, for 
- Keyword break
- Keyword continue

## Decisions - if then
* Dấu ngoặc đơn bao quanh điều kiện
* Nếu có một câu lệnh thì không cần cặp {}
* Nếu có nhiều hơn một thì bắt buộc phải sử dụng cặp {}

```
scanf("%i", &i);
if(i > 0) 
  printf("a positive number was entered\n"); 
```

```
if(i < 0) 
{
   printf("a negative number was entered\n"); 
   i = -i; 
}
```
## Warning!
* Dấu chấm phẩy sau khi điều kiện tạo thành một câu lệnh kết thúc luôn và nó sẽ không làm gì cả
```
printf("input an integer: "); 
scanf("%i", &j); 
  if(j > 0); 
printf("a positive number was entered\n");

```
- Đã trở nên quen thuộc với ý tưởng đặt các ký tự dấu chấm phẩy sau mỗi câu lệnh trong C, chúng ta bắt đầu thấy rằng từ dấu ; không phải là chỗ nào cũng có thể xuất hiện.
  Dấu chấm phẩy đã được đặt sau điều kiện trong đoạn mã trên. Trình biên dịch xem xét điều này được đặt vì một lý do và làm cho dấu chấm phẩy trở thành một phần của cấu trúc. Một câu lệnh không làm gì được hay một câu lệnh hay không được tạo ra (mỗi máy có một lệnh khiến nó phải chờ một chu kỳ máy). Theo nghĩa đen, nếu j lớn hơn 0, sẽ không có gì được thực hiện. Sau chu kỳ máy, câu lệnh tiếp theo luôn được đưa ra, bất kể không thực hiện.

## Decisions - if then else
* Thêm 1 tùy chọn "else".
* Nếu có một câu lệnh thì để mặc định còn nếu nhiều hơn một bắt buộc phải nằm trong cặp {}.

```
if(i > 0) 
  printf("i is positive\n"); 
else 
  printf("i is negative\n");

```
```
if(i > 0) 
  printf("i is positive\n"); 
else 
{
  printf("i is negative\n"); 
  i = -i; 
}

```
**Khi bạn thêm tùy chọn "else" có nghĩa là sẽ được thực thi khi điều kiện sai**
###### Ví dụ minh họa:
```
if(i > 0) 
{
  printf("i is positive\n");  
}
else {   
  printf("i is negative\n"); 
}
```

## Nesting ifs
###### Ví dụ minh họa:
```
int i = 100;
if(i > 0) 
  if(i > 1000) 
    printf("i is big\n");
  else 
    printf("i is reasonable\n"); 
```
**Nêu không có cặp ngoặc {} thì khi sử dụng else, trình biên dịch sẽ tự hiểu là cặp else với if gần nhất**

```
int i = -20; 
if(i > 0) 
{ 
  if(i > 1000) 
    printf("i is big\n"); 
} 
else printf("i is negative\n");
```
**Nêu có dấu {} sẽ tường minh hơn những câu lệnh khi chúng ta sử dụng câu điều kiện lồng**
## Decisions - if then else if then else
```
if(bieu_thuc_boolean 1)
{
   /* Thuc thi khi bieu thuc boolean 1 la true */
}
else if( bieu_thuc_boolean 2)
{
   /* Thuc thi khi bieu thuc boolean 2 la true */
}
else if( bieu_thuc_boolean 3)
{
   /* Thuc thi khi bieu thuc boolean 3 la true */
}
else 
{
   /* Thuc thi khi tat ca cac bieu thuc boolean tren khong la true */
}
```
## Switch
*Khi bạn có quá nhiều điều kiên cần xử lý thì bạn cần sử dụng Switch-Case.*
```
switch(c) {  
case 'a': case 'A': 
    printf("area = %.2f\n", r * r * pi); 
    break;  
case 'c': case 'C': 
    printf("circumference = %.2f\n", 2 * r * pi);
    break; 
case 'q': 
    printf("quit option chosen\n");
    break;  
default: 
    printf("unknown option chosen\n"); 
    break;
}
```

**Ví dụ so sánh giữa if/then/else  và switch**

*if/then/else*
```
if(c == 'a' || c == 'A')   
  printf("area = %.2f\n", r * r * pi);  
else if(c == 'c' || c == 'C')   
  printf("circumference = %.2f\n", 2 * r * pi);
else if(c == 'q')
  printf("quit option chosen\n");
else 
  printf("unknown option chosen\n");
```
*switch*
```
switch(c)
{    
default:
  printf("unknown option chosen\n");
  break;
case 'q':   
  printf("quit option chosen\n");
  break;
case 'c': case 'C':
  printf("circumference = %.2f\n", 2 * r * pi);
  break; 
case 'a': case 'A': 
  printf("area = %.2f\n", r * r * pi);  
  break;  
}
```

**=>Khi sử dụng switch-case code nhìn rành mạch hơn, hiệu suất sẽ cao hơn so với sử dụng cách thông thường**

*NOTE*
- Sau mỗi case đều phải có break; nếu không câu lệnh sẽ không dừng lại và tiếp tục thực hiện cảu case tiếp theo.
- Sau chữ case là dấu ":".
- Bắt đầu với kết thúc của 1 case sẽ không nằm trong 1 cặp "{}".
- Tất cả case sẽ được bọc trong 1 block code switch(choice){}.

## While Loop
- While là 1 vòng lặp đơn giản nhất trong ngôn ngữ lập trình C.
- Điều kiện phải được nằm trong dấu ().
- Một câu lệnh sẽ tạo thành phần thân của vòng lặp.
- Nếu có 2 câu lệnh trở nên nó phải được bọc trong cặp dấu {}.

```
while(j > 0)
{ 
  printf("j = %i\n", j);
  j--; 
}
```

*NOTE*
- Đưa ra một điều kiện và nó được nằm trong cặp dấu ().
- Nếu điều kiện là True phần thân vòng lặp sẽ được thực hiện.
- Điều kiện vẫn sẽ được đánh giá lại nếu vẫn đúng vòng lặp sẽ tiếp tục cho đến khi điều kiện sai thì vòng lặp sẽ dừng.
- Sau khi vòng lặp dừng thực thi sẽ nhảy đến câu lênh đầu tiên tiếp theo.
*Sau đây là một ví dụ khi người lập trình đưa ra một điều kiện không thể True*

```
int j = 5;
printf("start\n");
  while(j == 0)
    printf("j = %i\n", j--); 
printf("end\n");
```
## Do while
```
int j = -10;
printf("start\n");
do {
    printf("j = %i\n", j);
    j--;
} while(j > 0);
printf("stop\n");

==>Results
start 
j = -10 
stop
```
*NOTE*

Nhìn ví dụ trên các bạn có thể thấy một số vấn đề như sau:
- Cú pháp luôn có do{} trước xong đến While().
- Trong cặp dấu {} của do luôn là chứa câu lệnh thực thi còn trong cặp () của while luôn chứa câu điều kiện của vòng lặp.
- Khi sử dụng do{}-while() câu lệnh thực thi của bạn sẽ luôn được chạy một lần duy nhất cho dù điều kiện có đúng hay sai.(Ví dụ trên)
- Sau While() luôn phải có dấu ;
## for Loop
```
for(initial-part; while-condition; update-part) 
  body;
```
*Sau đây là một ví dụ nhỏ về vòng lặp for*
```
for(j = 5; j > 0; j--) 
{ 
  printf("j = %i ", j); 
  printf("%s\n", ((j%2)==0)?"even":"odd"); 
}
```
*NOTE*

- Vòng lặp for gồm 3 thành phần cơ bản đó là giá trị khởi tạo ban đầu, điều kiện để câu lệnh được viết trong for được thực thi, bước nhảy hay còn gọi là phần cập nhập cho vòng vòng tiếp theo.
- Các thành phần này luôn được ngăn cách nhau bởi dấu ";".

**Sau đây là một ví dụ để cho thấy for là một cách viết khác của while**
```
The construct: 
  for(initial-part; while-condition; update-part)  body; 
 is equivalent to: 
  initial-part; 
  while(while-condition) 
  {  
    body; 
    update-part; 
  }
 
```
- Phần điều kiện bạn phải cẩn thận phân tích bài toán để có thể đưa ra điều kiện hợp lý nhất tránh như trường hợp sau đây:

```
int j; 
printf("start\n"); 
for(j = 5; j == 0; j--) 
    printf("j = %i\n", j);
printf("end\n");

==>Results:
start
end
```
- Bước nhảy trong lập trình C không giới hạn. Bạn có tiến hoặc lùi bao nhiêu đơn vị là tùy bạn phụ thuộc trên bào toán bạn đang làm.

```
#include <math.h> 
int main(void) 
{ 
double angle; 
for(angle = 0.0; angle < 3.14159; angle += 0.2) 
  printf("sine of %.1lf is %.2lf\n", angle, sin(angle));
  return 0;
}
```
## Break
- Từ khóa break buộc thoát ngay lập tức từ vòng lặp gần nhất.
- Hạn chế sử dụng.
```
for(;;) 
{ 
  printf("type an int: "); 
  if(scanf("%i", &j) == 1) 
    break; 
  while((c = getchar()) != '\n') ;
}
printf("j = %i\n", j);

==>Results
 type an int: an int 
 type an int: no 
 type an int: 16
 j = 16
```
## Continue
- Từ Khóa break buộc lần lặp tiếp theo của vòng lặp gần nhất.
- Hạn chế sử dụng.
```
for(j = 1; j <= 10; j++)
{
  if(j % 3 == 0)
  continue; 
  printf("j = %i\n", j);
}
==>Results
j = 1
j = 2
j = 4
j = 5
j = 7
j = 8
j = 10
```
