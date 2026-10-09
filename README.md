# Báo cáo Thực hành Kiểm thử API với Postman

## 1. Thông tin sinh viên
- **Họ và tên:** [Trần Thiên Đạt]
- **Mã sinh viên:** [23010128]

## 2. Quá trình thực hành
Trong bài tập này, em đã thực hành gửi các HTTP Request và viết các kịch bản kiểm thử tự động cơ bản bằng công cụ Postman.

### 2.1. Gửi HTTP GET Request
- **API sử dụng:** `[Ví dụ: https://random-data-api.com/api/v2/users]`
- **Mô tả:** Lấy thông tin ngẫu nhiên của một người dùng.
- **Kết quả minh họa:**
> *(Kéo thả ảnh chụp màn hình Postman hiển thị trạng thái 200 OK và phần thân Body định dạng JSON vào đây)*

### 2.2. Gửi Request với tham số (Query Parameters)
- **API sử dụng:** `[Đường link API của bạn]`
- **Mô tả:** Sử dụng tab Params để truyền tham số lọc dữ liệu.
- **Kết quả minh họa:**
> *(Kéo thả ảnh chụp phần Query Params và kết quả tương ứng vào đây)*

### 2.3. Viết Test Script cơ bản (Tự động hóa)
- Sử dụng Snippets trong tab **Tests** để tự động kiểm tra Status Code.
- **Đoạn mã (Script):**
  ```javascript
  pm.test("Status code is 200", function () {
      pm.response.to.have.status(200);
  });
