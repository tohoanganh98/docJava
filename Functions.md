- Quy tắc của Functions
- 
## Quy tắc
- Một hàm có thể truyền một, nhiều tham số hoặc có thể không truyền tham số nào(hàm Main).
- Một hàm có thể trả về một giá trị hoặc không trả về gì cả.
- Các biến bên trong hàm chỉ có thể sử dụng bên trong hàm đó.
## Writing a Function - Example
```
int print_table(double start, double end, double step) 
{
double d; 
int lines = 1; 
printf("Celsius\tFarenheit\n");
  for(d = start; d <= end; d += step, lines++) 
    printf("%.1lf\t%.1lf\n", d, d * 1.8 + 32);
return lines; 
}
- int print_table : Đây là kiểu dữ liệu trả về của hàm.
- double start, double end, double step : Đây là các tham số truyền vào.
- return lines; : Đây là giá trị trả về cho hàm.
```

*NOTE*
- Kiểu dữ liệu khai báo và giá trị trả về phải cùng một kiểu dữ liệu.
- Tên hàm phải rõ ràng mỗi chức năng phải có một tên duy nhất để phân biệt với các chức năng khác trong chương trình.
- Nếu hàm đó có giá trị trả về thì phải được sử dụng từ khóa "return".

## Calling a Function - Example
```
#include <stdio.h> 
int print_table(double, double, double);
int main(void) 
{
int how_many; 
double end = 100.0;
how_many = print_table(1.0, end, 3);
print_table(end, 200, 15); 
return 0; 
} 
```
