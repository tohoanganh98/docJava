# Operators in C
- Toán tử số học
- Tăng và giảm
- Toán tử so sánh
- Toán tử biểu thức điều kiện
## Toán tử số học
***C supports the arithmetic operators:***
- + addition
- - subtraction
- (*) multiplication
- / division***
- % modulo (remainder
## ÉP Kiểu Dữ Liệu
- int i = 3, j = 2; double f; 
- f = (double)i / j = 1.5; 
- f = i / (double)j = 1.5; 
- f = (double)i / (double)j = 1.5; 
- f = (double)(i / j) = 1.0000;

```Khi một số nguyên chia cho một số nguyên ta sẽ chỉ nhận được một số nguyên, còn nếu một số thực chia cho một số nguyên kết quả nhận được sẽ là một số thực.Vì vậy khi bạn muốn có một số thực nhưng số chia và số bị chia của bạn lại là số nguyên vậy bận phải sử dụng kĩ thuật ép kiểu 1 trong 2 số đó về kiểu số thực hoặc cả 2 số đó```
## True False trong C
```Không có kiểu dữ liệu boolean trong C, các số nguyên được sử dụng thay thế ?? Giá trị 0 (hoặc 0.0) là sai ?? Bất kỳ giá trị nào khác 0 la 1, -1, 0,3, -20,8 ... là đúng```
## Toán tử so sánh
- < less than 
- <= less than or equal to 
- > greater than 
- >= greater than or equal to 
- == is equal to 
- != is not equal to 
## Toán tử biểu thức điều kiện
- && and 
- || or 
- ! not
###Truth Table 
| && | False | True |
|----|-------|------|
| False | False | False | 
| True  | False | True  |
| || | False | True |
|----|-------|------|
| False | False | True | 
| True  | True | True  |

 
