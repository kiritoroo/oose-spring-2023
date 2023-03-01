# Chapter 8 - Conceptual Modelling
Mô hình khái niệm (đôi khi còn được gọi là Mô hình hóa miền) là hoạt động tìm ra khái niệm nào là quan trọng đối với hệ thống của chúng ta.

Mô hình khái niệm cũng là một tập hợp các khái niệm. Một số mô hình là các đối tượng vật lý; ví dụ, một mô hình đồ chơi có thể được lắp ráp và có thể được chế tạo để hoạt động giống như đối tượng mà nó làm đại diện.

UML không cho chúng ta biết cách thức hoặc thời điểm thực hiện Mô hình khái niệm, nhưng nó cung cấp cho chúng ta cú pháp để thể hiện mô hình.

> Mô hình mà chúng ta sẽ sử dụng là **Sơ đồ lớp**.

<figure>
  <img src="../img/img_01.jpg" width="512">
  <figcaption>The Class Diagram</figcaption>
</figure>

Phát triển Sơ đồ lớp là chìa khóa cho bất kỳ quy trình thiết kế đối tượng nào. Sơ đồ lớp về cơ bản sẽ cung cấp cấu trúc của mã cuối cùng mà chúng ta tạo ra.

> Tuy nhiên ở giai đoạn này, chúng ta chưa quan tâm đến thiết kế hệ thống (vẫn đang phân tích), vì vậy Sơ đồ lớp chúng ta tạo ra ở giai đoạn này sẽ khá sơ sài và sẽ không chứa bất kỳ quyết định thiết kế nào.
Ví dụ: Chúng ta không muốn thêm một lớp Linklist vào giai đoạn này, vì điều đó bắt buộc chúng ta phải thực hiện một giải pháp cụ thể quá sớm.

Về cơ bản chúng ta đang tạo ra *Sơ đồ lớp phân tích*. Nhiều người thích phân biệt hoàn toàn giữa **Sơ đồ lớp phân tích** và **Sơ đồ lớp thiết kế** bằng cách gọi **Sơ đồ lớp phân tích** là **Mô hình khái niệm**. Một số ví dụ như:

* Thang máy trong hệ thống điều khiển thang máy
* Đặt hàng trong hệ thống mua sắm tại nhà
* Cầu thủ bóng đá trong hệ thống chuyển nhượng bóng đá (hoặc trò chơi bóng đá Playstation!)
* Huấn luyện viên hệ thống quản lý kho cho cửa hàng giày dép
* Phòng trong hệ thống đặt phòng

Một số ví dụ sai như: 

-	**OrderPurgeDaemon** quy trình thường xuyên “xóa” các đơn hàng cũ ra khỏi hệ thống
-	**EventTrigger** quy trình đặc biệt đợi trong 5 phút rồi yêu cầu hệ thống thức dậy và làm điều gì đó
-	**CustomerDetailsForm** cửa sổ yêu cầu thông tin chi tiết về khách hàng mới trong hệ thống mua sắm
-	**DbArchiveTable** bảng cơ sở dữ liệu chứa danh sách tất cả các  đơn đặt hàng cũ
> Đây là những khái niệm không ổn, bởi vì chúng ta đang tập trung vào thiết kế giải pháp chứ không phải vấn đề.

> “Rule of thumb” – quy tắc ngón tay cái
(Chỉ các nguyên tắc không hướng đến sự chính xác hoặc đáng tin cậy trong mọi tình huống, nhưng có ứng dụng rộng rãi. Nguyên tắc ngón tay cái đề cập đến một quy trình hoặc tiêu chuẩn dễ học và dễ áp dụng, dựa trên kinh nghiệm thực tế hơn là lý thuyết.)

**Mô hình khái niệm** sẽ dần chuyển đổi thành một **Sơ đồ lớp thiết kế** khi chúng ta chuyển qua giai đoạn xây dựng.

## FINDING CONCEPTS
Cách tốt nhất để tìm Use Case là tổ chức một buổi Workshop với càng nhiều bên liên quan quan tâm càng tốt.

Brainstorming gợi ý cho các khái niệm, nắm bắt tất cả các gợi ý.

Sau khi **Brainstorming** xong, làm việc theo nhóm để thảo luận và biện minh cho từng đề xuất.

Áp dụng quy tắc ngón tay cái (khách hàng phải hiểu khái niệm và loại bỏ những thứ không liên quan, những thứ không chạm đến thiết kế)

