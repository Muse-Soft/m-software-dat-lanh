# DESIGN.md — Landing page xưởng gốm thủ công Đất Lành (MSR-44)

> Tài liệu thiết kế chốt cho sprint TEC-332. Dev (task Dev của sprint) dựng đúng tài liệu này, không tự thêm màu, font hay khối ngoài danh sách. QA đối chiếu bản dựng với tài liệu này, kèm kiểm tra đa dạng theo OPERATIONS.md mục 16.5.

## 0. Khác biệt so với các project gần nhất (bắt buộc theo mục 16.5 — đã đọc thật ngày 2026-10-25)

Thứ tự project mới nhất lấy từ mô tả task TEC-333 và đối chiếu trực tiếp DESIGN.md của các project gần nhất trên GitHub (đọc qua raw.githubusercontent.com ngày 2026-10-25):

1. **Gác Sách** (m-software-gac-sach, TEC-326) — archetype: **A4 Bento-masonry**; cặp font: **EB Garamond + Be Vietnam Pro**; nhiệt màu: **sáng-ấm** (nền #FBF6EE, chữ #2B2620, nhấn đỏ gạch #A63D2F); điểm nhấn: "gáy sách làm vạch chia khối".
2. **Thả Lỏng** (m-software-tha-long, TEC-319) — archetype: **A3 Lệch tâm**; cặp font: **Playfair Display + Be Vietnam Pro**; nhiệt màu: **sáng-ấm nhạt** (nền #F4F1EA, chữ #2E2A33, nhấn tím oải hương #7C6A9E); điểm nhấn: "đường thở".
3. **Thời Khắc** (m-software-thoi-khac, TEC-312) — archetype: **A7 Typography-first**; cặp font: **Noto Serif Display + Be Vietnam Pro**; nhiệt màu: **tối-trung tính** (nền than chì #0F1419, chữ kem #ECE7DD, nhấn vàng đồng #C9A86A); điểm nhấn: chữ số khổng lồ kiểu mặt số + dải 60 vạch phút.

Lựa chọn cho Đất Lành (đối chiếu trực tiếp với 3 project trên):

- **Archetype: A1 Editorial dọc** — KHÁC A4 của project liền trước (Gác Sách) và KHÁC A3 của project liền trước nữa (Thả Lỏng), thỏa luật "không dùng lại archetype của 2 project liền trước"; cũng khác A7 của Thời Khắc. Cách editorial thể hiện ở: một cột dọc duy nhất, ảnh lớn dẫn nhịp từng khối, tiêu đề khối đặt trên ảnh hoặc ngay dưới ảnh với khoảng trắng lớn (96px desktop), không lưới ô lệch cỡ, không lệch trục, không chữ khổng lồ dẫn nhịp.
- **Cặp font: Cormorant Garamond + Be Vietnam Pro** — KHÁC nguyên cặp EB Garamond + Be Vietnam Pro của project liền trước (Gác Sách): font tiêu đề đổi sang Cormorant Garamond (serif thanh mảnh, hỗ trợ tiếng Việt); cũng khác Playfair Display + Be Vietnam Pro của Thả Lỏng và Noto Serif Display + Be Vietnam Pro của Thời Khắc.
- **Nhiệt màu: trung tính trầm (muted neutral) — ĐIỀU CHỈNH so với công thức gợi ý.** Chuỗi nhiệt gần nhất: Thời Khắc tối-trung tính → Thả Lỏng sáng-ấm → Gác Sách sáng-ấm: đã có 2 project sáng-ấm liên tiếp, giữ nguyên nền kem sáng #F3EEE6 của công thức gợi ý sẽ tạo chuỗi 3 sáng-ấm liên tiếp, vi phạm luật "tránh 3 project liên tiếp cùng một nhiệt màu". Vì vậy nền chính đổi từ kem sáng #F3EEE6 sang **đất xám trung tính #E7E1D6** (độ bão hòa thấp, không phải kem sáng-ấm), chữ chính đổi sang than đất trung tính #2B2B26, và khối Quy trình dùng nền tối đất #2B2B26 xen kẽ để phá nhịp sáng. Giữ nguyên tinh thần công thức gợi ý: nhấn chính vẫn là **xanh men ngọc #2E6B62**, không khí vẫn wabi-sabi, ảnh vẫn đồng tông đất và men xanh — chỉ đổi nhiệt màu nền từ sáng-ấm sang trung tính trầm, lý do ghi rõ tại đây.
- **Điểm nhấn đặc sắc riêng: "vệt men chảy"** — dưới mỗi tiêu đề khối là một đường kẻ men ngọc 3px, dài 64px, kèm 1 giọt men tròn đường kính 10px lệch về phía phải của đường kẻ, mô phỏng men chảy trên thân gốm (mô tả cụ thể ở mục 7). Khác hẳn "gáy sách", "đường thở" và "vạch phút" của 3 project gần nhất.

## 1. Tổng quan và phong cách tham chiếu (duy nhất)

- Sản phẩm: landing page 1 trang cho xưởng gốm thủ công Đất Lành — làm gốm bằng tay, bán bát đĩa hằng ngày, bình hoa, chén trà; nhận đặt lớp học trải nghiệm nặn gốm.
- Phong cách tham chiếu duy nhất: **wabi-sabi Nhật Bản** — đất nung mộc, men rạn, hình dáng không hoàn hảo có chủ ý, ánh sáng tự nhiên dịu qua cửa sổ xưởng, ít đồ, nhiều khoảng thở; chữ serif thanh mảnh, không ồn ào kiểu quảng cáo giảm giá.
- CẤM: template bán hàng (giỏ hàng, nút mua ngay, banner khuyến mãi), icon stock đủ màu, ảnh nền trắng studio kiểu sàn thương mại điện tử, lưới thẻ đều tăm tắp không có ảnh lớn dẫn nhịp.

## 2. Bảng màu — ĐÚNG 6 mã hex (không dùng màu ngoài bảng này)

| Mã | Vai trò |
|---|---|
| `#E7E1D6` | Nền chính — đất xám trung tính, toàn trang |
| `#D5CCC0` | Nền phụ — đất xám sậm hơn, dùng cho thẻ bộ sưu tập, thẻ cảm nhận, chân trang |
| `#2B2B26` | Chữ chính — than đất trung tính, tiêu đề và nội dung chính; cũng là nền của khối Quy trình (khi đó chữ trên nền này dùng màu nền chính #E7E1D6) |
| `#6E6A60` | Chữ phụ — xám đất, mô tả phụ, giá thứ cấp, chú thích ảnh |
| `#2E6B62` | Nhấn chính — xanh men ngọc, nút chính, giá mẫu, vệt men chảy, số bước quy trình |
| `#B07A4A` | Nhấn phụ — đất nung nhạt, đường viền, giá phụ, viền ảnh khi ảnh lỗi/chưa tải |

Quy tắc dùng màu:

- Nền trung tính trầm chiếm đa số diện tích; chữ than đất trên nền đất xám phải đọc rõ, không dùng chữ phụ cho đoạn văn chính.
- Xanh men ngọc chỉ làm điểm nhấn (nút, giá, vệt men), không phủ mảng lớn; đất nung nhạt chỉ làm viền và chi tiết phụ.

## 3. Font chữ

- **Tiêu đề: Cormorant Garamond** (serif thanh mảnh, hỗ trợ tiếng Việt) — tiêu đề khối 40px desktop / 30px mobile, đậm vừa (600), giãn dòng 1.2; tên xưởng ở hero 64px desktop / 40px mobile.
- **Nội dung: Be Vietnam Pro** (sans hỗ trợ tiếng Việt) — nội dung 17px, giãn dòng 1.7; chú thích 14px, màu chữ phụ.

## 4. Bố cục — archetype A1 Editorial dọc

- Một cột dọc duy nhất, chiều rộng tối đa 1120px, lề ngoài 24px (mobile) / 48px (desktop). Khoảng trắng giữa các khối: 96px (desktop), 64px (mobile).
- Thứ tự khối (không đổi): (1) hero ảnh lớn toàn màn hình → (2) giới thiệu xưởng + triết lý "làm chậm, làm thật" → (3) bộ sưu tập → (4) quy trình 4 bước → (5) lớp học trải nghiệm → (6) cảm nhận khách hàng → (7) form liên hệ / đặt lịch → (8) chân trang.

## 5. Từng khối

1. **Hero (100vh):** ảnh toàn màn hình bàn tay vuốt đất sét trên bàn xoay, phủ lớp tối nhẹ để chữ đọc được; tên xưởng "Đất Lành" + câu triết lý ngắn + nút CTA "Xem bộ sưu tập" (men ngọc) cuộn xuống khối 3.
2. **Giới thiệu + triết lý:** 2 đoạn ngắn, không ảnh; tiêu đề "Làm chậm, làm thật" + vệt men chảy.
3. **Bộ sưu tập:** 3 món, mỗi món một ảnh lớn 4:5 + tên món + giá ghi rõ "Giá mẫu" (bát đĩa hằng ngày, bình hoa, chén trà); ảnh xếp dọc, xen kẽ chú thích ngắn; không lưới thẻ.
4. **Quy trình 4 bước:** nền tối #2B2B26, chữ kem #E7E1D6; 4 bước xếp dọc, mỗi bước có số men ngọc lớn (01–04) + tên bước + 1 câu mô tả; bước: nhào đất → tạo hình → tráng men → nung.
5. **Lớp học trải nghiệm:** ảnh 3:2 + mô tả lớp + giá ghi rõ "Giá mẫu: 450.000đ/buổi" + nút "Đặt lịch học thử" cuộn xuống form.
6. **Cảm nhận khách hàng:** 3 cảm nhận ngắn, thẻ nền phụ #D5CCC0; tên người cảm nhận để [CẦN BỔ SUNG] nếu chưa có tên thật — không bịa tên.
7. **Form liên hệ / đặt lịch:** 4 trường (họ tên, điện thoại, loại yêu cầu, ghi chú) — CHỈ giao diện: submit chỉ preventDefault, không fetch, không action, không mailto, không tel:. Địa chỉ, điện thoại xưởng để [CẦN BỔ SUNG], không bịa số liệu thật.
8. **Chân trang:** tên xưởng + [CẦN BỔ SUNG] (địa chỉ, điện thoại, giờ mở cửa, người phụ trách) + ghi chú "Ảnh và giá trên trang là ảnh mẫu / giá mẫu".

## 6. Quy tắc hình ảnh

- Hero: ảnh ngang toàn màn hình 100vh, bàn tay vuốt đất sét trên bàn xoay, tông đất + men xanh, ánh sáng tự nhiên dịu.
- Bộ sưu tập: ảnh 4:5 từng món, nền xưởng hoặc nền đất trung tính, không nền trắng studio.
- Lớp học: ảnh 3:2, người học nặn gốm trong xưởng, cùng tông.
- Tất cả ảnh mẫu phải đồng tông (đất nung, men xanh ngọc, ánh sáng dịu), chất lượng cao, kiểm tra HTTP 200 trước khi dùng; ghi rõ là ảnh mẫu trong comment kết quả của Dev.
- Responsive: breakpoint 768px (tiêu đề khối 34px, khoảng trắng khối 72px) và 480px (tiêu đề khối 30px, khoảng trắng khối 64px, hero chữ 40px).

## 7. Điểm nhấn đặc sắc riêng — "vệt men chảy"

- Dưới mỗi tiêu đề khối (trừ hero): một đường kẻ ngang màu men ngọc #2E6B62, dày 3px, dài 64px, đặt lệch trái theo lề chữ; ở đầu phải của đường kẻ có 1 giọt men tròn đường kính 10px cùng màu men ngọc, như giọt men vừa chảy xuống thân gốm.
- Trên nền tối của khối Quy trình, vệt men dùng màu men ngọc #2E6B62 trên nền #2B2B26 (giữ nguyên hình dáng, không đổi màu).
- Không dùng vệt men ở nơi khác (không làm viền thẻ, không làm nền nút) để điểm nhấn không bị loãng.
