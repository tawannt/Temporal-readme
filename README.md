# Dự án Tiền xử lý và Phân tích Dữ liệu
# (Ảnh, Tabular, Text)

Dự án này tập trung vào việc khám phá, tiền xử lý và chuẩn bị 3 loại dữ liệu khác nhau cho các mô hình học máy và học sâu.

## Thông tin nhóm

| Tên thành viên | MSSV |
| :--- | :--- |
| Nguyễn Thị Khánh Linh | 23127082 |
| Lê Chí Vỹ | 23127146 |
| Nguyễn Trần Thiên An | 23127315 |
| ... | ... |

## Mô tả tập dữ liệu

### Part 1: Dữ liệu ảnh X-quang Ngực (Viêm phổi)

* **Tên:** [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
* **Tổng quan:** Tập dữ liệu chứa **5,863 ảnh X-quang ngực** (JPEG) được thu thập từ bệnh nhi (1-5 tuổi) tại *Guangzhou Women and Children’s Medical Center, China*.
* **Phân loại:** Dữ liệu được chia thành hai lớp để phân loại nhị phân:
    * `PNEUMONIA` (Viêm phổi): 4,273 ảnh
    * `NORMAL` (Bình thường): 1,584 ảnh
* **Cấu trúc:** Dữ liệu được chia sẵn thành 3 tập: `train/`, `test/`, và `val/`.
* **Lý do lựa chọn:** Đây là dữ liệu y khoa trực quan nhưng chứa nhiều nhiễu (độ sáng không đồng đều, tương phản thấp). Dự án này khám phá các kỹ thuật tiền xử lý (chuẩn hoá, CLAHE, phát hiện biên) để cải thiện độ rõ nét và làm nổi bật các cấu trúc phổi.

### Part 2: Dữ liệu Tabular

* **[Tên tập dữ liệu Tabular]**
* *[Mô tả chi tiết sẽ được cập nhật...]*

### Part 3: Dữ liệu Text

* **[Tên tập dữ liệu Text]**
* *[Mô tả chi tiết sẽ được cập nhật...]*

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
```
**Bước 2: Cài đặt các thư viện cần thiết**
```bash
pip install -r requirements.txt
```
## Cấu trúc thư mục
.
├── README.md
├── requirements.txt
├── data/
│   ├── image/
│   │   └── chest_xray/
│   │       ├── train/
│   │       ├── test/
│   │       └── val/
│   ├── tabular/
│   │   └── [ten_file_tabular.csv]
│   └── text/
│       └── [ten_file_text.csv]
│
├── notebooks/
│   ├── 01_image_preprocessing.ipynb
│   ├── 02_tabular_preprocessing.ipynb
│   └── 03_tabular_preprocessing.ipynb
│
├── docs/
│   └── Report.pdf
