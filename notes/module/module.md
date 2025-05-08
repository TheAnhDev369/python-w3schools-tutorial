# Module sys trong Python

## 1. Giới thiệu
`sys` là một module tích hợp (built-in module) quan trọng trong Python, được sử dụng để tương tác với trình thông dịch Python và môi trường hệ thống.

## 2. Cách Import
```python
import sys
```

## 3. Các chức năng chính

### 3.1. Thông tin hệ thống
| Thuộc tính/Phương thức | Mô tả |
|------------------------|--------|
| `sys.version` | Thông tin về phiên bản Python đang sử dụng |
| `sys.platform` | Thông tin về nền tảng hệ điều hành |
| `sys.executable` | Đường dẫn đến trình thông dịch Python |

### 3.2. Quản lý đường dẫn
| Thuộc tính/Phương thức | Mô tả |
|------------------------|--------|
| `sys.path` | Danh sách các đường dẫn tìm kiếm module |
| `sys.modules` | Dictionary chứa các module đã được import |

### 3.3. Xử lý đầu vào/đầu ra tiêu chuẩn
| Thuộc tính/Phương thức | Mô tả |
|------------------------|--------|
| `sys.stdin` | Đầu vào chuẩn |
| `sys.stdout` | Đầu ra chuẩn |
| `sys.stderr` | Đầu ra lỗi chuẩn |

### 3.4. Quản lý bộ nhớ và tài nguyên
| Thuộc tính/Phương thức | Mô tả |
|------------------------|--------|
| `sys.getsizeof()` | Lấy kích thước của đối tượng trong bộ nhớ |
| `sys.getrefcount()` | Đếm số tham chiếu đến một đối tượng |

## 4. Ví dụ sử dụng

### 4.1. Kiểm tra phiên bản Python
```python
import sys
print(sys.version)
```

### 4.2. Kiểm tra hệ điều hành
```python
import sys
print(sys.platform)
```

### 4.3. Xem đường dẫn tìm kiếm module
```python
import sys
print(sys.path)
```

### 4.4. Lấy đường dẫn Python interpreter
```python
import sys
print(sys.executable)
```

## 5. Các lệnh terminal liên quan

### 5.1. Chạy file Python
```bash
python tên_file.py
```

### 5.2. Chạy module
```bash
python -m tên_module
```

### 5.3. Vào Python shell
```bash
python
```

## 6. Lưu ý quan trọng
- Python Shell là môi trường giao diện dòng lệnh cho phép thực thi mã Python trực tiếp
- Sử dụng `exit()` để thoát khỏi Python shell
- Module sys rất hữu ích cho việc:
  - Kiểm tra và quản lý môi trường Python
  - Xử lý tham số dòng lệnh
  - Tương tác với hệ điều hành
  - Quản lý bộ nhớ và tài nguyên hệ thống

## 7. Code mẫu hoàn chỉnh
```python
# sys là module tích hợp trong Python, cung cấp các biến và hàm để:
# - Tương tác với trình thông dịch Python
# - Truy cập thông tin hệ thống
# - Quản lý đường dẫn và module
# - Xử lý đầu vào/đầu ra tiêu chuẩn
import sys

# Lấy thông tin về phiên bản Python
print("Python version:")
print(sys.version)
print("\n")

# Lấy đường dẫn đến thư mục chứa file python
print("Python executable path:")
print(sys.executable)
print("\n")

# Lấy danh sách đường dẫn tìm kiếm module
print("Python module search paths:")
print(sys.path)
print("\n")

# Lấy thông tin về hệ điều hành
print("Operating system platform:")
print(sys.platform)
print("\n")
```

## 8. Tài liệu tham khảo
- [Python sys module documentation](https://docs.python.org/3/library/sys.html)
- [Python.org](https://www.python.org/)

---
*Ghi chú: Tài liệu này được tạo để giúp hiểu rõ hơn về module sys trong Python. Hãy tham khảo tài liệu chính thức của Python để biết thêm chi tiết.*
