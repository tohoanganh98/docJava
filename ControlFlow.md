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