### EXTRACTING CONCEPTS FROM REQUIREMENTS
Tìm hiểu các khái niệm sau:

-	Đối tượng vật lý hoặc hữu hình
-	Địa điểm
-	Transactions
-	Vai trò của mọi người (Ví dụ: Khách hàng, Nhân viên bán hàng)
-	Containers for other Concepts
-	Các hệ thống khác bên ngoài hệ thống (Ví dụ: Cơ sở dữ liệu từ xa)
-	Danh từ trừ tượng
-	Tổ chức
-	Sự kiện
-	Nội quy / Chính sách
-	Hồ sơ / Nhật ký

Một số điểm lưu ý:

- Việc thu nhập các khái niệm một cách máy móc là việc làm kém hiệu quả. Bạn phải có nguồn tài liệu đầu vào từ khách hàng.
- Nhiều người đề nghị trích xuất các cụm danh từ từ các tài liệu.

**Thông tin đầu vào từ khách hàng là điều cần thiết!**

## THE CONCEPTUAL MODEL IN THE UML
Chúng ta sẽ trình bày khái niệm của mình trong một box đơn giản, với tiêu đề của khái niệm (theo quy ước, viết hoa) ở trên cùng của box.

<figure>
  <img src="../img/img_02.jpg" width="200">
</figure>
Bên trong Box lớn là hai Box nhỏ hơn, để trống.

Box ở giữa sẽ sớm được sử dụng để nắm bắt các thuộc tính của khái niệm.

Box dưới cùng được sử dụng để nắm bắt hành vi của khái niệm, hay nói cách khác, khái niệm này thực sự có thể làm gì đó (nếu có).

Ví dụ: Chúng ta đã quyết định rằng mọi người chạy đua sẽ có 2 thuộc tính Name và Age.

Box cuối để trống cho đến khi chúng ta quyết định được những gì mà người chạy đua có thể làm.
<figure>
  <img src="../img/img_03.JPG" width="650">
</figure>

## FINDING ATTRIBUTES

> Chúng ta cần xác định các thuộc tính của từng khái niệm. Và sẽ sử dụng phương pháp Brainstorming cho bước này.

Ví dụ: Giả sử chúng ta đang làm việc trên hệ thống Staff Manager. Chúng ta đã xác định “Manager”. Gợi ý cho một thuộc tính có thể là “Salary” như sau:
<figure>
  <img src="../img/img_04.JPG" width="650">
</figure>

Nhưng vấn đề ở đây là: Liệu “Salary” cũng sẽ là một khái niệm riêng biệt. Vì vậy, chúng ta có nên biến nó từ một thuộc tính thành một khái niệm không ?
Nếu bạn nghi ngờ về điều đó: Hãy biến nó thành một khái niệm khác

<figure>
  <img src="../img/img_05.jpg" width="650">
</figure>

## GUIDELINES FOR FINDING ATTRIBUTES
> Các quy tắc ngón tay cái sau đây có thể hữu ích khi quyết định giữa thuộc tính và khái niệm. Đừng quá lo lắng, nếu nghi ngờ hãy biến nó thành một khái niệm riêng.

-	Các chuỗi đơn giá trị hoặc số có giá trị đơn lẻ thường là Thuộc tính.
-	Nếu một thuộc tính của một khái niệm không có khả năng làm bất cứ điều gì, nó có thể là một thuộc tính.

## ASSOCIATION (SỰ LIÊN KẾT)
> Bước tiếp theo là quyết định các khái niệm của chúng ta có liên quan với nhau như thế nào. Trong bất kỳ hệ thống nào, ít nhất một số khái niệm sẽ có một số loại quan hệ khái niệm với các khái niệm khác.
<figure>
  <img src="../img/img_07.jpg" width="650">
</figure>

Ví dụ: Hai khái niệm này có liên quan với nhau, bởi vì trong công ty chúng ta đang phát triển một hệ thống:

Mỗi “Manager” sẽ lái một “Car” của công ty

Chúng ta có thể biểu thị mối quan hệ này trong UML bằng cách kết nối 2 khái niệm với nhau bằng một dòng duy nhất (được gọi là Association)

<figure>
  <img src="../img/img_06.jpg" width="650">
</figure>

-	Sự liên kết có một tên trong mô tả trường hợp này: Drives
-	Có những con số ở mỗi đầu của sự liên kết. Tượng trưng cho mối quan hệ ở trường hợp này là 1 Manager sẽ lái 1 Car và ngược lại.


