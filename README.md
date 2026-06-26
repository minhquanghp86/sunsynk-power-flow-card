# Sunsynk Power Flow Card (Bản Tiếng Việt)

Card Home Assistant có hoạt ảnh mô phỏng luồng điện hiển thị trên màn hình Inverter Sunsynk. Bạn có thể dùng card này để hiển thị dữ liệu từ nhiều loại inverter khác nhau như Sunsynk, Deye, Solis, Lux, FoxESS, Goodwe, Huawei... miễn là có đủ dữ liệu cảm biến cần thiết. Xem [wiki](https://github.com/slipx06/sunsynk-power-flow-card/wiki) để biết các phương pháp tích hợp và ví dụ.

> **Lưu ý:** Đây là bản fork được thêm hỗ trợ tiếng Việt. Mọi tính năng giữ nguyên so với [bản gốc](https://github.com/slipx06/sunsynk-power-flow-card).

[![Mở Home Assistant và thêm repository vào HACS](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=minhquanghp86&repository=sunsynk-power-flow-card&category=plugin)
![GitHub release (latest by date)](https://img.shields.io/github/v/release/minhquanghp86/sunsynk-power-flow-card?style=for-the-badge)

## Tài liệu

Tham khảo tài liệu gốc tại [https://slipx06.github.io/sunsynk-power-flow-card/index.html](https://slipx06.github.io/sunsynk-power-flow-card/index.html)

## Tính năng

- Lựa chọn giữa ba kiểu card: `compact`, `lite` hoặc `full`.
- Bố cục màn hình rộng 16:9.
- Hoạt ảnh luồng điện dựa trên giá trị cảm biến dương/âm/không với tốc độ động có thể cấu hình (hỗ trợ đảo chiều ắc quy, AUX và lưới điện).
- Hình ảnh ắc quy động theo SOC.
- Trạng thái kết nối lưới điện.
- Cấu hình dung lượng ắc quy và SOC tắt máy để tính và hiển thị thời gian còn lại của ắc quy dựa trên mức tiêu thụ hiện tại và cài đặt time slot — có thể bật/tắt.
- Số liệu tiêu thụ trong ngày có thể bật/tắt.
- Ẩn toàn bộ dữ liệu PV nếu chưa lắp đặt hoặc chỉ định số MPPT đang sử dụng. Đặt nhãn MPPT tùy chỉnh.
- Hiển thị cài đặt "Dùng hẹn giờ" và "Ưu tiên năng lượng" (Ưu tiên tải hoặc Ưu tiên ắc quy) dưới dạng biểu tượng động, có thể ẩn nếu không cần. Nếu cấu hình dạng switch có thể bật/tắt trực tiếp trên card.
- Có thể thay đổi kích thước card bằng thuộc tính `card_height` và `card_width`.
- AUX và tải phụ có thể ẩn hoặc đặt nhãn tùy chỉnh.
- Tùy chỉnh màu sắc và hình ảnh.
- Hầu hết các thực thể có thể bấm để xem thông tin chi tiết.
- Các điểm dữ liệu tùy chọn gồm tỉ lệ tự chủ, nhiệt độ ắc quy, nhiệt độ AC và DC.
- Hiển thị thêm tải phụ, tải chính và tải AUX.
- Hiển thị giá điện theo kWh và trạng thái bán điện mặt trời.
- Chọn model inverter để hiển thị thông báo trạng thái phù hợp với từng hãng: Sunsynk, Lux, Goodwe, Solis.

## Ảnh minh họa

_Phiên bản Compact_

![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/b1e437a8-d1f7-4d6a-a549-1cc908950002)
![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/49c499c5-9d2b-43e7-8f5d-5b9da5e07fb9)

_Phiên bản Lite_

![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/d25c621c-2607-445f-b3a3-865930387a05)
![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/5a9078ee-7375-4f1c-affa-6fe291d62f8a)
![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/73d6fae3-3e6b-4891-acc2-deb29156cd2d)
![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/54ae290d-aa5c-428e-8a00-2a75e11c2de8)

_Phiên bản Full_

![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/fdcce257-e7b5-4874-926c-17e911e83eba)
![image](https://github.com/slipx06/sunsynk-power-flow-card/assets/7227275/12af5b02-c456-4685-a50f-bd0044b9e9b0)

_Phiên bản Full màn hình rộng (2 ắc quy)_

![{4D3F02C5-3DC5-4995-AD99-7478E6DE5557}](https://github.com/user-attachments/assets/af169593-c73f-469e-bc8b-62fb72b8af43)

_Phiên bản Lite màn hình rộng (2 ắc quy)_

![{F448EFB0-5549-470B-BAE0-13F9DF2E3769}](https://github.com/user-attachments/assets/100c80d2-1d5f-46f4-ae83-f48c923cadf6)

_Phiên bản Compact màn hình rộng (2 ắc quy)_

![{B8CBC3C3-0E0A-4E37-B489-C41CB8EA4E7E}](https://github.com/user-attachments/assets/1cd5508d-33a0-4df9-9665-5a4d9e753178)

## Cài đặt

Card có thể cài qua HACS (khuyến nghị) hoặc thủ công.

### Cài đặt qua HACS

[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg)](https://github.com/custom-components/hacs)

1. Cài đặt HACS.
2. Vào HACS → menu 3 chấm → **Custom repositories**.
3. Nhập `minhquanghp86/sunsynk-power-flow-card`, chọn loại **Lovelace** → bấm **Add**.
4. Tìm kiếm **sunsynk** trong HACS → bấm **Install**.

Hoặc bấm nút bên dưới:

[![Mở Home Assistant và thêm repository vào HACS](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=minhquanghp86&repository=sunsynk-power-flow-card&category=plugin)

### Cài đặt thủ công

1. Tạo thư mục mới trong `www` với tên `sunsynk-power-flow-card`, ví dụ: `www/sunsynk-power-flow-card/`.
2. Sao chép file `sunsynk-power-flow-card.js` vào thư mục đó.
3. Thêm resource vào Dashboard. Có thể thêm `?ver=x` vào cuối tên file và tăng x mỗi khi tải phiên bản mới để tránh dùng bản cache cũ. Nên xóa cache trình duyệt sau mỗi lần cập nhật.

![image](https://user-images.githubusercontent.com/7227275/235441241-93ab0c7d-341d-428f-8ca8-60ec932dde2d.png)
