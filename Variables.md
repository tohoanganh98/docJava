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
