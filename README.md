## 1. Tạo Volume
Lệnh: `docker volume create easy-volume`

Kết quả: Tạo thành công Volume `easy-volume`.

## 2. Ghi dữ liệu vào Volume
Lệnh: `docker run --rm -v easy-volume:/data alpine sh -c "echo 'Luu tru du lieu Docker' > /data/test.txt"`

Kết quả: Ghi nội dung `Luu tru du lieu Docker` vào file `/data/test.txt`.

## 3. Đọc dữ liệu từ container thứ hai
Lệnh: `docker run --rm -v easy-volume:/data alpine cat /data/test.txt`

Kết quả: `Luu tru du lieu Docker`

