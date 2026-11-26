# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 04
- **Họ tên:** Đỗ Nguyễn Trung Kiên
- **Lớp:** KS26-CNTT1
- **Link repository Pha2:** https://github.com/TkIen-hue/KS26-CNTT1_PromptAI_H02_Pha1/blob/main/bai_lam_pha2.md
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt vé xe ra JSON

**KET QUA AI**

```JSON
[
  {
    "ma_tuyen": "SGDL",
    "ngay_di": "2026-12-22",
    "ve_nguoi_lon": 2,
    "ve_tre_em": 1,
    "loai_cho": "giuong",
    "ghi_chu": null
  },
  {
    "ma_tuyen": "SGNT",
    "ngay_di": "2027-01-02",
    "ve_nguoi_lon": 3,
    "ve_tre_em": 0,
    "loai_cho": null,
    "ghi_chu": "một người đang mang thai 6 tháng"
  },
  {
    "ma_tuyen": "SGCT",
    "ngay_di": null,
    "ve_nguoi_lon": 4,
    "ve_tre_em": 0,
    "loai_cho": "ghe",
    "ghi_chu": "bà nội đi xe lăn"
  }
]
```

**Link trò chuyện:** https://share.gemini.google/kRBEMO2wubQ7

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
- Thông tin trích xuất từ yêu cầu:Tuyến:
- SGDL (Sài Gòn – Đà Lạt) – Giá vé người lớn: 320.000 đồng
- Số lượng người lớn: 8 ngườiSố lượng trẻ em (5 – 10 tuổi): 3 trẻ (6, 7 và 9 tuổi)
- Số lượng trẻ em (dưới 5 tuổi): 1 trẻ (2 tuổi)
- Hành lý cồng kềnh: 2 kiện
- Chi tiết các bước tính toán:
- Tính tiền vé người lớn:
- Đơn giá vé tuyến SGDL là 320.000 đồng/người lớn.
- Phép tính: 8 . 320.000 = 2.560.000 đồng.
- Tính tiền vé trẻ em:
- 3 trẻ em (6, 7 và 9 tuổi) thuộc nhóm từ 5 đến 10 tuổi, được tính 75% giá vé người lớn 320.000 . 75% = 240.000 đồng/trẻ).
- 1 bé 2 tuổi thuộc nhóm dưới 5 tuổi nên được miễn phí ($0$ đồng).
- Phép tính: (3 . 320.000 . 75%) + (1 . 0) = 3 . 240.000 + 0 = 720.000 đồng.- Tính tiền vé:
- Tổng tiền vé bao gồm tiền vé người lớn và tiền vé trẻ em.
- Phép tính: 2.560.000 + 720.000 = 3.280.000 đồng.
- Áp dụng quy tắc để xét giảm giá đoàn:
- Đoàn có 8 người lớn (thỏa điều kiện từ 6 người lớn trở lên) nên được giảm 5% trên tổng tiền vé.
- Số tiền được giảm: 3.280.000 . 5% = 164.000 đồng.
- Tiền vé sau giảm: 3.280.000 - 164.000 = 3.116.000 đồng.
- Phụ thu:Đoàn có 2 kiện hành lý cồng kềnh với mức phụ thu 100.000 đồng/kiện (không áp dụng giảm giá).
- Phép tính: 2 . 100.000 = 200.000 đồng.
- Tính tổng tiền:Tổng tiền = tiền vé sau giảm + phụ thu.
- Phép tính: 3.116.000 + 200.000 = 3.316.000 đồng.[RESULT: 3.316.000 đồng]
```

**Link trò chuyện:** https://share.gemini.google/uWxUvUa1rBY2

### b) Kiểm tra kết quả AI

Đúng.

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```JSON
{
  "loai_su_co": "sai_loai_xe",
  "so_khach": 3,
  "so_chang_bi_doi": 2,
  "tom_tat": "Khách đặt xe giường nằm cho 3 người nhưng cả 2 chặng đi và về đều bị đổi sang ghế ngồi."
}
```

**Link trò chuyện:** https://share.gemini.google/RjDGzvpbDxzq

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text

```

**Link trò chuyện:** https://share.gemini.google/50UyiDqvASNG