Ví dụ: Ta thấy mỗi “Manager” quản lý từ 1 “Staff Member” trở lên; và (đi theo một cách khác) mỗi “Staff Member” được quản lý bởi 1 “Manager”.
<figure>
  <img src="../img/img_08.jpg" width="650">
</figure>

## POSSIBLE CARDINALITES 

> *Cardinality* có nghĩa là số lượng của một cái gì đó nhưng nó được sử dụng trong nhiều ngữ cảnh khác nhau. 
Định nghĩa: Chúng ta có các bảng trong cơ sở dữ liệu. Trong cơ sở dữ liệu quan hệ, chúng ta có quan hệ giữa các bảng. Các quan hệ này có thể là một-một, một-nhiều hoặc nhiều-nhiều. Những mối quan hệ này được gọi là ***cardinality***.

<figure>
  <img src="../img/img_10.jpg" width="650">
</figure>

Trong ngữ cảnh của cơ sở dữ liệu, cardinality đề cập đến tính duy nhất của các giá trị dữ liệu có trong một cột. Cardinality cao có nghĩa là cột chứa một tỷ lệ lớn các giá trị hoàn toàn duy nhất. Cardinality thấp có nghĩa là cột chứa rất nhiều "lặp lại" trong phạm vi dữ liệu của nó.

Về cơ bản, không có giới hạn nào đối với các Cardinalities mà bạn có thể chỉ định. Sơ đồ sau đây liệt kê một số ví dụ, mặc dù danh sách này không có nghĩa là đầy đủ.

<figure>
  <img src="../img/img_11.jpg" width="512">
</figure>

> Kí hiệu * biểu thị “nhiều”
Lưu ý: Sự khác biệt giữa * và 1…*
“*”: nhiều nhưng không rõ ràng, có nghĩa là bất kỳ số lượng khái niệm nào cũng được cho phép hoặc có thể chúng ta sẽ đưa ra quyết định.
“1…*”: rõ ràng hơn, ngụ ý rằng một hoặc nhiều sẽ được cho phép

<figure>
  <img src="../img/img_09.jpg" width="512">
</figure>

## BUILDING THE COMPLETE MODEL 
Chúng ta hãy xem xét một hệ thống phương pháp để xác định mối liên hệ giữa các khái niệm.

Giả sử, chúng ta hoàn thành bước Brainstorming và phát hiện ra một số khái niệm cho hệ thống “Staff Manager”

<figure>
  <img src="../img/img_12.jpg" width="512">
  <figcaption>Tập hợp các khái niệm về “Staff Manager”</figcaption>
</figure>

> Cách tốt nhất để sửa chữa một khái niệm, chẳng hạn như “Manager” và xem xét lần lượt những khái niệm khác. 
Liệu những khái niệm này có liên quan gì với nhau không? Và nếu có hãy quyết định ngay tên liên kết và tính chính xác của nó

1.	“Manager” và “Staff” có liên quan với nhau không? – Có, mỗi “Manager” quản lý 1 hoặc nhiều “Staff”

2.	“Manager” và “Pension”
“Manager” và “Company Car”
      → Mỗi “Manager” đóng góp vào 1 khoản “Pension”
      → Mỗi “Manager” lái 1 ô tô của công ty

Và cứ như vậy cho đến khi hoàn thành mô hình.

Một sai lầm phổ biến ở giai đoạn này là quyết định hai khái niệm có liên quan với nhau sau đó vẽ 1 đường thẳng trên biểu đồ và bỏ qua tên liên kết đó. Và sau này khi cần bạn sẽ không biết ý nghĩa của nó là gì và phải bắt đầu lại từ đầu!

<figure>
  <img src="../img/img_13.jpg" width="512">
  <figcaption>Mô hình khái niệm đơn giản, đã hoàn thành</figcaption>
</figure>

***Lưu ý:***

> Khi xây dựng mô hình, điều quan trọng cần nhớ là Các liên kết không quan trọng bằng các Thuộc tính

> Mọi liên kết bị thiếu sẽ dễ dàng được chọn trong quá trình thiết kế, nhưng sẽ khó phát hiện ra các thuộc tính bị thiếu.

> Một nguyên tắc nhỏ là tập trung vào các khái niệm và thuộc tính, đồng thời cố gắng khắc phục những liên kết rõ ràng nhất.























