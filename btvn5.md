# phần 1. phân tích
input. cảm biến đo nhiệt độ, độ ẩm
process. soc xử lý dữ liệu
output. bật hoặc tắt máy bơm

# phần 2. readme.md

## 🚀 smart-farm

* hệ thống tưới lan tự động bằng iot *

### cài đặt
```bash
python main.py
```

### tính năng
- [x] đo nhiệt độ
- [x] đo độ ẩm
- [x] tưới tự động

### thông số
| thiết bị | chức năng |
|---|---|
| soc | xử lý |
| cảm biến | thu dữ liệu |
| máy bơm | tưới nước |

### sơ đồ
![sơ đồ hệ thống](https://mermaid.ink/img/pako:eNpLLkksSVVIzSspVrJSKEktLgEAQ_UGFg)

### cpu xử lý
> fetch lấy lệnh → decode giải mã → execute bật bơm

### mô hình dikw
- data. nhiệt độ 35 độ
- information. nhiệt độ cao
- knowledge. cây có thể thiếu nước
- wisdom. kiểm tra độ ẩm rồi tưới khi cần

# phần 3. lưu ý
nếu ram đầy do log thì kiểm tra file log, sao lưu rồi xóa file cũ, ko xóa file hệ thống.