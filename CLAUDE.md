# vlncn-laocai-files

Kho lưu trữ tài liệu hành chính (GCN, GP VLNCN, TCTN, DVNM, iOffice) của Lào Cai.
Dữ liệu trong `uploads/` được trang web https://vlncn-laocai.vercel.app/ sử dụng qua đường dẫn
`https://raw.githubusercontent.com/Trangsct/vlncn-laocai-files/main/uploads/<tệp>` — tệp có hiệu lực ngay khi merge vào `main`.

**Không triển khai kho này lên Vercel** (`vercel.json`: `deploymentEnabled: false`, 05/11/2026): kho nặng 1,1 GB, mỗi commit
Vercel lưu một bản triển khai đầy đủ, khoảng 10 commit là hết 10 GB dung lượng miễn phí của nhóm trangscts-projects.

## Quy ước làm việc (bắt buộc)

- **Cuối MỖI phiên làm việc, luôn đồng bộ toàn bộ thay đổi lên GitHub và web:**
  1. Commit tất cả thay đổi trên nhánh làm việc và push lên origin.
  2. Tạo pull request vào `main` và merge (người dùng đã yêu cầu thường trực việc này
     — không cần hỏi lại), để trang web lấy được tệp mới qua raw.githubusercontent.com.
  3. Báo cáo lại cho người dùng những gì đã đồng bộ.

## Quy ước đặt tên file

- Tên file theo số hiệu văn bản thật bên trong tài liệu: `<số>_<ký hiệu>.pdf|docx`
  (ví dụ `1503_QĐ-SCT.pdf`, `07_KDTCTN_GP-HC.pdf`).
- Văn bản trùng số hiệu giữa các năm: thêm hậu tố năm, ví dụ `02_KDTCTN_GP-HC_2026.pdf`.
- File đính kèm/phụ lục của cùng văn bản: hậu tố `_2`, `_3`, ... Không lưu bản trùng
  lặp 100% nội dung (kiểm tra bằng MD5 trước khi thêm).
