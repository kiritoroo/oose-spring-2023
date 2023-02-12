# Chapter 4 - An Overview of the UML

> Đối với UML cung cấp rất nhiều các biểu đồ khác nhau. Nó có thể giúp ta có thể nhìn nhận hệ thống qua nhiều góc nhìn khác nhau.

Một quá trình phát triển phần mềm sẽ có nhiều bên liên quan tham gia vào dự án, ví dụ như là:

* Analysts
* Designers
* Coders
* Testers
* QA
* The customer
* Technical Authors

Tất cả những người này đều quan tâm đến các khía cạnh khác nhau của hệ thống và mỗi người trong số họ sẽ yêu cầu mức độ chi tiết khác nhau.

## 1. The Use Case Diagram
> Biểu đổ Use Case là một sự mô tả hành vi của hệ thống dưới góc nhìn của người dùng. Biểu đồ này giúp ích rất nhiều cho Analysis vì nó giúp ta có thể hiểu được các yêu cầu của hệ thống đó.
<figure>
  <img src="../img/img_01.JPG" width="512">
  <figcaption>The Use Case Diagram</figcaption>
</figure>

## 2. The Class Diagram
> Biểu đồ Lớp mô tả kiểu của các đối tượng trong hệ thống và các quan hệ(relationship) khác nhau tồn tại giữa chúng. Đây là biểu đồ hay dùng nhất trong UML và gần gũi với các lập trình viên. Nó giúp trao đổi thông tin và hiểu rõ ý tưởng của nhau dễ dàng hơn.
<figure>
  <img src="../img/img_02.JPG" width="512">
  <figcaption>The Class Diagram</figcaption>
</figure>

## 3. The Collaboration Diagrams
> Biểu đồ cộng tác là một minh họa về các mối quan hệ và tương tác giữa các đối tượng phần mềm trong UML. Thay vì hiểu thị luồng thông báo, nó mô tả kiến trúc của đối tượng có trong hệ thống vì nó dựa trên lập trình Hướng đối tượng. Một đối tượng bao gồm một số tính năng. Nhiều dối tượng hiện diện trong hệ thống được kết nối với nhau.
Biểu đồ cộng tác, còn được gọi là biểu đồ giao tiếp, được sử dụng để mô tả kiến trúc của đối tượng trong hệ thống.
<figure>
  <img src="../img/img_03.JPG" width="512">
  <figcaption>The Collaboration Diagram</figcaption>
</figure>

## 4. The Sequence Diagram
> Biểu đồ tuần tự (Sequence Diagram) mô tả luồng hoạt động một số chức năng quan trọng / phức tạp. Ví dụ: chức năng thanh toán, chức năng booking.

<figure>
  <img src="../img/img_04.JPG" width="512">
  <figcaption>The Sequence Diagram</figcaption>
</figure>

Là biểu đồ dùng để xác định các trình tự diễn ra sự kiện của một nhóm đối tượng nào đó. Nó miêu tả chi tiết các thông điệp được gửi và nhận giữa các đối tượng đồng thời cũng chú trọng đến việc trình tự về mặt thời gian gửi và nhận thông điệp đó.

Với những chức năng phức tạp, với các workflow chồng chéo, việc xây dựng tài liệu Sequency Diagram là rất cần thiết và còn giúp các thành viên tưởng tượng rõ hơn về quy trình vận hành, workflow của các chức năng.
    
## 5. The State Diagrams
>Biểu đồ trạng thái là dạng biểu đồ mô tả các trạng thái có thể có và sự chuyển đổi giữa các trạng thái đó khi có các sự kiện tác động của một đối tượng.
Đối với các đối tượng có nhiều trạng thái thì biểu đồ trạng thái là sự lựa chọn tốt nhất giúp chúng ta có thể hiểu rõ hơn về hệ thống.

<figure>
  <img src="../img/img_05.jpg" width="512">
  <figcaption>The State Diagrams</figcaption>
</figure>

Biểu đồ trạng thái thể hiện những khía cạnh mà ta quan tâm tới khi xem xét trạng thái của một đối tượng:

* Trạng thái ban đầu
* Một số trạng thái ở giữa
* Một hoặc nhiều trạng thái kết thúc
* Sự biến đổi giữa các trạng thái
* Những sự kiện gây nên sự biến đổi từ một trạng thái này sang trạng thái khác

## 6. The Package Diagrams
<figure>
  <img src="../img/img_06.jpg" width="512">
  <figcaption>The Package Diagrams</figcaption>
</figure>

> Package Diagrams được sử dụng để phản ánh tổ chức của packages (các gói) và các elements của chúng.

<figure>
  <img src="../img/img_07.jpg" width="512">
  <figcaption>The Package Diagrams Detail</figcaption>
</figure>

## 7. The Component Diagrams
> Biểu đồ thành phần là biểu đồ mô tả các thành phần và sự phụ thuộc của chúng trong hệ thống.

Các thành phần của hệ thống có thể là:

*	**Thành phần mã nguồn** – có ý nghĩa vào thời điểm dịch chương trình. Thông thường nó là tập các chương trình cài đặt lớp.
*	**Thành phần mã nhị phân** - là mã trình nhị phân được dịch từ mã chương trình nguồn.
Nó có thể là tệp mã đích (.obj), tệp thư viện tĩnh (.lib) hay tệp thư viện động (.dll).
Thành phần nhị phân được sử dụng để liên kết, hoặc để thực thi chương trình (đối với thư viện động)
*	**Thành phần thực thi** – là tệp chương trình có thể thực thi được (các tệp .exe). Nó là kết quả của chương trình liên kết các thành phần nhị phân
<figure>
  <img src="../img/img_08.jpg" width="512">
  <figcaption>The Component Diagrams</figcaption>
</figure>

## 8. The Deployment Diagrams
> Biểu đồ triển khai là một loại biểu đồ thể hiện kiến trúc thực thi của hệ thống, bao gồm các nút như môi trường thực thi phần cứng hoặc phần mềm và phần mềm trung gian kết nối chúng.
Biểu đồ triển khai giúp chúng ta xác định sẽ triển khai hệ thống phần mềm(Component) lên hệ thống ra sao.

<figure>
  <img src="../img/img_09.jpg" width="512">
  <figcaption>The Deployment Diagrams</figcaption>
</figure>

Biểu đồ triển khai thường được sử dụng để hình dung phần cứng và phần mềm vật lý của hệ thống
Thể hiện rõ kiến trúc triển khai nên nó sẽ ảnh hưởng đến sự thiết kế, phát triển, hiệu năng, khả năng mở rộng của hệ thống…
