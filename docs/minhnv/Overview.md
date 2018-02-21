# Tư duy lập trình hướng đối tượng 
## I. Khái niệm:

Trước khi tìm hiểu về lập trình hướng đối tượng là gì, chúng ta sẽ cùng đi qua một chút khái niệm về lập trình là gì?

**Lập trình** (coding) khác với hai khái niệm hay bị nhầm lẫn là phát triển (development) và triển khai (implementation).

<ul>
Lập trình là hoạt động viết ra một bản mô tả bằng ngôn ngữ con người có thể hiểu được (human language) hoặc ngôn ngữ thiết bị điện tử có thể hiểu được (machine language) theo một quy tắc nhất định để các thiết bị này thực thi.
</ul>

Trong lối tư duy lập trình cổ điển, quy tắc lập trình dựa trên ba cấu trúc điều khiển (flow control) cơ bản là tuần tự (sequence), rẽ nhánh (conditional) và vòng lặp (loop) mà lập trình viên có thể giải quyết được hầu hết các bài toán. Tuy nhiên, đến những năm thập niên 80 – 90 thì nhu cầu phải giải quyết các bài toán về quản lí trở thành vấn đề khi mà các kiểu dữ liệu nguyên thủy (primitive) không có đủ khả năng để mô tả được các đối tượng như con người, sinh vật, đồ đạc. Và tư duy lập trình hướng đối tượng ra đời mà theo đó:

<ul>
Tư duy lập trình hướng đối tượng là tư duy lập trình mà theo đó tất cả mọi thứ có thể định nghĩa được thuộc tính (properties) và phương thức (method) đều được coi là các đối tượng.
</ul>

Trong nhiều tài liệu có nhắc đến các thuật ngữ liên quan như phân tích, thiết kế, lập trình hướng đối tượng. Đó là các giai đoạn trong phát triển phần mềm, gọi chung là hướng đối tượng.

- Phân tích hướng đối tượng (OOA) là quá trình xem xét bài toán đặt ra để biến nó thành ứng dụng và xác định các đối tượng cũng như sự tương tác lẫn nhau của chúng. Đầu ra của quá trình phân tích là một tập các yêu cầu.

- Thiết kế hướng đối tượng (OOD) là quá trình chuyển đổi các yêu cầu thành đặc tả thực hiện. Người thiết kế phải đặt tên cho các đối tượng, xác định các hành vi, xác định được đối tượng này liên quan tới đối tượng khác như nào.

- Lập trình hướng đối tượng (OOP) là quá trình chuyển đổi các đặc tả của bước thiết kế thành chương trình theo chính xác những yêu cầu ban đầu.

## II. Bốn tính chất của lập trình hướng đối tượng 

Trong lập trình hướng đối tượng bao gồm 4 tính chất là:

- Tính trừu tượng (abstraction)
- Tính đóng gói (encapsulation)
- Tính đa hình (polymorphism) 
- Tính kế thừa (inheritance)

### Tính trừu tượng 

<ul>
Tính trừu tượng được thể hiện qua việc một đối tượng có thể được thực thi và tương tác với các đối tượng khác mà không cần biết tới hoạt động bên trong của đối tượng đó.
</ul>

Ví dụ như chiếc xe máy ta hay đi hàng ngày chỉ cần bạn biết nổ máy, vào số, phanh và một số thứ khác là bạn có thể sử dụng được mà không cần phải hiểu rõ cấu trúc của chiếc xe mình đi, cấu tạo như thế nào, động cơ 4 thì hoạt động ra sao =))) 

Tác dụng lớn nhất của tính chất này là khi tương tác với một đối tượng bất kì bạn phải thiết kế sao cho chỉ quan tâm tới đầu vào (input) và đầu ra (output) thay vì phải tập trung tới xử lí (process) bên trong của đối tượng. Điều này giúp cho việc sử dụng lại phần code, tiện ích của các lập trình viên khác được dễ dàng hơn, giúp tiết kiệm công sức hơn. Đồng thời việc phân chia công việc cho nhiều người làm cũng dễ dàng hơn. Vậy tính trừu tượng đang mô phỏng lại cách mà các đối tượng trong thế giới thực tương tác với nhau.

### Tính đóng gói 

<ul>
Tính đóng gói được thể hiện qua việc mỗi một đối tượng có một phạm vi tương tác cụ thể. Nếu trong C là khái niệm về namespace thì trong Java là khái niệm về package.
</ul>

