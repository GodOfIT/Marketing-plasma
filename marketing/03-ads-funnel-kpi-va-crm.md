# Kế hoạch ads, phễu, CRM, tài chính thử nghiệm — Plasma

## 1. Hạ tầng và data governance
- Website: /plasma/, /seo/ hoặc /se-o/ (SEO nên là \`/dieu-tri-seo/\`), /sac-to-moi/, /tham-my-mi/ (**chỉ công khai landing dịch vụ đủ pháp lý**) và /thiet-bi-plasma/ cho B2B nếu có.
- Có FAQ “plasma lạnh và plasma nhiệt khác nhau thế nào?”, trang về cơ sở/người hành nghề, bảng giá thực, giới hạn phương pháp, chính sách bảo mật.
- Đặt Google Analytics 4, Google Tag Manager, conversion API hoặc pixel theo chính sách đồng ý; UTM \`utm_source\`, \`utm_medium\`, \`utm_campaign\`, \`utm_content\`, \`utm_term\`. Không chuyển tình trạng sức khỏe/ảnh khách hoặc dữ liệu nhạy cảm qua pixel/sự kiện ngoài.
- Chỉ đo \`lead_submitted\`, \`booking_confirmed\`, \`showed_up\`, \`sale_recorded\` bằng ID nội bộ/pseudonymous, chính sách phân quyền thích hợp.
- Google Business Profile nếu có địa chỉ thật và đủ điều kiện.

### CRM lead tối thiểu
ID, created_at, source/UTM, service_interest (chung), contact consent, phone, location/branch, assigned_staff, stage, next_followup_at, appointment_at, show_attended, order_value, variable_cost, reason_lost, date_closed. **Không lưu bệnh án, ảnh sức khỏe, chỉ định y khoa vào CRM marketing** nếu không có cơ sở pháp lý, quản trị và hệ thống phù hợp.

Stage: New → Contacted → Qualified for consultation → Appointment requested → Appointment confirmed → Attended → Medical consultation/screening (chỉ tag trạng thái, không lưu chẩn đoán) → Purchased / Not suitable / Lost → Aftercare / Referral. B2B dùng funnel riêng: New → Fit verified → Demo → Proposal → Negotiation → Won/Lost.

## 2. Khung test quảng cáo B2C
**Gate:** chỉ chạy dịch vụ được phép + claim đã duyệt. Tháng đầu tối đa 2–3 angle với 2 creative/angle, tránh quá nhiều adset không đủ mẫu.
- **Angle A: Minh bạch kỹ thuật** — video giải thích plasma lạnh vs plasma pen, điều kiện lựa chọn; landing FAQ; không nhắm trực diện đặc điểm ngoại hình của người xem.
- **Angle B: Con người & quy trình** — gặp chuyên gia, tiêu chí sàng lọc, lịch tư vấn; chỉ nói đúng cơ sở đã xác minh.
- **Angle C: Minh bạch chi phí** — cách báo giá và chính sách, không hứa “hiệu quả ngay”.
- Google keyword idea: \`khử thâm môi [địa bàn]\`, \`trị sẹo rỗ [địa bàn]\`, \`tư vấn sẹo mụn [địa bàn]\` nếu offer phù hợp; phủ định các truy vấn \`tự làm tại nhà\`, \`miễn phí máy\`, \`hướng dẫn đốt\`, \`tìm việc\`, \`plasma vật lý\`; nên đọc query report mỗi 48–72h.
- Remarketing chỉ với điều kiện đồng ý và chính sách nền tảng; không tạo đối tượng dựa trên dữ liệu sức khỏe nhạy cảm.

**Thông điệp B2C ví dụ (chờ duyệt):** “Mỗi tình trạng da và sắc tố có thể cần phương án khác nhau. Tìm hiểu quy trình đánh giá chuyên môn, những câu hỏi cần hỏi và thông tin chi phí minh bạch trước khi lựa chọn dịch vụ tại [cơ sở đủ điều kiện].”
**Không dùng:** “Bạn đang xấu vì sẹo/môi thâm/mí sụp phải không?” hoặc cam kết chữa dứt điểm.

## 3. Khung test B2B (nếu có bán máy)
- Form: loại cơ sở, địa bàn, số cơ sở, loại giấy phép, mục đích sử dụng, ngân sách, người quyết định, thời điểm mua.
- Lead magnet: “Bộ 18 tiêu chí thẩm định một máy plasma cho phòng khám/spa”.
- Offer: cuộc trao đổi 30 phút về mô hình đầu tư có điều kiện, **không cam kết doanh thu/hoàn vốn**.
- Demo model thật, chỉ định thật, nhân sự đủ điều kiện; chụp/đăng hình có consent.
- 10 outbound chất lượng/tuần → 3–5 cuộc hội thoại đủ điều kiện → 1–2 demo; **các số này chỉ là định mức tác nghiệp nội bộ để bắt đầu, không phải thống kê conversion thị trường**.
- KPI: qualified account cost, qualified meeting, demo held, proposal rate, win rate, gross profit / signed contract, payback của đối tác từ số liệu thực.

## 4. KPI định nghĩa rõ
| Tên | Công thức | Lưu ý |
|---|---|---|
| CPL | Ad spend / # new leads hợp lệ | Đừng dùng CPL làm KPI duy nhất |
| Qualified lead rate | qualified leads / leads | “Qualified” = đồng ý tư vấn + ở địa bàn phục vụ + hiểu đúng loại dịch vụ |
| Appointment rate | confirmed bookings / qualified leads | Không gộp appointment requests |
| Show rate | attended / confirmed bookings | Có dữ liệu lịch và check-in |
| Close rate | paid orders / attended | Trừ trường hợp được chuyên môn đánh giá không phù hợp khỏi số ca sale kỳ vọng để tránh khuyến khích bán sai |
| CAC | tổng sales + marketing cost / số khách mua mới | Có thể phân tích paid-media CAC riêng |
| AOV | doanh thu / số đơn | Ghi số lần thực hiện và hoàn/hoãn |
| Contribution | doanh thu thuần – chi phí biến đổi – hoàn/refund – paid ads | Chưa gồm fixed overhead |
| ROAS | doanh thu gán nguồn ads / ad spend | Chỉ số phụ, không đại diện lợi nhuận |
| Review/referral | số giới thiệu đã consent / tổng khách hợp lệ | Không trả tiền đổi 5 sao |

## 5. Ví dụ mô phỏng kinh tế — **HOÀN TOÀN GIẢ ĐỊNH**, dùng để hiểu phép tính
Tháng B2C spend quảng cáo 15 triệu. Giả định 150 lead (CPL = 100k) → 90 qualified (60%) → 45 booked (50%) → 34 attended (~75%) → 12 paid (~35% của attended). **Paid-media CAC = ~1,25 triệu/khách** (chưa gồm chi phí team/sản xuất). Nếu AOV 3,5tr và biến phí 35% (giả định), đóng góp gộp trước ads mỗi khách = 2,275tr → 12 khách tạo ~27,3tr trước ads → sau 15tr ads còn **~12,3tr** để trả chi phí cố định/sản xuất/thuế, chưa phải lợi nhuận ròng. 

**Tất cả đầu vào đều chưa được kiểm chứng** và có thể khác rất nhiều trong thực tế. Không coi đây là KPI dự báo hay bằng chứng ROI.

Quy tắc kinh tế: **CAC toàn phần < gross contribution/customer + contribution from legitimate repeat purchases - risk reserve**; đo theo cohort và phản ánh chi phí khám/tái hẹn. Không bán liệu trình không cần thiết để tăng LTV.

## 6. Khi nào scale / stop?
- Gate 0: pháp lý, giấy phép, chuyên môn, chứng cứ model **PASS**.
- Gate 1: tracking lead + booking + payment tin cậy; nếu mismatch >10%, sửa tracking trước.
- Gate 2: ít nhất 2 tuần / đủ mẫu thực để so sánh; đọc thêm phản hồi tiêu cực, refund, khiếu nại.
- Gate 3: contribution sau ads dương, tỷ lệ tư vấn không phù hợp được ghi nhận, CSKH có công suất.
- Sau đó tăng ngân sách từng bước **20–30%/chu kỳ đánh giá**, kiểm tra CAC và chỉ số chất lượng. Nếu CAC xấu hoặc tín hiệu rủi ro tăng thì ngừng mở rộng.

## 7. Checklist triển khai công nghệ trong tuần 1
- [ ] Mã dịch vụ/offer có nhãn \`approved_for_ads\`, ngày phê duyệt, người duyệt.
- [ ] Trang chính sách bảo mật, checkbox liên hệ đúng mục đích.
- [ ] CRM mobile-friendly, phân quyền sales vs chuyên môn.
- [ ] Template inbox “chưa thể tư vấn chỉ định y tế qua chat”, chuyển tiếp hợp lý.
- [ ] 3 event conversion, UTM, dashboard CAC, staff SLA.
- [ ] SLA mục tiêu nội bộ: phản hồi trong giờ làm việc nhanh nhất có thể, đánh giá bằng số liệu thực; không thông báo nhắc hẹn quá mức.
- [ ] Báo cáo hàng tuần theo nguồn và nhóm dịch vụ; nguồn marketing rõ và không lưu thông tin bệnh lý cá nhân vào nền tảng quảng cáo.

## 8. Báo cáo tuần mẫu
\`Week | Campaign | Spend | Impressions | CTR | Leads | Qualified | Booked | Attended | Paid | Revenue | Variable Cost | CAC | Contribution after Ads | Refund | Complaints | Action\`

**Không tự điền số khi chưa có dữ liệu.** Tất cả KPI target chính thức chỉ chốt sau tuần 2–4 nghiên cứu/pilot.

[Xem kế hoạch 90 ngày](01-ke-hoach-marketing-90-ngay.md) · [Nội dung 30 ngày](02-lich-noi-dung-30-ngay.md).
