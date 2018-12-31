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
