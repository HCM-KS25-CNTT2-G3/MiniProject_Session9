# 📦 Web-based Warehouse Management System

> **Dự án:** Ứng dụng Quản lý kho hàng trên trình duyệt.  
> **Team size:** 8 thành viên.  
> **Công nghệ:** HTML, JavaScript (Core).

## 📖 Giới thiệu
Dự án xây dựng một hệ thống quản lý kho đơn giản chạy trên trình duyệt sử dụng `prompt` và `alert`. Hệ thống sử dụng cơ chế **3 mảng song song (Parallel Arrays)** để lưu trữ dữ liệu và vòng lặp vô hạn để duy trì menu điều khiển.

---

## ⚙️ Quy ước Kỹ thuật (QUAN TRỌNG)
Để đảm bảo code của 8 người khi ghép lại hoạt động ngay lập tức, **tất cả thành viên bắt buộc** tuân thủ tên biến toàn cục sau đây, không được tự ý đổi tên:

1.  **`names`**: Mảng chứa tên sản phẩm (String).
2.  **`prices`**: Mảng chứa giá sản phẩm (Number).
3.  **`stocks`**: Mảng chứa số lượng tồn kho (Number).

---

## 👥 Bảng Phân Công Tóm Tắt

| Thành viên | Vai trò | Tên hàm bắt buộc (Function Signature) |
| :--- | :--- | :--- |
| **TV 1** | **Leader & Core** | `main()` (Chứa vòng lặp chính & Switch Case) |
| **TV 2** | **UI/UX** | `showMenu()` |
| **TV 3** | **Logic Dev** | `filterHighValue(names, prices)` |
| **TV 4** | **QA Dev** | `validateData(prices, stocks)` |
| **TV 5** | **Finance Dev** | `calculateTotal(prices, stocks)` |
| **TV 6** | **Sales Dev** | `applyDiscount(prices)` |
| **TV 7** | **Search Dev** | `searchProduct(names, prices, stocks)` |
| **TV 8** | **Reporter** | `viewStockReport(names, stocks)` |

---

## 📝 Chi Tiết Nhiệm Vụ (Task Specifications)

Các thành viên copy đúng khung code (Template) dưới đây về máy cá nhân, viết logic vào bên trong, sau đó gửi lại cho **TV 1**.

### 👤 Thành viên 1: Leader (Khởi tạo & Ghép nối)
* **File:** `script.js` (File chính).
* **Nhiệm vụ:**
    1.  Khai báo 3 mảng `names`, `prices`, `stocks` với dữ liệu mẫu (5-10 sản phẩm).
    2.  Viết hàm `main()` chứa vòng lặp `while(true)`.
    3.  Gọi hàm `showMenu()` để lấy lựa chọn.
    4.  Dùng `switch/case` để gọi hàm của các thành viên khác.

### 👤 Thành viên 2: Interface (Menu)
* **Nhiệm vụ:** Hiển thị danh sách 7 chức năng và trả về lựa chọn của user.
* **Template:**
```javascript
function showMenu() {
    // 1. Tạo biến chuỗi menu (dùng \n để xuống dòng cho đẹp).
    // 2. Dùng prompt(menu) để lấy dữ liệu.
    // 3. Dùng parseInt() để chuyển dữ liệu nhập vào thành số.
    // 4. return số vừa chuyển.
}
