# CS2 ImGui DX11 Menu Template

Một mã nguồn mở (Template) viết bằng **C++** hỗ trợ khởi tạo **ImGui Menu** cho tựa game **Counter-Strike 2**. Project này đã được setup sẵn phần Hook DirectX 11, xử lý Input (Bật/Tắt Menu) và dọn dẹp tài nguyên. Người dùng chỉ cần tập trung viết tính năng (Features) cho game.

## ✨ Tính năng sẵn có (Features)
- **DirectX 11 Hook**: Tối ưu sẵn phần khởi tạo `RenderTargetView` và `SwapChain`.
- **ImGui Setup**: Tích hợp sẵn thư viện ImGui bản mới nhất.
- **Safe Code**: Đã xử lý các lỗi crash logic (`!` thay vì `= nullptr`), quản lý bộ nhớ sạch sẽ.
- **Dễ mở rộng**: Thích hợp làm nền tảng để phát triển Cheat/Tool (Esp, Aimbot, Skinchanger...).

## 🚀 Hướng dẫn cài đặt & Biên dịch (Build)
1. Tải hoặc Clone repository này về máy:
   ```bash
   git clone https://github.com
   ```
2. Mở file `.sln` bằng **Visual Studio 2022 hoặc bản khác**.
3. Cài đặt cấu hình biên dịch thành **Release | x64**.
4. Nhấn `Ctrl + Shift + B` để tiến hành Build ra file `.dll`.

## 💉 Cách sử dụng (How to use)
1. Sử dụng một phần mềm Injector bất kỳ (ví dụ: *Xenos Injector*, *Process Hacker*).
2. Tiêm (Inject) file `.dll` vừa build vào tiến trình game `cs2.exe`.
3. Nhấn phím **Insert** (hoặc phím bạn cài đặt) trên bàn phím để Bật/Tắt giao diện menu ImGui.

## 🛠️ Hướng dẫn thêm tính năng riêng của bạn
Để thêm các tính năng hack/mod, bạn chỉ cần code bổ sung vào:
- `interfaces.cpp`: Nơi bạn lấy thêm các Interface khác của game CS2 từ mạng (Network/Engine).
- Phần vẽ giao diện ImGui (thường ở file render/gui): Thêm các nút bấm Checkbox, Slider để người dùng tương tác.

## 📄 Giấy phép (License)
Dự án này tuân theo giấy phép MIT - Miễn phí sử dụng và chia sẻ.
