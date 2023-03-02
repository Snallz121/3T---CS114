<p align="center">
   <a href="https://www.uit.edu.vn/">
      <img src="https://i.imgur.com/WmMnSRt.png" border="none">
   </a>
</p>
<h1 align="center">
    CS114.N11.KHCL - Machine Learning
</h1>

<h2>
   Giới thiệu môn học   
</h2>

- **Tên môn học:** Machine Learning
- **Mã môn học:** CS114
- **Mã lớp:** CS114.N11.KHCL
- **Năm học:** HK1 (2022-2023)
- **Giảng viên:** 

<h2>
   Giới thiệu nhóm
</h2>

- **Thông tin thành viên** 

<table align="center">
      <tr>
       <th>Họ và Tên</th>
       <th>MSSV</th>
       <th>Github</th>
       <th>Email</th>
      </tr>
      <tr>
       <td>Nguyễn Minh Thuận</td>
       <td>20520795</td>
       <td> https://github.com/ThuanE3691</td>
       <td>20520795@gm.uit.edu.vn</td>  
      </tr>
      <tr>
       <td>Tống Phúc Thịnh</td>
       <td>20520785</td>
       <td> https://github.com/Snallz121</td>
       <td>20520785@gm.uit.edu.vn</td>  
      </tr>
      <tr>
       <td>Trương Thị Thanh Thanh</td>
       <td>20520767</td>
       <td>https://github.com/TTTThanh2812</td>
       <td>20520767@gm.uit.edu.vn</td>  
      </tr>
</table>


<h2>
  Chủ đề báo cáo 
</h2>

- **Tên đồ án:** Phân loại trái cây tươi và trái cây hư
- **Thư mục lưu trữ:** [Project](Project)

<h3>
  Mô tả đồ án
</h3>

<h3>
  1. Mô tả bài toán
</h3>

**Ngữ cảnh ứng dụng**: 

<p align="justify"> 
   Trong thời đại công nghệ 4.0, tự động hóa sử dụng machine learning là một việc thường thấy trong thực tế và xuất hiện ở trong mọi lĩnh vực như nông nghiệp, công nghiệp,.... Đặc biệt là trong nông nghiệp thì machine learning đã xuất hiện rất nhiều bài toán khó cần giải quyết để đáp ứng nhu cầu tự động hóa trong nông nghiệp như phân loại giống, phân loại hoa quả,...
</p>

Bài toán phân loại trái cây tươi hay hư ra đời vì trái cây nếu không được bảo quản đúng cách thì sẽ rất dễ bị hư, vì thế để đảm bảo chất lượng của trái cây và sức khỏe của người ăn thì bài toán rất cấp thiết.  

Bài toán được ứng dụng rất nhiều như phân loại các trái cây sau khi phân loại ở trạng thái nào để có thể mang ra ngoài tiêu thụ, hay ở trong các siêu thị khi nhập hàng lượng lớn các loại trái cây thì sẽ có khả năng xuất hiện trái cây hư, vì thế bài toán này sẽ giải quyết việc phân loại trái cây tươi hoặc hư để mang đến cho an toàn cho sức khỏe của người dùng khi dùng cái loại thực phẩm nhanh hư như trái cây. 

   
**Input**: 
+ Một tấm ảnh màu có định dạng đuôi ảnh là định dạng .jpg

+ Ảnh được chụp từ camera của điện thoại hoặc máy ảnh 

+ Ảnh chỉ có duy nhất 1 loại quả nhưng không giới hạn số lượng của loại quả đó trong tấm ảnh.

**Output**:

Dự đoán tên của loại quả trong ảnh và trạng thái “Fresh”(tươi) hoặc “Rotten”(hư) của loại quả ấy. Kết quả đầu ra sẽ có dạng như sau “Trạng thái của quả”“Tên quả” trong tiếng anh.

Ví dụ output: "FreshApple", "RottenBanana"
<h3>
  2. Mô tả bộ dữ liệu
</h3>

Tên bộ dữ liệu: Fresh and Rotten Fruits Dataset for Machine-Based Evaluation of Fruit Quality

Nguồn bộ dữ liệu: 

+ Được lấy từ web Mendeley Data được đăng tải vào ngày 8 tháng 4 năm 2022 bởi nhóm tác giả Nusrat Sultana, Musfika Jahan, Mohammad Shorif Uddin thuộc Jahangirnagar University.

+ Web Mendeley Data là một nền tảng lưu trữ và chia sẽ dữ liệu khoa học, trực tuyến được phát triển Elsevier, nó cung cấp cho các nhà nghiên cứu và tổ chức khoa họa một cách để quản lý, lưu trữ dữ liệu một cách dễ dàng và đáng tin cậy

**Cách thức xây dựng bộ dữ liệu**:

Ảnh được nhóm tác giả chụp bằng máy ảnh (Nikon D5600) ở các sạp trái cây ở Bangladesh với điều kiện khi chụp ảnh là ánh sáng, góc chụp, các điều kiện khác mà không được thiết lập theo bất kì điều kiện gì.

**Số lượng, độ đa dạng**: 
- Tổng cộng 3200 tấm ảnh
- Chia thành 16 thư mục
- Mỗi thư mục đại diện cho một nhãn của bộ dữ liệu
- Mỗi thư mục chứa 200 tấm ảnh

- Các nhãn của bộ dataset:
+ Táo tươi (Fresh Apple)
+ Chuối tươi (Fresh Banana)
+ Nho tươi (Fresh Grape)
+ Ổi tươi (Fresh Guava)
+ Táo tàu tươi (Fresh Jujube)
+ Cam tươi (Fresh Orange)
+ Lựu tươi (Fresh Pomegranate)
+ Dâu tươi (Fresh Strawberry)
+ Táo hư (Rotten Apple), 
+ Chuối hư (Rotten Banana)
+ Nho hư (Rotten Grape)
+ Ổi hư (Rotten Guava)
+ Táo tàu hư (Rotten Jujube)
+ Cam hư (Rotten Orange)
+ Lựu hư (Rotten Pomegranate)
+ Dâu hư (Rotten Strawberry) 

**Thao tác tiền xử lí**

**Phân chia dữ liệu**
- 80% dùng để train
- 20% dùng để test




