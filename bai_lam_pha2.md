# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 09
- **Họ tên:** Nguyễn Đăng Minh Nhật
- **Lớp:** CNTT1
- **Link repository Pha2:**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt chỗ workshop ra JSON

**KET QUA AI**

```text
TN1:

JSON
{"ma_lop": "NANTAY", "ngay_hoc": "2026-12-13", "nguoi_lon": 2, "tre_em": 1, "ca_hoc": "chieu", "ghi_chu": null}
TN2:

JSON
{"ma_lop": "BANXOAY", "ngay_hoc": "2027-01-10", "nguoi_lon": 3, "tre_em": 0, "ca_hoc": null, "ghi_chu": "1 người bị đau cổ tay"}
TN3:

JSON
{"ma_lop": "VEGOM", "ngay_hoc": null, "nguoi_lon": 4, "tre_em": 0, "ca_hoc": "sang", "ghi__chu": "1 bạn đi xe lăn"}
```

**Link trò chuyện:**

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
Tiền học trước giảm giá:5 người lớn: $5 \times 550.000 = 2.750.000\text{ đồng}$2 trẻ em (8 tuổi và 12 tuổi — thuộc nhóm 6 đến 12 tuổi, tính 70% giá người lớn):Đơn giá/trẻ em: $550.000 \times 70\% = 385.000\text{ đồng}$Thành tiền 2 trẻ em: $2 \times 385.000 = 770.000\text{ đồng}$1 bé 4 tuổi (dưới 6 tuổi đi kèm): Miễn phí ($0\text{ đồng}$)Tổng tiền học ban đầu: $2.750.000 + 770.000 = 3.520.000\text{ đồng}$Tiền học sau giảm giá:Vì nhóm có đủ 5 người lớn trở lên nên được giảm 5% trên tổng tiền học:Mức giảm: $3.520.000 \times 5\% = 176.000\text{ đồng}$Tiền học còn lại: $3.520.000 - 176.000 = 3.344.000\text{ đồng}$Phí nung và giao sản phẩm tận nhà (không áp dụng giảm giá):4 sản phẩm: $4 \times 80.000 = 320.000\text{ đồng}$Tổng thanh toán:$3.344.000 + 320.000 = \mathbf{3.664.000\text{ đồng}}$ 

```

**Link trò chuyện:** https://share.gemini.google/97stJPv2kg9y

### b) Kiểm tra kết quả AI

nhận xét : kết luận AI đúng 

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
Dưới đây là tóm tắt phương án giải quyết theo quy định của xưởng và đối tượng JSON tương ứng với trường hợp của gia đình bạn:

Trường hợp áp dụng: hong_san_pham (5 sản phẩm bị nứt vỡ khi nhận hàng).

Mức hoàn tiền: 
5
×
150.000
=
750.000
 VNĐ
5×150.000=750.000 VNĐ.

Quy trình duyệt: Do tổng mức đền bù (
750.000
 VNĐ
750.000 VNĐ) lớn hơn 
600.000
 VNĐ
600.000 VNĐ, khoản này cần được Quản lý xưởng duyệt trước khi gửi đến khách hàng.

JSON
{
  "ngay_hoc": "2026-11-01",
  "so_khach": 3,
  "so_san_pham_lam": 6,
  "truong_hop_ap_dung": [
    "hong_san_pham"
  ],
  "chi_tiet_den_bu": {
    "hong_san_pham": {
      "so_san_pham_hong": 5,
      "don_gia_hoan_vnd": 150000,
      "thanh_tien_vnd": 750000
    },
    "giao_tre": {
      "ap_dung": false,
      "so_khach": 3,
      "don_gia_voucher_vnd": 50000,
      "thanh_tien_vnd": 0
    },
    "huong_dan": {
      "ap_dung": false,
      "so_khach": 3,
      "don_gia_voucher_vnd": 100000,
      "thanh_tien_vnd": 0
    },
    "khac": {
      "ap_dung": false,
      "chuyen_cskh": false,
      "ghi_chu": "Khach hang hai long voi nguoi huong dan, khong co khieu nai khac."
    }
  },
  "tong_muc_den_bu_vnd": 750000,
  "nguong_can_duyet_vnd": 600000,
  "yeu_cau_quan_ly_xuong_duyet": true,
  "trang_thai": "cho_quan_ly_xuong_duyet"
}
```

**Link trò chuyện:** : https://share.gemini.google/r162EgYb8PG4

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
Chào bạn, giá vé tham gia lớp vẽ gốm VEGOM là 250.000 đồng/người lớn.

Về chính sách đổi lịch: nếu bạn đổi sang buổi khác trước giờ học 1 ngày (tương đương 24 giờ, nằm trong khoảng từ 12 đến dưới 48 giờ trước giờ học), mức phí đổi lịch là 30.000 đồng/người. (Lưu ý: đổi từ 48 giờ trở lên sẽ được miễn phí, và đổi dưới 12 giờ trước giờ học sẽ không áp dụng).

Để mình hỗ trợ đặt chỗ cho bạn, bạn vui lòng cung cấp giúp mình các thông tin sau nhé:

Ngày học mong muốn

Ca học (khung giờ bạn muốn tham gia)

Số lượng người tham gia (người lớn/trẻ em nếu có)
```

**Link trò chuyện:** : https://share.gemini.google/RddVgbs5QOg0
