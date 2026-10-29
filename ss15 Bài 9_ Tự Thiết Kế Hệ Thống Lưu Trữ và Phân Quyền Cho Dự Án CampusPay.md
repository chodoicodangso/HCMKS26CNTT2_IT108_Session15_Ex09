I. Cấu Trúc Thư Mục (Google Drive)  
\[Dự án\] CampusPay/ (Thư mục gốc)  
1\. KyThuat/ (Mã nguồn, API, config)  
2\. ThietKe/ (Figma files, tài sản UI/UX)  
3\. KinhDoanh/ (Business Plan, số liệu tài chính)  
4\. Chung\_Pitch/ (Slide Pitch, tài liệu giới thiệu ngoài)  
II. Ma Trận Phân Quyền (Access Control Matrix)

| Loại tài liệu | Ban Kỹ thuật | Ban Thiết kế | Ban Kinh doanh | Nhà đầu tư |
| :---- | :---- | :---- | :---- | :---- |
| Mã nguồn & API | Editor | No Access | No Access | No Access |
| Tài sản UI/UX | Viewer | Editor | Viewer | No Access |
| Business Plan | Commenter | No Access | Editor | Viewer |
| Slide Pitch | Viewer | Viewer | Editor | Viewer\* |

III. Phương Án Xử Lý Rủi Ro (Edge Cases)  
Nhu cầu xem chéo phòng ban: Áp dụng quyền Commenter/Viewer để nắm nghiệp vụ mà không làm sai lệch số liệu gốc của ban khác.  
Bảo vệ chất xám với đối tác ngoài: Giới hạn quyền Viewer cấp qua email đích danh, kết hợp chặn tải/copy file.Cấm sử dụng Link Public.  
Quy trình Offboarding: Revoke quyền truy cập email của nhân sự đó tại cấp thư mục gốc CampusPay ngay lập tức, kết hợp reset các khóa API