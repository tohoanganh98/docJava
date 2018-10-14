# C Basic
## A C Program

### Include
```Lệnh #include chỉ thị cho Trình tiền xử lý C (một trình soạn thảo không tương tác sẽ được thảo luận sau) để tìm tệp văn bản “stdio.h”```
### Comments
```Nhận xét được đặt trong / * và * / chuỗi ký tự khi bạn comment đoạn code đó sẽ không ảnh hưởng đến chương trình chạy của bạn```
### Main Fuction
``` The main function là quan trọng nhất. Điều này xác định điểm mà tại đó chương trình của bạn bắt đầu thực thi. Nếu bạn không viết một main fuction chương trình của bạn sẽ không chạy (nó sẽ không có điểm bắt đầu). Trong thực tế, nó thậm chí sẽ không biên dịch.```
### { }

```Đây là 1 block code trong ngôn ngữ lập trình C sử dụng dấu ngoặc kép “{” có nghĩa là “bắt đầu” và “}” có nghĩa là “kết thúc”. Họ dễ dàng hơn để gõ và sau một thời gian, dễ đọc hơn rất nhiều. ```
### printf
```Hàm này được định nghĩa trong Thư viện chuẩn, hàm này có chức năng là in ra màn hình hiển thị cho người dùng```
### scanf
```Hàm scanf là "đối diện" của printf. Trong khi printf tạo ra đầu ra trên màn hình, scanf đọc từ bàn phím. Trình tự “% d” chỉ thị cho scanf đọc một số nguyên từ bàn phím. Bởi vì “% d% d” được sử dụng hai số nguyên sẽ được đọc. Giá trị đầu tiên được nhập vào biến “a”, biến thứ hai thành biến “b”.```

### \n
```
Trình tự của hai ký tự “\” theo sau là “n” là cách C xử lý các dòng mới. Khi in nó di chuyển con trỏ đến đầu dòng tiếp theo.
```
### return
```trở lại gây ra giá trị, ở đây 0, được chuyển trở lại hệ điều hành.Trả về 0 có nghĩa là thành công. Giá trị 1, 2, 3, v.v. cho biết lỗi.```

## The Format of C
### Dấu ;
```Dấu chấm phẩy là rất quan trọng trong C. Họ tạo thành một terminator tuyên bố - họ nói với trình biên dịch, nơi một tuyên bố kết thúc và tiếp theo bắt đầu. Nếu bạn không đặt một cái sau mỗi câu lệnh, bạn sẽ nhận được các lỗi biên dịch.```
### Trường hợp nhạy cảm cần lưu ý
```C là một ngôn ngữ nhạy cảm. Mặc dù int biên dịch, "Int", "INT" hoặc bất kỳ biến thể nào khác sẽ không. Tất cả 40 từ khóa C đều là chữ thường. Tất cả hàng trăm hàm trong Thư viện Chuẩn đều là chữ thường..```
## Variables
***Các biến phải được khai báo trước khi sử dụng ngay sau “{” Ký tự hợp lệ là chữ cái, chữ số và “_” Ký tự đầu tiên không thể là ký tự 31 chữ số được nhận dạng cho biến cục bộ (có thể sử dụng nhiều hơn, nhưng bị bỏ qua) Một số triển khai chỉ nhận ra 6 ký tự biến toàn cục (và tên hàm)! Chữ hoa và chữ thường là khác biệt***
### Khai báo biến
```Trong C, tất cả các biến phải được khai báo trước khi sử dụng. Trong C, bạn lập trình viên phải khai báo tất cả các biến và cung cấp cho mỗi loại một (và tốt hơn là một giá trị khởi tạo).```
### Tên Biến Hợp Lệ
```Chỉ chữ cái, chữ số và ký tự gạch dưới có thể được sử dụng hợp lệ trong các tên biến. Ký tự đầu tiên của một biến có thể là một chữ cái hoặc dấu gạch dưới, mặc dù The Standard nói để tránh việc sử dụng dấu gạch dưới làm chữ cái đầu tiên. Vì vậy, các tên biến “temp_in_celsius”, “index32” và “sine_value” đều hợp lệ, trong khi “32index”, “temp-in-celsius” và “sine $ value” thì không. Sử dụng tên biến như “_sine” sẽ bị cau mày, mặc dù không phải cú pháp không hợp lệ```
### Chữ In Hoa
```Chữ hoa có thể được sử dụng trong các tên biến nếu muốn. Chúng thường được sử dụng như là một thay thế cho các ký tự gạch dưới, do đó "temp_in_celcius" có thể được viết là "tempInCelsius". Kiểu đặt tên này đã trở nên khá phổ biến trong những năm gần đây và dấu gạch dưới đã rơi vào tình trạng không sử dụng.```
### Printf and Scanf
- printf ghi các giá trị số nguyên vào màn hình khi% d được sử dụng
- scanf đọc các giá trị số nguyên từ bàn phím khi% d được sử dụng
- "&" RẤT quan trọng với scanf (yêu cầu thay đổi tham số, điều này sẽ được điều tra sau) - không có sẽ làm cho chương trình bị lỗi
- “&” Không cần thiết với printf vì giá trị hiện tại của tham số được sử dụng
### printf
```Hàm printf ghi đầu ra vào màn hình. Khi nó đáp ứng các định dạng specifier% i, một số nguyên là đầu ra.```
### scanf
```Chức năng scanf đọc đầu vào từ bàn phím. Khi nó đáp ứng các định dạng specifier% i chương trình chờ cho người dùng gõ một số nguyên.```
