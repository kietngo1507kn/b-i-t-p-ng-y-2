### BÀI 1

[](https://github.com/kietngo.1507kn-ops/CNTT1_Nhap-mon-CNTT_OnTap-Ngay2/blob/d21ebf4d55b9fa0a7557d5e8c5e4142ec137fb31/starter-kit/bai_lam_ngay2.md#b%C3%A0i-1)

`select-string "ERROR" logs/access.log > logs/error_report.txt`

### BÀI 2

[](https://github.com/kietngo.1507kn-ops/CNTT1_Nhap-mon-CNTT_OnTap-Ngay2/blob/d21ebf4d55b9fa0a7557d5e8c5e4142ec137fb31/starter-kit/bai_lam_ngay2.md#b%C3%A0i-2)

**1. Lệnh đếm số dòng chứa WARNING trong logs/access.log bằng pipeline (dấu |)**.

PS D:\Ôn_thi_giữa-kì\starter-kit\trung-tam-tieng-anh> select-string "WARNING" logs/access.log | Measure-Object Count : 4 Average : Sum : Maximum : Minimum : Property :  **2.Đếm số dòng chứa ERROR trong logs/payment.log bằng pipeline**  PS D:\Ôn_thi_giữa-kì\starter-kit\trung-tam-tieng-anh> Select-string "ERROR" logs/payment.log | Measure-Object

Count : 3 Average : Sum : Maximum : Minimum : Property :

### BÀI 3

[](https://github.com/kietngo.1507kn-ops/CNTT1_Nhap-mon-CNTT_OnTap-Ngay2/blob/d21ebf4d55b9fa0a7557d5e8c5e4142ec137fb31/starter-kit/bai_lam_ngay2.md#b%C3%A0i-3)

logs\payment.log:4:2025-10-18 09:19:13 [WARNING] Cong thanh toan phan hoi cham logs\payment.log:7:2025-10-18 09:28:16 [WARNING] Nhieu lan nhap sai ma OTP logs\payment.log:12:2025-10-18 09:43:01 [WARNING] So du vi gan bang hoc phi logs\payment.log:13:2025-10-18 09:46:22 [WARNING] So du vi gan bang hoc phi logs\payment.log:14:2025-10-18 09:49:43 [WARNING] So du vi gan bang hoc phi

### BÀI 4 ( Ở trong file )

[](https://github.com/kietngo.1507kn-ops/CNTT1_Nhap-mon-CNTT_OnTap-Ngay2/blob/d21ebf4d55b9fa0a7557d5e8c5e4142ec137fb31/starter-kit/bai_lam_ngay2.md#b%C3%A0i-4--%E1%BB%9F-trong-file-)

### BÀI 5 Câu trả lời của em là:

[](https://github.com/kietngo.1507kn-ops/CNTT1_Nhap-mon-CNTT_OnTap-Ngay2/blob/d21ebf4d55b9fa0a7557d5e8c5e4142ec137fb31/starter-kit/bai_lam_ngay2.md#b%C3%A0i-5-c%C3%A2u-tr%E1%BA%A3-l%E1%BB%9Di-c%E1%BB%A7a-em-l%C3%A0)

**a). lệnh > khác >> là**

-   lệnh > thường dùng để ghi đè lên file ví dụ một file hoc_sinh.txt, thêm văn bản PhamQuocDat vào dùng > lập tức toàn bộ file hoc_sinh.txt thay hoàn toàn thành chỉ còn nguyên dòng PhamQuocDat. lệnh >> thường dùng để ghi thêm lên file ví dụ một file hoc_sinh.txt, thêm văn bản PhamQuocDat vào dùng >> lập tức file hoc_sinh.txt giữ nguyên và thêm dòng PhamQuocDat.

**b)Ở Bài 4, nếu lệnh thứ hai (nối các dòng ERROR) dùng > thay cho >>, nội dung file tong_hop_ngay2.txt sẽ thay đổi ra sao?**

-   Thì nội dung file tổng hợp ngày đó sẽ biết mấy hoàn toàn và thay cho văn bài mới thêm vào.

**c) Vì sao trong script nên dùng đường dẫn tương đối logs/payment.log thay vì đường dẫn tuyệt đối trên máy mình (ví dụ C:/Users/An/Desktop/...)?**

-   Vì đường dẫn tương đối đảm bảo tính linh hoạt và chạy được trên nhiều môi trường khác nhau nếu dùng đường dẫn tuyệt đối dễ lỗi khi chạy trên máy khác không tìm thấy đường dẫn file.
