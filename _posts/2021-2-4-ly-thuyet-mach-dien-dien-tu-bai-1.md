---
layout: post
comments: true
title: "Lý thuyết mạch điện - điện tử bài 1: Thông số và phần tử cơ bản trong mạch điện"
title2: 
date: 2021-02-04 17:00:00
permalink: 2021/02/04/ly-thuyet-mach-dien-dien-tu-bai-1-thong-so-va-phan-tu-co-ban-trong-mach-dien/
mathjax: true
tags: Lý-thuyết-mạch
category: Điện
sc_project: 12473858
sc_security: 2277ef59
img: /assets/images/ly-thuyet-mach-1/nen-tang-ky-thuat-dien.jpg
summary: Giới thiệu về thông số mạch, phần tử cơ bản hay dùng trong các bài toán lý thuyết mạch điện - điện tử, giải tích mạch.
---
__Blog này mình viết cho 2 đối tượng chính:__
- Những bạn nhập môn.
- Những bạn đã có nền tảng vững.

_Đối với những bạn đã có nền tảng vững, nếu thấy những bài viết nào đó quá cơ bản hãy bỏ qua và nhảy thẳng vào những bài mà các bạn cho là phù hợp._

Mục lục:
<!-- MarkdownTOC -->
- [1. Giới thiệu](#-gioi-thieu)
- [2. Đối tượng nghiên cứu mạch điện](#-doi-tuong)
    - [2.1. Điện tích là gì?](#-dien-tich-la-gi)
    - [2.2. Dòng điện là gì?](#-dong-dien-la-gi)
    - [2.3. Điện áp là gì?](#-dien-ap-la-gi)
    - [2.4. Công suất là gì?](#-cong-suat-la-gi)
    - [2.4. Công suất tức thời](#-cong-suat-tuc-thoi)
- [3. Tài liệu tham khảo](#-tai-lieu-tham-khao)
<!-- /MarkdownTOC -->

<a name ="-gioi-thieu"></a>

## 1. Giới thiệu
Lý thuyết mạch là cơ sở của ngành kỹ thuật điện. Khi nghiên cứu về lý thuyết mạch ta có thể hiểu được các nhánh ứng dụng khác như hệ thống điện, máy điện, đo lường, điều khiển, điện tử viễn thông,... 

__Để học tốt các môn chuyên ngành, hãy học tốt lý thuyết mạch.__

Bức hình này là tổng quan về ngành điện:

<hr>
<div class = "imgcap">
    <img src ="/assets/images/ly-thuyet-mach-1/nen-tang-ky-thuat-dien.jpg" style="align:center">
    <div class="thecap">Hình 1: Tổng quan về ngành kỹ thuật điện.</div>
</div>
<hr>

<a name = "-doi-tuong"></a>

## 2. Đối tượng nghiên cứu mạch điện

<a name = "-dien-tich-la-gi"></a>

### 2.1. Điện tích là gì?
Rất khó cắt nghĩa điện tích. Các bạn hãy nhìn xuống hình bên dưới để xem mô hình hóa của một nguyên tử gồm: _Proton, Electron, Neutron_. Ta quy ước rằng các Electron mang điện tích âm(-), các Proton mang điện tích dương(+), và cuối cùng Neuton không mang điện. Các điện tích cùng dấu thì sẽ đẩy nhau, ngược lại các điện tích trái dấu thì sẽ hút nhau.

<hr>
<div class = "imgcap">
    <img src ="/assets/images/ly-thuyet-mach-1/cau-tao-co-ban-cua-nguyen-tu.png" style="align:center">
    <div class="thecap">Hình 2: Cấu tạo cơ bản của nguyên tử</div>
</div>
<hr>

<a name = "-dong-dien-la-gi"></a>

### 2.2. Dòng điện là gì?
Dòng điện là dòng chuyển dời có hướng của các hạt mang điện tích. Điện tích dương và âm luôn có xu hướng chuyển động ngược chiều nhau. Quy ước chiều của dòng điện là chiều chuyển dời của các hạt mang điện tích dương.

Định nghĩa chặt chẽ hơn về dòng điện biểu thị theo công thức:

<div style="text-align:center"> $$i = \frac{dq}{dt}$$ </div>
Đơn vị cường độ dòng điện là _Ampe_ - ký hiệu _A_
<hr>
<div class = "imgcap">
    <img src = "/assets/images/ly-thuyet-mach-1/mo-hinh-don-gian-dien-tich-chay-qua-nguyen-tu-tao-ra-dong-dien.gif" style = "align:center">
    <div class="thecap">Hình 3: Mô hình điện tích chạy qua nguyên tử tạo ra dòng điện</div>
</div>
<hr>
Mỗi một dòng điện chạy qua phần tử mạch nào đó, thì ta sẽ biểu thị bằng biểu tượng mũi tên. Mũi tên chỉ chiều chuyển động của các điện tích dương. Bên cạnh mũi tên thì dùng chữ ký hiệu _i_, hoặc một con số biểu thị giá trị của dòng điện.
<hr>
<div class = "imgcap">
    <img src = "/assets/images/ly-thuyet-mach-1/bieu-tuong-ky-hieu-dong-dien-trong-mach-dien.PNG" style = "align:center">
    <div class="thecap">Hình 4: Biểu tượng dòng điện được ký hiệu trong bản vẽ</div>
</div>
<hr>

Ta sẽ xét với 2 kiểu dòng điện chính:
<hr>
<div>
<table width = "100%" style = "border: 0px solid gray">
   <tr >
        <td width="40%" style = "border: 0px solid white"> 
        <img style="display:block;" width = "100%" src = "/assets/images/ly-thuyet-mach-1/dong-dien-mot-chieu-dc-current.png">
        <div class="thecap">Hình 5: Dòng điện một chiều - DC Current</div>
         </td>
        <td width="40%" style = "border: 0px solid white">
        <img style="display:block;" width = "100%" src = "/assets/images/ly-thuyet-mach-1/dong-dien-xoay-chieu-ac-current.png">
        <div class="thecap">Hình 6: Dòng điện xoay chiều - AC Current</div>
        </td>
    </tr>
    <tr>
        <td width="40%" style = "border: 0px solid white">
        <div style="text-align:left">Dòng điện một chiều là dòng điện không thay đổi về giá trị theo thời gian.</div>
        </td>
        <td width="40%" style = "border: 0px solid white">
        <div style="text-align:left">Dòng điện xoay chiều là dòng điện biến thiên theo quy luật hình sin.</div>
        </td>
    </tr>
</table> 
</div>
<hr>

<a name = "-dien-ap-la-gi"></a>

### 2.3. Điện áp là gì?
Điện áp là năng lượng để dịch chuyển điện tích từ xa vô cùng đến điểm mà ta đang xét, nhưng chúng ta sẽ không dùng định nghĩa này trong mạch điện. Để dễ dàng hình dung về điện áp hơn thì hãy tưởng tượng điện áp là chênh lệch về mức nước ở 2 điểm.

<hr>
<div class = "imgcap">
    <img src = "/assets/images/ly-thuyet-mach-1/dien-ap-la-gi.png" style = "align:center">
    <div class="thecap">Hình 7: Tưởng tượng điện áp là chênh lệch về mức nước ở 2 điểm.</div>
</div>
<hr>

Công thức định nghĩa về điện áp: 

<div style="text-align:center">$$u = \frac{dw}{dq}$$</div>

- w là năng lượng
- q là điện tích
- đơn vị điện áp là V - đọc là Vôn

Để biểu thị điện áp của một phần tử mạch nào đó ta vẽ một mũi tên song song với phần tử đang xét có chiều từ điện áp cao sang điện áp thấp và ký hiệu chữ cái _u_ (giống như có chiều từ mức nước cao sang mức nước thấp) bên cạnh mũi tên đó ta viết một giá trị, một con số biểu thị điện áp.

<hr>
<div class = "imgcap">
    <img src = "/assets/images/ly-thuyet-mach-1/bieu-tuong-ky-hieu-dien-ap-trong-mach-dien.PNG" style = "align:center">
    <div class="thecap">Hình 8: Điện áp được biểu diễn trong mạch điện.</div>
</div>
<hr>

Tương tự như dòng điện ta xét 2 kiểu điện áp chính 

<hr>
<div>
<table width = "100%" style = "border: 0px solid gray">
   <tr >
        <td width="40%" style = "border: 0px solid white"> 
        <img style="display:block;" width = "100%" src = "/assets/images/ly-thuyet-mach-1/dien-ap-mot-chieu-dc-voltage.png">
        <div class="thecap">Hình 8: Điện áp một chiều - DC Voltage</div>
         </td>
        <td width="40%" style = "border: 0px solid white">
        <img style="display:block;" width = "100%" src = "/assets/images/ly-thuyet-mach-1/dien-ap-xoay-chieu-ac-voltage.png">
        <div class="thecap">Hình 9: Điện áp xoay chiều - AC Voltage</div>
        </td>
    </tr>
    <tr>
        <td width="40%" style = "border: 0px solid white">
        <div style="text-align:left">Điện áp một chiều là điện áp không thay đổi về giá trị theo thời gian.</div>
        </td>
        <td width="40%" style = "border: 0px solid white">
        <div style="text-align:left">Điện áp xoay chiều là điện áp biến thiên theo quy luật hình sin.</div>
        </td>
    </tr>
</table> 
</div>
<hr>

<a name = "-cong-suat-la-gi">

### 2.4. Công suất là gì?
Công suất là lượng năng lượng của đối tượng, phần tử, mạch điện phát ra hoặc nhận về trong một giây đồng hồ. Công suất được ký hiệu là P

Công thức định nghĩa:

<div style = "text-align:center">$$p = \frac{dw}{dt}$$</div>

- w là năng lượng
- Thời gian t đang xét
- Đơn vị là Watt - ký hiệu W

<a name = "-cong-suat-tuc-thoi">

### 2.5. Công suất tức thời

Từ công thức tính công suất P ta nhân cả tử số và mẫu với với _dq_ không làm thay đổi phân số ban đầu.

<div style = "text-align:center">$$p = \frac{dw}{dq} . \frac{dq}{dt}$$</div>

Ta đã biết:

<div style = "text-align:center">$$u = \frac{dw}{dq} ; i = \frac{dq}{dt}$$</div>

Nên ta có công thức tính công suất tức thời thay đổi theo thời gian nếu như dòng và áp cũng thay đổi theo thời gian:

<div style = "text-align:center">$$p = ui$$</div>

__Kết luận__: Một vật chỉ phát hoặc thu năng lượng điện khi có cả dòng và áp, nếu thiếu một trong hai yếu tố này thì đối lượng đó không thể hoạt động được.

__Chiều của công suất__: 

<hr>
<div>
<table width = "100%" style = "border: 0px solid gray">
   <tr >
        <td width="40%" style = "border: 0px solid white"> 
        <img style="display:block;" width = "100%" src = "/assets/images/ly-thuyet-mach-1/dien-ap-dong-dien-cung-chieu-nhau.PNG">
        <div class="thecap">Hình 10: Điện áp và dòng điện cùng chiều nhau</div>
         </td>
        <td width="40%" style = "border: 0px solid white">
        <img style="display:block;" width = "100%" src = "/assets/images/ly-thuyet-mach-1/dien-ap-dong-dien-nguoc-chieu-nhau.PNG">
        <div class="thecap">Hình 11: Điện áp và dòng điện ngược chiều nhau</div>
        </td>
    </tr>
    <tr>
        <td width="40%" style = "border: 0px solid white">
        <div style="text-align:left">Công suất có giá trị dương nên mạch đang tiêu thụ công suất</div>
        </td>
        <td width="40%" style = "border: 0px solid white">
        <div style="text-align:left">Công suất có giá trị âm nên mạch đang phát công suất</div>
        </td>
    </tr>
</table> 
</div>
<hr>

<a name = "-tai-lieu-tham-khao">

## 3. Tài liệu tham khảo

[1] [Alternating Current (AC) vs. Direct Current (DC)](https://learn.sparkfun.com/tutorials/alternating-current-ac-vs-direct-current-dc/)

[2] [What is Electricity?](https://learn.sparkfun.com/tutorials/what-is-electricity)

[3] [Bài giảng lý thuyết mạch thầy Nguyễn Công Phương - Đại học Bách Khoa Hà Nội](https://sites.google.com/site/ncpdhbkhn/bai-giang/ly-thuyet-mach)