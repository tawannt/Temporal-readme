# Dự án Tiền xử lý và Phân tích Ảnh X-quang Ngực (Viêm phổi)

Dự án này tập trung vào việc khám phá, tiền xử lý và chuẩn bị tập dữ liệu "Chest X-Ray Images (Pneumonia)" cho các mô hình học sâu (Deep Learning).

## 👥 Thông tin nhóm

| Tên thành viên | MSSV |
| :--- | :--- |
| [Tên thành viên 1] | [MSSV 1] |
| [Tên thành viên 2] | [MSSV 2] |
| [Tên thành viên 3] | [MSSV 3] |
| ... | ... |

## 📊 Mô tả tập dữ liệu

* **Tên:** [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
* **Tổng quan:** Tập dữ liệu chứa **5,863 ảnh X-quang ngực** (JPEG) được thu thập từ bệnh nhi (1-5 tuổi) tại *Guangzhou Women and Children’s Medical Center, China*.
* **Phân loại:** Dữ liệu được chia thành hai lớp để phân loại nhị phân:
    * `PNEUMONIA` (Viêm phổi): 4,273 ảnh
    * `NORMAL` (Bình thường): 1,584 ảnh
* **Cấu trúc:** Dữ liệu được chia sẵn thành 3 tập: `train/`, `test/`, và `val/`.
* **Lý do lựa chọn:** Đây là dữ liệu y khoa trực quan nhưng chứa nhiều nhiễu (độ sáng không đồng đều, tương phản thấp). Dự án này khám phá các kỹ thuật tiền xử lý (chuẩn hoá, CLAHE, phát hiện biên) để cải thiện độ rõ nét và làm nổi bật các cấu trúc phổi, nhằm tạo đầu vào ổn định và giàu thông tin hơn cho các mô hình DL.

## 🚀 Hướng dẫn chạy Notebooks

### 1. Yêu cầu về môi trường

Dự án này yêu cầu Python 3.x và các thư viện được liệt kê trong file `requirements.txt`.

**Bước 1: (Tùy chọn) Tạo và kích hoạt môi trường ảo**
```bash
# Tạo môi trường ảo
python -m venv venv

# Kích hoạt môi trường (Windows)
.\venv\Scripts\activate

# Kích hoạt môi trường (macOS/Linux)
source venv/bin/activate

