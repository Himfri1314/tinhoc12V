<html lang="vi">
  <head>
    <meta charset = "UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  </head>
  <body>
     <!-- Banner -->
    <div class="banner">
        <h1 style="text-align:center;text-decorating: none; color: white; padding: 0 30px;">Bài 9: TẠO DANH SÁCH, BẢNG</h1>
    </div>
  </body>
    <style>
      body {
    margin: 0;
    font-family: 'Times New Roman';
    background-color: #f2f2f2;
}
      /* Banner nền ảnh */
.banner {
    width: 100%;
    height: 300px;
    background-image: url('xanh.jpg');
    background-size: cover;
    background-position: center;
    display: flex;
    justify-content: center;
    align-items: center;
}
.banner h1 {
    color: white;
    font-size: 40px;
    letter-spacing: 5px;
    font-weight: bold;
}
</style>
   <div id="wp-products">
    <h1 style="text-align:center;text-decorating: none; color: #243b9a; padding: 0 30px;">LUYỆN TẬP</h1>
  </div>
  <div style="background-color: #FFFFFF; padding: 10px;">
  		<h2>Sửa lại chương trình trong Hình 9.5a, sử dụng thuộc tính Style thay vì thuộc tính border để tạo viền cho bảng. Sử dụng màu xanh cho viền của ô hai dòng đầu bảng và sử dụng 3 màu đỏ, vàng, xanh cho ba chữ Toán, Vật lý và Hóa học.</h2> 
  </div>
  		<p>< table style="border: 3px solid"></p>
      <p>< tr> </p>
      <p>< th style="border:2px solid green" rowspan="2">Họ và tên< /th></p>
      <p>< th style="border:2px solid green" colspan="3"›Điểm thi< /th> </p>
      <p>< /tr></p>
      <p>< /tr></p>
      <p>< td style="border:2px solid black; color:red">Toán< /td></p>
      <p>< td style="border:2px solid black; color:yellow">Vật lí< /td></p>
      <p>< td style="border:2px solid black; color:blue">Hóa học< /td></p>
      <p>< /tr></p>
      <p>< /table></p>
        <div id="wp-products">
    <h1 style="text-align:center;text-decorating: none; color: #243b9a; padding: 0 30px;">VẬN DỤNG</h1>
  </div>
          <div style="background-color: #FFFFFF; padding: 10px;">
        <h2>Cho trước một bảng dữ liệu cỡ nx4, mỗi hàng tương ứng với một bộ (họ tên, điểm Toán, điểm Vật lý, điểm Hóa học) viết chương trình Python để tạo ra tệp HTML thực hiện việc vẽ bảng tương tự như Hình 9.5 và bổ sung dữ liệu vào các hàng phía dưới.</h2>
          </div>
      <p>data_input = [ [ ‘ Nguyen Van A ’ , 10, 9, 8 ] , [ ‘ Tran Van B ’ , 9, 9.5, 8.5 ] , [ ‘ Pham Thi C ’ , 9.5, 9.5, 9 ] ]</p>
      <p>output_file=open(“D:\TIN12-KNTT\B9-Vandung.html”,“w”,</p>
      <p>encoding=“utf-8”)</p>
      <p>content= “< table border-\ “1\”>\n”</p>
      <p>content+=”””< tr></p>
      <p>< th style= “border:1px solid green” rowspan= “2”>Họ và tên< /th></p>
      <p>< th style= “border:1px solid green” colspan= “3”>Điểm thi< /th></p>
      <p>< /tr></p>
      <p>< td style= “border:1px solid red”>Toán< /td></p>
      <p>< td style= “border:1px solid red”>Vật lí< /td></p>
      <p>< td style= “border:1px solid red”>Hoá học< /td></p>
      <p>< /tr></p>
      <p>” ” ”</p>
      <p>for dulieu in data_input:</p>
      <p>content+= “< tr>”</p>
      <p>for d in dulieu:</p>
      <p>content+=”””< td style= “border:1px solid red”>”””+str(d)+”””< /td>”””</p>
      <p>content+=”< /tr>\n”</p>
      <p>content+=”</ table>”</p>
      <p>output_file.write(content)</p>
      <p>output_file.close()</p>
