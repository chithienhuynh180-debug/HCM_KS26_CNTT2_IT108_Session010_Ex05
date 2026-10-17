
# Bài: README.md hệ thống Smart-Farm

## Phần 1. Phân tích

- **Input:** độ ẩm, nhiệt độ từ cảm biến, lệnh tưới.
- **Process:** SoC (CPU + RAM) so sánh với ngưỡng, ra quyết định.
- **Output:** bật máy bơm, ghi nhật ký.

````text
Cảm biến --> SoC (CPU + RAM + GPIO) --> Máy bơm
````

## Phần 2. File `README.md`

````markdown
# 🚀 Smart-Farm

Hệ thống **tưới cây tự động** cho trang trại Lan, *đo độ ẩm và nhiệt độ* rồi tự bật máy bơm.

![Sơ đồ hệ thống: cảm biến, SoC, máy bơm](https://greentech.vn/so-do.png)

## Cài đặt

```bash
git clone https://github.com/greentech/smart-farm.git
cd smart-farm
python main.py
```

## Tính năng

- [x] Đọc độ ẩm đất
- [x] Tự động bật máy bơm
- [ ] Gửi cảnh báo qua điện thoại

## Bảng thông số

| Thông số | Giá trị |
|----------|---------|
| Vi điều khiển | SoC Raspberry Pi |
| Nguồn điện | 5V |
| Ngưỡng tưới | 30% |

## Chu kỳ Fetch–Decode–Execute

> **Fetch:** CPU lấy lệnh "tưới Lan" từ RAM.
> **Decode:** giải mã thành lệnh bật máy bơm.
> **Execute:** gửi tín hiệu bật máy bơm.

## Kim tự tháp DIKW

1. **Data:** nhiệt độ 38°C.
2. **Information:** cao hơn mức bình thường 30°C.
3. **Knowledge:** nhiệt độ cao làm đất khô, cây cần nước.
4. **Wisdom:** bật máy bơm tưới cho Lan.

## Lưu ý

Nếu RAM đầy