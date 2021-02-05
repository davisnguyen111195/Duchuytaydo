---
layout: post
comments: true
title: "Lý thuyết mạch điện - điện tử bài 1: Thông số và phần tử cơ bản trong mạch điện"
title2: 
date: 2021-02-04 17:00:00
permalink: 2021/02/04/ly-thuyet-mach-dien-dien-tu-bai-1-thong-so-va-phan-tu-co-ban-trong-mach-dien/
mathjax: true
tags: Lý-thuyết-mạch Điện Điện-tử Giải-tích-mạch
category: Điện
sc_project: 12473858
sc_security: 2277ef59
img: /assets/images/ly-thuyet-mach-1/nen-tang-ky-thuat-dien.jpg
summary: Giới thiệu về thông số mạch, phần tử cơ bản hay dùng trong các bài toán lý thuyết mạch điện - điện tử, giải tích mạch.
---

Mục lục:
<!-- MarkdownTOC -->
- [1. Giới thiệu](#-gioi-thieu)
- [2. Đối tượng nghiên cứu mạch điện](#-doi-tuong)
    - [2.1. Điện tích](#-dien-tich)
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

<a name = "-dien-tich"></a>

### 2.1 Điện tích
Vậy điện tích là gì? Rất khó cắt nghĩa điện tích. Các bạn hãy nhìn xuống hình bên dưới để xem mô hình hóa của một nguyên tử gồm: Proton, Electron, Neutron. Ta quy ước rằng các Electron mang điện tích âm(-), các Proton mang điện tích dương(+), và cuối cùng Neuton không mang điện. Các điện tích cùng dấu thì sẽ đẩy nhau, ngược lại các điện tích trái dấu thì sẽ hút nhau.

<hr>
<div class = "imgcap">
    <img src ="/assets/images/ly-thuyet-mach-1/cau-tao-co-ban-cua-nguyen-tu.png" style="align:center">
    <div class="thecap">Hình 2: Cấu tạo cơ bản của nguyên tử</div>
</div>
<hr>

<a name = "-dong-dien"></a>

### 2.2 Dòng điện
Dòng điện là dòng chuyển dời có hướng của các hạt mang điện tích. Điện tích dương và âm luôn có xu hướng chuyển động ngược chiều nhau. Quy ước chiều của dòng điện là chiều của các hạt mang điện tích dương.

Định nghĩa chặt chẽ hơn về dòng điện biểu thị theo công thức:

<div style="text-align:center"> $$i = \frac{dq}{dt}$$ </div>
