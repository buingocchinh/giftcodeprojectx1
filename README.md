# 🎁 CGIFT - Plugin Giftcode Thế hệ mới

![Phiên bản](https://img.shields.io/badge/version-1.0.0-blue?style=for-the-badge)
![Nền tảng](https://img.shields.io/badge/platform-Spigot%20%7C%20Paper-brightgreen?style=for-the-badge)
![Tác giả](https://img.shields.io/badge/Remake%20bởi-Bnchinh-orange?style=for-the-badge)

**CGIFT** là một plugin giftcode mạnh mẽ và linh hoạt, được làm lại (remake) và cải tiến bởi **[Bnchinh](https://github.com/[tên-github-của-bạn])** từ plugin `DHgiftcode` tiền nhiệm.

Plugin này cung cấp một giải pháp toàn diện để tạo, quản lý và trao tặng các mã quà tặng (giftcode) cho người chơi, giúp tăng cường sự tương tác và tạo động lực cho cộng đồng máy chủ của bạn.

---

## ✨ Tính năng nổi bật

* **Quản lý mã trực quan:** Dễ dàng tạo, xóa, và kiểm tra thông tin giftcode.
* **Phần thưởng đa dạng:** Hỗ trợ tặng vật phẩm (items), tiền (economy - yêu cầu Vault), và thực thi lệnh (commands) khi người chơi sử dụng mã.
* **Giới hạn linh hoạt:** Thiết lập giới hạn số lần sử dụng cho mỗi mã (dùng một lần hoặc nhiều lần).
* **Tùy chỉnh thông báo:** Toàn bộ các tin nhắn, thông báo đều có thể được tùy chỉnh trong file `config.yml`.
* **Mã nguồn tối ưu:** Được viết lại để đảm bảo hiệu suất ổn định và dễ dàng bảo trì.

---

## 🚀 Cài đặt & Build từ Source (Git Codespace)

Project này được thiết lập để phát triển và build dễ dàng ngay trên **Git Codespace**.

1.  **Mở Codespace:** Khởi động môi trường Codespace của bạn cho repository này.
2.  **Build Plugin:** Mở Terminal và chạy lệnh build (giả sử bạn dùng Maven):
    ```bash
    mvn clean package
    ```
    *(Nếu bạn dùng Gradle, hãy thay bằng: `./gradlew build`)*

3.  **Lấy file .jar:** File plugin (ví dụ: `CGIFT-1.0.jar`) sẽ nằm trong thư mục `target/` (với Maven) hoặc `build/libs/` (với Gradle).
4.  **Cài đặt lên máy chủ:**
    * Tải file `.jar` đã build về máy.
    * Đặt file vào thư mục `plugins/` của máy chủ (Spigot/Paper).
    * Khởi động lại máy chủ.

---

## 🎮 Lệnh & Quyền (Commands & Permissions)

*(Lưu ý: Đây là các lệnh và quyền giả định. Bạn hãy chỉnh sửa lại cho đúng với plugin của mình khi hoàn thiện.)*

### Lệnh cho Quản trị viên (Admin)

| Lệnh | Mô tả | Quyền |
| :--- | :--- | :--- |
| `/cgift create <tên_mã> [số_lượng]` | Tạo một mã giftcode mới. | `cgift.admin.create` |
| `/cgift delete <tên_mã>` | Xóa một mã giftcode. | `cgift.admin.delete` |
| `/cgift reload` | Tải lại file cấu hình. | `cgift.admin.reload` |
| `/cgift list` | Xem danh sách các mã. | `cgift.admin.list` |

### Lệnh cho Người chơi (Player)

| Lệnh | Mô tả | Quyền |
| :--- | :--- | :--- |
| `/giftcode <tên_mã>` | Sử dụng mã giftcode. | `cgift.use` |

---

## ❤️ Ghi công

* **Tác giả Remake:** **[Bnchinh](https://github.com/[tên-github-của-bạn])**
* **Plugin gốc:** Cảm ơn `DHgiftcode` đã cung cấp nền tảng và ý tưởng ban đầu.

---

## 📜 Giấy phép

Project này được cấp phép theo [Giấy phép MIT](LICENSE). (Hoặc bất kỳ giấy phép nào bạn chọn).
