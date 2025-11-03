# Dự án Tiền xử lý và Phân tích Dữ liệu

Dự án này tập trung vào việc khám phá, tiền xử lý và chuẩn bị 3 loại dữ liệu khác nhau.

## Thông tin nhóm

| Tên thành viên | MSSV |
| :--- | :--- |
| Nguyễn Thị Khánh Linh | 23127082 |
| Lê Chí Vỹ | 23127146 |
| Nguyễn Trần Thiên An | 23127315 |

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

* **Tập dữ liệu:** [Unclean Airline Customer Dataset](https://www.kaggle.com/datasets/edisugiarto/unclean-airline-customer-dataset/data)
* **Nguồn:** Kaggle
* **Kích thước:** 62,988 dòng, 23 cột
* **Mô tả đặc trưng:**

| Tên đặc trưng | Mô tả |
|---------------|-------|
| `MEMBER_NO` | Mã định danh hội viên |
| `FFP_DATE` | Ngày đăng ký hội viên |
| `FIRST_FLIGHT_DATE` | Ngày bay chuyến đầu tiên |
| `GENDER` | Giới tính |
| `FFP_TIER` | Hạng hội viên |
| `WORK_CITY` | Thành phố nơi làm việc |
| `WORK_PROVINCE` | Tỉnh nơi làm việc |
| `WORK_COUNTRY` | Quốc gia nơi làm việc |
| `AGE` | Tuổi |
| `LOAD_TIME` | Ngày load dữ liệu |
| `FLIGHT_COUNT` | Số chuyến bay của khách hàng |
| `BP_SUM` | Tổng số điểm cơ bản |
| `SUM_YR_1` | Tổng chi tiêu khách hàng năm đầu |
| `SUM_YR_2` | Tổng chi tiêu khách hàng năm thứ hai |
| `SEG_KM_SUM` | Tổng số km đã bay, di chuyển |
| `LAST_FLIGHT_DATE` | Ngày bay chuyến cuối cùng |
| `LAST_TO_END` | Thời gian `LAST_FLIGHT_DATE` - `LOAD_TIME` |
| `AVG_INTERVAL` | Thời gian trung bình giữa các chuyến bay |
| `MAX_INTERVAL` | Thời gian tối đa giữa các chuyến bay |
| `EXCHANGE_COUNT` | Số điểm đổi thưởng |
| `avg_discount` | Mức giảm giá trung bình |
| `Points_Sum` | Tổng điểm tích lũy |
| `Point_NotFlight` | Số điểm tích lũy không từ việc bay |

* **Ứng dụng:** Thường được dùng cho các bài toán phân tích khám phá dữ liệu (EDA), làm sạch dữ liệu hay các bài toán phân cụm để phân tích RFM của khách hàng

### Part 3: Dữ liệu Text

* **[Tên tập dữ liệu Text]**
* *[Mô tả chi tiết sẽ được cập nhật...]*

## Hướng dẫn chạy Notebooks

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