Việc xây dựng tính đóng gói hay xây dựng phạm phi được phép truy cập, sử dụng và điều khiển các đối tượng thường được hiểu là có chức năng giống với khái niệm trừu tượng. Tuy nhiên mục tiêu chính của tính chất này là đảm bảo giới hạn sự thay đổi từ bên ngoài với các thành phần bên trong của đối tượng. Ví dụ bạn không phải là thành viên trong nhà thì sẽ không được vào trong nhà và sử dụng đồ đạc. Nắm được tính chất này tức là bạn phải phân quyền được cụ thể các thuộc tính và phương thức của một đối tượng. Có một quy tắc nhỏ với tính chất này đó là đối tượng của bạn càng đóng thì càng khó tùy biến nhưng nếu càng mở thì càng dễ xảy ra lỗi ngoại lệ. 

### Tính kế thừa 

<ul>
Tính kế thừa là tính chất mà một đối tượng bất kì có thể sử dụng lại định nghĩa (mô tả) của một đối tượng khác.
</ul>

Ví dụ cuộc sống mà tính chất này mô tả chính là việc con thừa kế cha. Thừa kế ở đây không chỉ hiểu hẹp ở mức thừa kế lại tài sản mà phải hiểu rằng đối tượng con đang kế thừa tính chất, tính cách của đối tượng cha.

### Tính đa hình 

<ul>
Tính đa hình trong lập trình hướng đối tượng là việc cung cấp một giao diện đơn (single interface) cho các thực thể (entity) của các kiểu (type) khác nhau.
</ul>

Tính đa hình mô phỏng lại việc mỗi đối tượng ở trong những hoàn cảnh khác nhau lại có những hình thái khác nhau. Ví dụ như khi bạn là sinh viên đến trường bạn sẽ mang nhưng tính chất, đặc điểm, hoạt động của một sinh viên còn khi về nhà thì bạn là mang tính chất, đặc điểm, hoạt động của một người con, người anh. Hoặc giống như bạn đổ nước vào cốc hình vuông thì nó sẽ có dạng theo cốc đó còn khi bạn đổ vào lọ hình cầu thì nó lại có dạng hình cầu... Qua đó để mô phỏng lại việc này thì đối tượng thầy sẽ cung cấp ra một danh sách các thuộc tính cũng như phương thức được xác định trước (khái niệm interface) và trong mỗi một hoàn cảnh, ở một cương vị khác nhau (khái niệm type) thì người thầy lúc đó (khái niệm entity) sẽ có những thể hiện khác nhau.  

Tính đa hình có 3 kiểu như sau: 

- Kiểu đầu tiên là mức thuộc tính (parametric polymorphism). Khi mà code được viết ra mà không cần khai báo kiểu dữ liệu cho thuộc tính của đối tượng. Trong phần lớn các ngôn ngữ lập trình đã hỗ trợ kiểu đa hình này thông qua khái niệm generic.

- Kiểu thứ hai là mức phương thức (ad hoc polymorphism). Kiểu đa hình này được thể hiện thông qua việc một hàm(function) có khả năng được lập trình và có những biểu hiện khác nhau dựa trên các kiểu đối số khác nhau. Các ngôn ngữ lập trình hướng đối tượng hỗ trợ kiểu đa hình này thông qua khái niệm **overloading**. Ví dụ đặc trưng trong lập trình đó là phép toán cộng ‘+’. Khi đối số truyền vào là hai số kiểu integer, ‘+’ thực hiện cộng hai số. Khi đối số truyền vào là string, ‘+’ lại thực hiện phép nối chuỗi.

- Kiểu cuối cùng là ở mức kế thừa (inclusion polymorphism). Khác với hai kiểu trên, việc đa hình được thể hiện thông qua thời điểm sử dụng. Tức là đối tượng thầy giáo phải đến trường mới thực hiện thay đồng phục và thực hiện các hành vi tương ứng của thầy giáo. Kiểu đa hình thứ ba này là kiểu nạp chồng lên làm thay đổi những phương thức có sẵn của lớp cha. Các ngôn ngữ lập trình hỗ trợ tính đa hình này thông qua khái niệm **overriding**.

## III. Vai trò

**Tính mạnh mẽ**: phần mềm có khả năng xử lý biệt lệ mà không được xác định rõ ràng.

Ví dụ :

- Phần mềm điều khiển nhà máy hạt nhân
- Phần mềm điều khiển máy bay

**Khả năng thích nghi**: phần mềm có thể phát triển theo thời gian để đáp ứng theo nhu cầu sử dụng.

=> Dễ mở rộng dự án, dễ dàng quản lý code

Ví dụ :

- Trình duyệt và các công cụ tìm kiếm được được sử dụng từ nhiều năm nay

**Khả năng tái sử dụng**: một đoạn mã có thể được sử dụng trong các hệ thống khác nhau, các ứng dụng khác nhau.

=> Tiết kiệm tài nguyên, tiền bạc và thời gian

## IV. Ví dụ 

## Tài liệu tham khảo

- http://www.stroustrup.com/glossary.html#Gpolymorphism
- python 3 object oriented programming 
- https://tungnt.net/cac-nguyen-ly-cua-lap-trinh-huong-doi-tuong-object-oriented-programming/


