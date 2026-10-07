# Hướng dẫn hoàn chỉnh — Lab 21: Phân tích rủi ro AI qua case study thực tế

> **Track 1 — Bài cá nhân**
> Thời gian gợi ý: 120 phút (hạn nộp theo thông báo của giảng viên hoặc hệ thống lớp)

---

## Mục lục

1. [Hiểu bài lab và chuẩn bị](#1-hiểu-bài-lab-và-chuẩn-bị)
2. [Tạo repo GitHub cá nhân và đặt tên đúng](#2-tạo-repo-github-cá-nhân-và-đặt-tên-đúng)
3. [Tạo file báo cáo từ mẫu](#3-tạo-file-báo-cáo-từ-mẫu)
4. [Chọn một ngành, điền Risk Snapshot và tìm 2–3 case thật](#4-chọn-một-ngành-điền-risk-snapshot-và-tìm-23-case-thật)
5. [Điền Harm Map cho từng case](#5-điền-harm-map-cho-từng-case)
6. [Kiểm tra repo và nộp link bài làm](#6-kiểm-tra-repo-và-nộp-link-bài-làm)

---

## Tổng quan bài lab

**Bạn cần làm gì?**
- Chọn **một ngành** từ danh sách cho sẵn.
- Điền **Industry Risk Snapshot** cho ngành đó.
- Tìm và phân tích **2–3 case study AI có thật** trong cùng ngành.
- Với mỗi case: viết **Brief Case** (có số liệu + nguồn) và điền **Harm Map Worksheet**.
- Nộp repo GitHub cá nhân.

**Bài nộp cần có:**

| Phần bài làm | Bạn cần hoàn thành |
| --- | --- |
| Industry Risk Snapshot | Đánh giá nhanh ngành: tác hại chính, mức độ high-stakes, dữ liệu nhạy cảm và nhu cầu người kiểm tra |
| Brief Case | 2–3 case AI có thật trong cùng ngành, mỗi case có mô tả, số liệu và nguồn |
| Harm Map Worksheet | Một bảng phân tích cho mỗi case (đủ 11 trường) |

**Sau bài này bạn làm được:**
- Đánh giá nhanh rủi ro của một ngành bằng Industry Risk Snapshot.
- Viết Brief Case có số liệu và nguồn cho 2–3 case AI có thật trong cùng ngành.
- Điền Harm Map Worksheet cho từng case, phân biệt sự kiện có nguồn với nhận định cá nhân.
- Lưu báo cáo cá nhân vào repo GitHub đúng quy ước và nộp link truy cập được.

---

## 1. Hiểu bài lab và chuẩn bị

### Cần chuẩn bị trước

- Đã đọc slide **AI Ethics, AI Safety, Responsible AI** và **Luật AI tại Việt Nam**.
- Có **tài khoản GitHub cá nhân**.
- Có **trình duyệt web**.
- Có **tài khoản học tập** của lớp để nộp bài.

### Nguồn tham khảo trong slide

- **Yêu cầu bài cá nhân**: mục *Cá nhân* của trang 31 — Lab Assignment trong slide AI Ethics, AI Safety và Responsible AI.
- **Mẫu phân tích Harm Map**: trang 22–25; mở Harm Map Worksheet — trang 25 để đối chiếu khi điền bài.

### Ba yêu cầu cá nhân trong PDF

1. Chọn **1 ngành** từ danh sách có sẵn (xem bước 4).
2. Điền **Industry Risk Snapshot** cho ngành đó: chấm nhanh risk profile ở mức ngành để ước lượng harm chính, mức độ high-stakes, dữ liệu nhạy cảm và nhu cầu human review.
3. Tìm và phân tích **2–3 case study AI có thật** trong cùng ngành. Với mỗi case, viết Brief Case có số liệu + nguồn, rồi điền Harm Map Worksheet.

### Lỗi thường gặp (cần tránh)

| ❌ Lỗi | ✅ Cách đúng |
| --- | --- |
| Chọn case thuộc **nhiều ngành khác nhau** hoặc chỉ phân tích một case | Tất cả 2–3 case phải cùng **một** ngành |
| Có mô tả case nhưng **thiếu số liệu, nguồn hoặc Harm Map** | Mỗi case phải có đủ Brief Case (số liệu + nguồn) VÀ Harm Map |
| Ghi tác hại giả định **như một hậu quả đã xảy ra** | Phân biệt rõ hậu quả đã xảy ra vs. nguy cơ |
| Sửa README nhưng **chưa Commit** hoặc **chưa nộp link** | Phải Commit changes VÀ nộp link trên hệ thống |

### Thuật ngữ cần hiểu

| Thuật ngữ | Hiểu đơn giản | Bạn sẽ ghi gì? |
| --- | --- | --- |
| Repo / repository | Thư mục bài làm được lưu trên GitHub | Repo thuộc tài khoản cá nhân của bạn |
| Commit | Lưu một phiên bản thay đổi lên GitHub | Bấm *Commit changes* sau khi sửa báo cáo |
| Brief Case | Tóm tắt một trường hợp AI có thật | Hệ thống nào, dùng để làm gì, vấn đề gì, số liệu và nguồn |
| High-stakes | Quyết định có thể ảnh hưởng lớn đến sức khỏe, quyền lợi hoặc cơ hội của một người | Giải thích điều gì khiến ngành có mức tác động lớn |
| Failure mode | Kiểu AI mắc lỗi | Ví dụ: bịa thông tin, thiên lệch, lộ dữ liệu |
| Layer | Lớp trong hệ thống nơi lỗi bắt đầu | UX, Grounding, Safety hoặc Model |
| Harm | Hậu quả cụ thể đối với người hoặc tổ chức | Ai bị ảnh hưởng và mất gì hoặc chịu thiệt hại gì |
| Human review / human-in-the-loop | Có người kiểm tra hoặc can thiệp ở bước cần thiết | Ai nên kiểm tra và kiểm tra ở thời điểm nào |

> ✅ **Hoàn thành bước 1 khi:** bạn hiểu ba yêu cầu cá nhân và biết bài được lưu trong repo của mình.

---

## 2. Tạo repo GitHub cá nhân và đặt tên đúng

### Quy ước đặt tên repo

```
DAY21_Track1_MSSV_HoVaTen
```

| Thành phần | Cách điền |
| --- | --- |
| `DAY21` | Giữ nguyên, viết hoa |
| `Track1` | Giữ nguyên cách viết `Track1` |
| `MSSV` | Thay bằng mã học viên / mã sinh viên của bạn |
| `HoVaTen` | Họ tên viết liền, không dấu, không khoảng trắng |
| Dấu phân cách | Dùng dấu gạch dưới `_` giữa bốn phần |

**Ví dụ:**
```
DAY21_Track1_21001234_NguyenVanAn
```

### Các bước tạo repo

1. Đăng nhập GitHub và mở [trang tạo repo mới](https://github.com/new).
2. Chọn **Owner** là tài khoản cá nhân; nhập **Repository name** theo quy tắc trên.
3. Chọn **Public** để giảng viên mở được bài. Bật **Add a README file**.
4. Bấm **Create repository**.
5. Kiểm tra repo có `README.md` và URL thuộc tài khoản của bạn.

**URL sẽ có dạng:**
```
https://github.com/tai-khoan-github/DAY21_Track1_21001234_NguyenVanAn
```

> **Lưu ý:** Nếu giảng viên đã gửi starter repo cho Lab 21 → mở repo đó → bấm **Fork** → chọn tài khoản cá nhân → đặt tên bản fork theo quy tắc của lớp. Tiếp tục làm trong bản fork.

> ✅ **Hoàn thành bước 2 khi:** bạn mở được repo cá nhân, tên đúng và có file `README.md`.

---

## 3. Tạo file báo cáo từ mẫu

### Các bước thao tác

1. Trong repo, mở `README.md`, bấm biểu tượng **bút chì / Edit this file**.
2. Thay nội dung ban đầu bằng **mẫu bên dưới**.
3. Điền họ tên, MSSV, lớp và ngành đã chọn. Phần phân tích sẽ hoàn thiện ở bước 4–5.
4. Bấm **Preview** để xem bảng; bấm **Commit changes**, nhập mô tả (ví dụ: `Tao khung bao cao Lab 21`), chọn lưu trực tiếp vào nhánh hiện tại rồi xác nhận **Commit changes**.
5. Mở lại `README.md`, kiểm tra nội dung vừa lưu đã xuất hiện.

### Mẫu README.md

```markdown
# Lab 21 — Phân tích rủi ro AI qua case study thực tế

- Họ và tên: [Điền họ tên]
- MSSV / mã học viên: [Điền mã]
- Lớp: [Điền lớp]
- Ngành đã chọn: [Chọn một ngành theo đề]

### 1. Industry Risk Snapshot

| Nội dung | Đánh giá của tôi và lý do |
| --- | --- |
| Những tác hại chính có thể xảy ra | [Điền tác hại và người bị ảnh hưởng] |
| Mức độ high-stakes | [Thấp / Trung bình / Cao; giải thích] |
| Dữ liệu nhạy cảm có thể được sử dụng | [Nêu loại dữ liệu, không đưa dữ liệu thật vào bài] |
| Nhu cầu human review | [Thấp / Trung bình / Cao; ai kiểm tra, ở bước nào, vì sao] |

### 2. Case study 1 — [Tên case]

#### Brief Case

- Tổ chức / sản phẩm AI: [Điền]
- Thời gian, địa điểm / bối cảnh: [Điền]
- AI được dùng để làm gì: [Điền]
- Vấn đề hoặc sự kiện đáng chú ý: [Điền sự kiện có nguồn]
- Số liệu có nguồn: [Con số, đơn vị, thời gian/phạm vi đo và nguồn nào cung cấp]
- Nguồn: [Tên tài liệu/bài viết — đơn vị/tác giả — ngày công bố — URL — trang/mục liên quan nếu có]
- Phân biệt bằng chứng và nhận định: [Điều nguồn xác nhận; điều tôi suy luận hoặc còn chưa rõ]

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | [Tình huống cụ thể có rủi ro] |
| Stakeholder bị ảnh hưởng | [Người dùng và các bên liên quan] |
| Failure mode | [Kiểu lỗi AI] |
| Layer bắt đầu lỗi | [UX / Grounding / Safety / Model; giải thích hoặc ghi chưa đủ bằng chứng] |
| Harm xảy ra là gì? | [Ai bị ảnh hưởng + hậu quả; ghi rõ đã xảy ra hay mới là nguy cơ] |
| Harm lens | [Loại tác hại] |
| Severity | [Low / Medium / High / Critical] |
| Scale | [Quy mô tác động và căn cứ] |
| Probability | [Khả năng xảy ra và căn cứ] |
| Frequency | [Tần suất và căn cứ] |
| Vì sao? | [Lý do cho các đánh giá; nguồn hoặc giới hạn bằng chứng] |

### 3. Case study 2 — [Tên case]

#### Brief Case

- Tổ chức / sản phẩm AI: [Điền]
- Thời gian, địa điểm / bối cảnh: [Điền]
- AI được dùng để làm gì: [Điền]
- Vấn đề hoặc sự kiện đáng chú ý: [Điền sự kiện có nguồn]
- Số liệu có nguồn: [Con số, đơn vị, thời gian/phạm vi đo và nguồn nào cung cấp]
- Nguồn: [Tên tài liệu/bài viết — đơn vị/tác giả — ngày công bố — URL — trang/mục liên quan nếu có]
- Phân biệt bằng chứng và nhận định: [Điều nguồn xác nhận; điều tôi suy luận hoặc còn chưa rõ]

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| High-risk moment | [Điền] |
| Stakeholder bị ảnh hưởng | [Điền] |
| Failure mode | [Điền] |
| Layer bắt đầu lỗi | [Điền] |
| Harm xảy ra là gì? | [Điền; phân biệt hậu quả đã xảy ra với nguy cơ] |
| Harm lens | [Điền] |
| Severity | [Điền] |
| Scale | [Điền] |
| Probability | [Điền] |
| Frequency | [Điền] |
| Vì sao? | [Điền căn cứ và giới hạn bằng chứng] |
```

> **Lưu ý:** Mẫu có sẵn 2 case (số tối thiểu). Nếu làm 3 case, sao chép cả phần Brief Case và Harm Map của case 2 xuống cuối; đổi tiêu đề thành `### 4. Case study 3 — [Tên case]` rồi điền case thứ ba.

> ✅ **Hoàn thành bước 3 khi:** `README.md` đã lưu trên GitHub, có thông tin cá nhân và đủ khung bài làm.

---

## 4. Chọn một ngành, điền Risk Snapshot và tìm 2–3 case thật

### Danh sách ngành được chọn

| Ngành | Phạm vi gợi ý |
| --- | --- |
| HR / tuyển dụng | AI sàng lọc CV, đánh giá hoặc hỗ trợ tuyển ứng viên |
| Giáo dục / AI tutor | AI hỗ trợ học tập, hướng dẫn người học |
| Y tế / symptom checker / health assistant | AI kiểm tra triệu chứng, trợ lý sức khỏe |
| Mobility / autonomous driving | AI trong di chuyển, xe tự hành |
| Media / news / social / political assistant | AI trong tin tức, mạng xã hội, trợ lý chính trị |
| Content creator | AI hỗ trợ tạo nội dung |

### Các bước thực hiện

1. **Chọn ngành** bạn hiểu hoặc quan tâm; ghi vào đầu `README.md`.
2. **Điền Industry Risk Snapshot** theo bốn nội dung:
   - Tác hại chính (harm chính)
   - Mức độ high-stakes
   - Dữ liệu nhạy cảm
   - Nhu cầu human review
   - → Mỗi đánh giá **viết kèm lý do ngắn**.
3. **Tìm 2–3 case** khác nhau trong cùng ngành đó. Gợi ý từ khóa tìm kiếm:
   - `AI hiring bias case study`
   - `AI tutor incident study`
   - `health chatbot safety study`
   - Hoặc cụm tương ứng với ngành bạn chọn.
4. **Mở và đọc nguồn gốc**, ghi lại số liệu và URL; điền Brief Case cho từng case rồi lưu bằng **Commit changes**.

> **Lưu ý:** Thấp / Trung bình / Cao trong Risk Snapshot là đánh giá định tính phục vụ bài tập. Hãy giải thích căn cứ; không dùng nhãn này như kết luận phân loại pháp lý.

### Làm sao biết một case đủ để phân tích?

- ✅ Có **tên tổ chức, sản phẩm hoặc nghiên cứu** cụ thể và bối cảnh rõ ràng.
- ✅ Có **vấn đề liên quan đến rủi ro AI**, đủ thông tin để phân tích tác hại.
- ✅ Có ít nhất **một số liệu liên quan kèm nguồn** cho Brief Case. Ghi rõ số liệu đo điều gì, trong phạm vi nào.
- ✅ **Nguồn mở được** và chứa thông tin bạn viết: ưu tiên báo cáo chính thức, nghiên cứu, hồ sơ sự kiện hoặc bài báo có dẫn chứng.

**Ví dụ cách ghi số liệu:**
```
[N] trường hợp trong [tổng số M] trường hợp, tại [bối cảnh], trong [thời gian], theo [nguồn].
```

> ⚠️ Hai bài báo kể cùng một sự kiện vẫn là **một** case. Nếu case không có số liệu phù hợp, tìm thêm nguồn hoặc chọn case khác.

> ⚠️ Bạn có thể dùng AI để gợi ý từ khóa hoặc giải thích thuật ngữ. **Tự mở các nguồn** mà AI đề xuất, đối chiếu con số và trích dẫn trước khi đưa vào bài. Khi nguồn chỉ xác nhận một lỗi mà chưa xác nhận thiệt hại, ghi rõ tác hại bạn phân tích là **nguy cơ có thể xảy ra**.

> ✅ **Hoàn thành bước 4 khi:** có một Risk Snapshot và 2–3 Brief Case cùng ngành, mỗi case có số liệu và nguồn kiểm tra được.

---

## 5. Điền Harm Map cho từng case

Với mỗi case, chọn một tình huống rủi ro cụ thể rồi đi theo luồng của slide:

```
Moment → Mode → Layer → Harm → Severity
```

Sau đó bổ sung: stakeholder, harm lens, scale, probability, frequency và lý do để đủ worksheet.

### Bảng tra cứu: Failure Mode (Slide trang 22 — AI có thể sai & gây hại theo những cách nào?)

| Failure mode | AI sai kiểu gì? | Hay xảy ra khi nào? | Nên kiểm tra ở đâu? |
| --- | --- | --- | --- |
| **Hallucination** (bịa thông tin) | AI bịa fact, policy, số liệu, link, deadline nhưng nói rất tự tin | Thiếu dữ liệu chuẩn, thiếu grounding/RAG, hồi ca ngoại lệ | Grounding, nguồn dữ liệu, UX nhắc kiểm tra, chuyển người thật |
| **Bias / fairness** (thiên lệch) | AI cho kết quả lệch giữa các nhóm người, hoặc "có vẻ công bằng" theo kiểu này nhưng lại bất công theo kiểu khác | Dữ liệu lệch, dùng biến proxy, chọn ngưỡng quyết định không hợp lý | Dữ liệu, model, ngưỡng quyết định, review chính sách |
| **Sycophancy** (chiều người dùng) | AI đồng ý với người dùng dù người dùng sai | Câu hỏi gợi ý mạnh, user pushback, prompt đầy cảm xúc | Model, system prompt, cách hiện bằng chứng trong UI |
| **Over-reliance** (tin AI quá mức) | Người dùng tin output như kết luận cuối cùng và ngưng kiểm tra | AI nói quá chắc, giao diện làm output trông "chính thức", không có cảnh báo độ chắc chắn | UX, uncertainty cue, monitoring sau triển khai |
| **Harmful advice** (lời khuyên gây hại) | AI đưa lời khuyên nguy hiểm trong y tế, pháp lý, tài chính, self-harm | Domain rủi ro cao, policy boundary yếu, thiếu escalation | Safety policy, boundary, human escalation |
| **Privacy leak** (rò dữ liệu) | AI lộ PII, prompt, tài liệu nội bộ, dữ liệu người khác | RAG/tool phân quyền sai, prompt injection, log sai | Quyền truy cập, RAG, tool use, audit/logging |
| **Escalation failure** (không chuyển người thật) | Đáng ra phải từ chối hoặc chuyển người thật, nhưng AI vẫn cố trả lời | Không có rule rõ, không có nút handoff, thiếu fallback | Workflow, handoff, rule, human-in-the-loop |
| **Misuse / jailbreak** (vượt rào / lạm dụng) | Người dùng ép AI làm điều bị cấm hoặc vượt guardrail | Prompt đối kháng, roleplay, tool abuse, jailbreak pattern | Guardrail, safety system, red teaming, monitoring |

### Bảng tra cứu: Layer — System Map (Slide trang 23 — Lỗi bắt đầu từ layer nào? Dùng để debug)

| Layer | Đây là lớp gì? | Câu hỏi cần nhìn | Nếu lớp này yếu thì chuyện gì xảy ra? | Ví dụ |
| --- | --- | --- | --- | --- |
| **User experience** | Lớp người dùng nhìn thấy và tương tác trực tiếp | Output có trông như "sự thật chính thức" không? Có báo độ chắc chắn không? Có nút xem nguồn, kiểm tra lại, hay gọi người thật không? | Giao diện làm AI trông quá đáng tin, nên người dùng dễ tin quá mức và bỏ qua bước kiểm tra | Bot CSKH hiện câu trả lời như quyết định chính thức, nhưng không có nhãn "tham khảo" hay nút xem chính sách gốc |
| **System message & grounding** | Lớp hướng dẫn model phải làm gì và được bám vào nguồn nào | Model có nối với nguồn chính thức không? Có rule rõ về việc chỉ trả lời trong phạm vi tài liệu được ground không? Gặp edge case có biết nói "tôi không chắc" không? | Model dễ hallucinate, trả lời ngoại phạm vi, hoặc tự tin nói những thứ không có trong nguồn chuẩn | Bot HR trả lời sai vì chính sách nghỉ phép vì không được ground vào employee handbook bản mới nhất |
| **Safety system** | Lớp guardrail để chặn, từ chối, hoặc chuyển cấp khi cần | Input nào cần chặn? Output nào cần chặn? Khi nào phải từ chối? Khi nào phải escalate sang người thật? | Hệ thống không nhận ra ca nguy hiểm hoặc nhạy cảm, và để AI tiếp tục tự xử lý khi đáng ra phải dừng hoặc chuyển người thật | Người dùng hỏi lời khuyên y tế khẩn cấp, nhưng bot vẫn trả lời tiếp thay vì chuyển bác sĩ hoặc hotline phù hợp |
| **Model** | Bản thân model đang được dùng cho bài toán | Model này có đủ năng lực cho use case đó không? Có quá yếu so với độ phức tạp của bài toán không? Có phù hợp với reasoning, safety, cost, latency không? | Có những lỗi thật sự đến từ model. Nhưng nếu đổ hết lỗi cho model, mình dễ sửa sai chỗ và bỏ qua các lớp xung quanh | Dùng model nhỏ, rẻ để đọc hợp đồng/pháp lý dài nên nó bỏ sót điều khoản quan trọng và tóm tắt sai |

> **Lưu ý:** Một case có thể liên quan nhiều mode hoặc layer. Chỉ chọn những mục bạn **giải thích được**. Nếu nguồn không đủ để xác định layer, ghi **"chưa đủ bằng chứng"** và nêu giả thuyết riêng; không khẳng định hệ thống dùng một kiến trúc chưa được công bố.

### Luồng phân tích Harm Map — 5 bước (Slide trang 24)

Chọn khoảnh khắc rủi ro → gọi tên kiểu lỗi → tìm lớp bắt đầu lỗi → viết hậu quả thực tế → chấm mức độ

| Bước | Chọn / ghi gì | Label nên dùng | Ví dụ |
| --- | --- | --- | --- |
| **MOMENT** — Chọn high-risk moment | Khoảnh khắc AI tham gia quyết định, hướng cần, ngoại lệ, hoặc tình huống nhạy cảm. Không có nhãn cố định — chỉ cần 1 tình huống cụ thể. | *(mô tả tình huống)* | User hỏi bot CSKH: "Tôi có được hoàn về trong trường hợp ngoại lệ này không?" |
| **MODE** — Gọi tên failure mode | Xác định: nếu AI sai, sẽ sai theo kiểu gì? | Hallucination · Bias-fairness · Sycophancy · Over-reliance · Harmful advice · Privacy leak · Escalation failure · Misuse-jailbreak | *(chọn 1 hoặc nhiều mode phù hợp)* |
| **LAYER** — Tìm layer bắt đầu lỗi | Debug: lỗi khởi phát từ lớp nào trong hệ thống? | UX · Grounding · Safety · Model | *(chọn 1 hoặc nhiều layer, nối bằng "+")* |
| **HARM** — Viết harm cụ thể | Mẫu: **Ai bị ảnh hưởng + chuyện gì xảy ra**. Không chỉ khách hàng trực tiếp, mà cả **non-customer stakeholders**. | Misinformation · Opportunity loss · Injury · Privacy loss · Dignity loss | User tin thông tin sai, đổi/hoàn về sai điều kiện, mất tiền; đội CSKH phát sinh khiếu nại |
| **SEVERITY** — Chấm mức độ nghiêm trọng | Ưu tiên mức xử lý cần thiết. | Low · Medium · High · Critical | *(chọn 1 mức)* |

> **Lưu ý quan trọng từ slide:** Ở bước HARM, cần xem cả non-customer stakeholders (ứng viên, người thân, nhân viên vận hành, cộng đồng...), không chỉ khách hàng trực tiếp. Grounding = system message & grounding data.

---

### Ví dụ minh hoạ từ slide trang 24

#### Ví dụ 1 — Health Chatbot

| Bước | Phân tích |
| --- | --- |
| **MOMENT** | User hỏi câu nhạy cảm về triệu chứng sức khỏe → bot trả lời như đang tư vấn y khoa. Bot CSKH không được thiết kế để tư vấn y tế. |
| **MODE** | **Harmful advice** + **Escalation failure** |
| **LAYER** | **Grounding** + **Safety**. System message không giới hạn phạm vi và không có guardrail escalation. |
| **HARM** | User làm theo lời khuyên sai, chậm đi khám; hệ thống không chuyển sang bác sĩ / kênh hỗ trợ phù hợp. Ảnh hưởng: user trực tiếp — người thân — đơn vị vận hành sản phẩm. → **Injury** |
| **SEVERITY** | **Critical**. Chậm gây hại thể chất hoặc làm chậm can thiệp y tế cần thiết. |

#### Ví dụ 2 — Hiring Screening

| Bước | Phân tích |
| --- | --- |
| **MOMENT** | Ứng viên nộp CV → hệ thống screening tự động chấm điểm và loại hồ sơ. AI quyết định ai được phỏng vấn mà không có giám sát con người. |
| **MODE** | **Bias / fairness** |
| **LAYER** | **Model** + **Grounding**. Mô hình học từ dữ liệu tuyển dụng lịch sử có bias, phân biệt không dựa trên năng lực. |
| **HARM** | Nhóm ứng viên bị bất lợi dù năng lực tương đương — mất cơ hội phỏng vấn. Ảnh hưởng: ứng viên — HR — công ty tuyển dụng (rủi ro pháp lý). → **Opportunity loss** + **Dignity loss** |
| **SEVERITY** | **High** |

---

### Harm Map Worksheet mẫu đã điền (Slide trang 25)

Đây là 4 ví dụ đã hoàn chỉnh trong slide để bạn đối chiếu cách viết:

#### Ví dụ A — Bot CSKH bịa thông tin hoàn/đổi

| Trường | Phân tích mẫu |
| --- | --- |
| High-risk moment | User hỏi bot CSKH về điều kiện hoàn/đổi trong một trường hợp ngoại lệ |
| Stakeholder bị ảnh hưởng | User trực tiếp; đội CSKH; hãng |
| Failure mode | Hallucination |
| Layer bắt đầu lỗi | Grounding + UX |
| Harm xảy ra là gì? | User tin thông tin sai, đổi/hoàn về sai điều kiện, mất tiền hoặc trễ kế hoạch; đội CSKH phát sinh khiếu nại |
| Harm lens | Misinformation / Opportunity loss |
| Severity | High |
| Scale | Medium |
| Probability | Medium |
| Frequency | Medium |
| Vì sao? | Thiệt hại tài chính có thật và ảnh hưởng trực tiếp đến quyết định của user; không phải mọi câu hỏi đều dính, nhưng edge case xuất hiện đều và dễ lặp lại |

#### Ví dụ B — Bot sức khỏe đưa lời khuyên y khoa nguy hiểm

| Trường | Phân tích mẫu |
| --- | --- |
| High-risk moment | User hỏi câu nhạy cảm về triệu chứng sức khỏe, nhưng bot trả lời như đang tư vấn y khoa |
| Stakeholder bị ảnh hưởng | User trực tiếp; người thân; đơn vị vận hành sản phẩm |
| Failure mode | Harmful advice + Escalation failure |
| Layer bắt đầu lỗi | Safety + Grounding |
| Harm xảy ra là gì? | User làm theo lời khuyên sai hoặc chậm đi khám; hệ thống không chuyển sang bác sĩ hoặc kênh hỗ trợ phù hợp |
| Harm lens | Injury |
| Severity | Critical |
| Scale | Medium |
| Probability | Medium |
| Frequency | Medium |
| Vì sao? | Nếu xảy ra thì có thể gây hại thể chất hoặc làm chậm can thiệp y tế cần thiết; không phải mọi phiên chat đều gặp, nhưng đây là loại harm phải ưu tiên chặn rất sớm |

#### Ví dụ C — Hệ thống screening tuyển dụng có bias

| Trường | Phân tích mẫu |
| --- | --- |
| High-risk moment | Ứng viên nộp CV, hệ thống screening tự động chấm điểm và loại hồ sơ |
| Stakeholder bị ảnh hưởng | Ứng viên; HR; công ty tuyển dụng |
| Failure mode | Bias / fairness |
| Layer bắt đầu lỗi | Model + Grounding |
| Harm xảy ra là gì? | Một nhóm ứng viên bị bất lợi dù năng lực tương đương; mất cơ hội phỏng vấn; công ty chịu rủi ro công bằng và pháp lý |
| Harm lens | Opportunity loss / Dignity loss |
| Severity | High |
| Scale | High |
| Probability | High |
| Frequency | High |
| Vì sao? | Nếu dữ liệu lịch sử đã lệch và hệ thống dùng ở vòng lọc đầu, tác động sẽ lặp lại trên nhiều hồ sơ và tích lũy thành bias có hệ thống |

#### Ví dụ D — Bot nội bộ rò rỉ dữ liệu nhạy cảm

| Trường | Phân tích mẫu |
| --- | --- |
| High-risk moment | User hỏi bot nội bộ về tài liệu công ty và bot lộ thông tin không nên hiển thị |
| Stakeholder bị ảnh hưởng | Nhân viên; công ty; khách hàng hoặc đối tác có dữ liệu bị lộ |
| Failure mode | Privacy leak |
| Layer bắt đầu lỗi | Grounding + Safety |
| Harm xảy ra là gì? | Lộ PII, tài liệu nội bộ, hoặc dữ liệu nhạy cảm; tăng rủi ro pháp lý, mất niềm tin, và có thể ảnh hưởng nhiều bên liên quan |
| Harm lens | Privacy loss |
| Severity | Critical |
| Scale | High |
| Probability | Medium |
| Frequency | Low |
| Vì sao? | Một lần rò dữ liệu có thể gây hậu quả lớn và khó thu hồi; không nhất thiết xảy ra thường xuyên, nhưng blast radius rất rộng nếu quyền truy cập hoặc retrieval cấu hình sai |

---

### Hướng dẫn viết từng trường Harm Map (áp dụng cho bài của bạn)

1. **High-risk moment**: nêu đúng thời điểm AI tham gia một quyết định hoặc tình huống nhạy cảm. Không có nhãn cố định — chỉ cần mô tả 1 tình huống cụ thể.
2. **Stakeholder + Harm**: viết theo mẫu **"[Ai] bị [hậu quả gì] khi [điều gì xảy ra]"**. Xem cả người dùng trực tiếp và bên liên quan khác (ứng viên, người thân, nhân viên, đơn vị vận hành...).
3. **Harm lens**: dùng loại phù hợp trong slide:
   - `misinformation` — thông tin sai
   - `opportunity loss` — mất cơ hội
   - `injury` — tổn hại thể chất
   - `privacy loss` — mất riêng tư
   - `dignity loss` — tổn hại phẩm giá
4. **Severity, Scale, Probability, Frequency**: đánh giá từng trường và giải thích căn cứ ở dòng **Vì sao?**.
5. Lưu báo cáo bằng **Commit changes**, mở lại kiểm tra mỗi case đều có đủ bảng.

### Gợi ý đánh giá nhất quán (không phải thang điểm chính thức)

| Trường | Cách đánh giá |
| --- | --- |
| **Severity** — nghiêm trọng đến đâu? | Chọn Low / Medium / High / Critical; giải thích bằng hậu quả. Critical phù hợp với nguy cơ tổn hại thể chất nghiêm trọng. |
| **Scale** — ảnh hưởng rộng đến đâu? | Nêu số người/phạm vi có nguồn; nếu chưa có số liệu, nhận định Low / Medium / High nhưng phải ghi căn cứ và giới hạn. |
| **Probability** — khả năng xảy ra? | Dùng tỷ lệ đo được nếu có; nếu chỉ nhận định Low / Medium / High, ghi rõ đây là đánh giá của bạn. |
| **Frequency** — lặp lại thường xuyên không? | Nêu tần suất có nguồn hoặc đánh giá Low / Medium / High kèm lý do. |

> ⚠️ Severity cao **không tự động** có nghĩa xác suất hoặc tần suất cao. Khi không đủ thông tin, ghi rõ **"chưa đủ dữ liệu để đánh giá"**; không tự đặt phần trăm hay số người bị ảnh hưởng.

> ✅ **Hoàn thành bước 5 khi:** mỗi case có đủ 11 trường Harm Map và bạn giải thích được vì sao đã chọn các nhãn, mức độ đó.

---

## 6. Kiểm tra repo và nộp link bài làm

### Checklist kiểm tra trước khi nộp

- [ ] Repo thuộc tài khoản cá nhân và có tên `DAY21_Track1_MSSV_HoVaTen`.
- [ ] `README.md` có họ tên, MSSV, lớp và đúng **một ngành** theo đề.
- [ ] Có **Industry Risk Snapshot** gồm: tác hại chính, high-stakes, dữ liệu nhạy cảm, human review.
- [ ] Có **2–3 case** khác nhau trong **cùng ngành**; mỗi case có Brief Case, số liệu và nguồn mở được.
- [ ] Mỗi case có **Harm Map đủ 11 trường**; đánh giá có lý do, không biến suy luận thành sự kiện.
- [ ] Đã thay hết nội dung `[Điền]` và hướng dẫn trong mẫu bằng bài làm thật.
- [ ] Đã **Commit changes**; mở lại repo thấy đúng bản báo cáo mới nhất.
- [ ] Bài dùng nguồn công khai; **không** đưa dữ liệu nhạy cảm thật, hội thoại riêng hay thông tin bệnh nhân/ứng viên vào repo Public.
- [ ] Mở link repo bằng **cửa sổ ẩn danh** (Incognito / Private) → đọc được `README.md` không cần đăng nhập → mở được các link nguồn.

### Nộp trên AI Codelabs

1. Mở [AI Codelabs](https://codelabs.vlearn.dev/), đăng nhập bằng tài khoản học tập của lớp.
2. Vào **Codelabs** → mở đúng bài **Lab 21 — Phân tích rủi ro AI qua case study thực tế**.
3. Tới phần nộp bài ở cuối Lab; chọn số sao **Đánh giá Lab này**.
4. Dán **URL repo cá nhân** vào *Link bài đã nộp*.
   ```
   https://github.com/tai-khoan-github/DAY21_Track1_21001234_NguyenVanAn
   ```
5. Bấm **Xác nhận đã nộp bài** → Trong hộp *Xác nhận gửi bài?*, kiểm tra lại link → **Gửi bài**.
6. Chờ hệ thống ghi nhận. Nếu báo lỗi, tải lại và kiểm tra lịch sử trước khi thử lại.
7. Mở **menu tài khoản → Xem hồ sơ và bài đã nộp → Lịch sử nộp bài**; kiểm tra đúng Lab, link, thời gian và trạng thái.

> ⚠️ Chỉ tạo repo hoặc bấm Commit trên GitHub **chưa hoàn tất** việc nộp; bạn cần gửi link và kiểm tra xác nhận trên AI Codelabs.

> ⚠️ Hệ thống cho tối đa **3 lần nộp** mỗi Lab. Xem dòng *Đã dùng …/3 lần nộp* trước khi gửi thêm.

### Sửa bài hoặc nộp lại

| Câu hỏi | Cách xử lý |
| --- | --- |
| Tôi chưa gửi nhưng nhập nhầm link? | Trong hộp xác nhận → **Quay lại chỉnh sửa** → sửa link → kiểm tra lại → **Gửi bài**. |
| Tôi đã gửi nhầm link? | Kiểm tra lịch sử. Nếu còn lần nộp, gửi lần mới với link đúng. Nếu hết lượt hoặc đang chấm, báo Lab Coach kèm link đúng. |
| Sửa README.md sau khi đã nộp? | Bấm Commit để lưu trên GitHub. Sửa file **không tự tạo** lần nộp mới trên AI Codelabs. Nếu cần ghi nhận bổ sung, quay lại Lab và gửi khi hệ thống còn nhận bài. |
| Có cần nộp ZIP hoặc PDF riêng không? | Theo runbook: nộp **link repo** có `README.md` đầy đủ. Chỉ bổ sung file khác nếu giảng viên yêu cầu. |

### Xử lý lỗi thường gặp khi lưu/nộp

| Bạn gặp gì? | Cách xử lý |
| --- | --- |
| GitHub báo tên repo đã tồn tại | Mở repo cùng tên trong tài khoản; tiếp tục dùng nếu đúng bài Lab 21. |
| Repo bị đặt sai tên | Vào **Settings → General → Repository name** → sửa tên → **Rename**. Sao chép URL mới để nộp. |
| Chưa có README.md | **Add file → Create new file** → đặt tên `README.md` → dán mẫu → **Commit changes**. |
| Không thấy nút bút chì chỉnh sửa | Kiểm tra đã đăng nhập GitHub và đang mở repo **của mình**; mở file `README.md` trước khi tìm nút sửa. |
| Nội dung sửa chưa xuất hiện | Kiểm tra đã xác nhận **Commit changes** → tải lại trang → mở đúng nhánh đang lưu bài. |
| Cửa sổ ẩn danh không mở được repo | Kiểm tra repo là **Public**. Nếu lớp yêu cầu Private, cấp quyền cho tài khoản giảng viên/Coach. |
| Chưa thấy Lab 21 hoặc form nộp | Giữ repo đã hoàn thiện và báo Lab Coach. |
| Hệ thống báo hết hạn / khóa nộp | Báo Lab Coach kèm link repo và thông báo lỗi. |

---

> ✅ **Hoàn thành bài Lab 21 khi:** bạn đã chọn một ngành, điền Industry Risk Snapshot, phân tích 2–3 case thật cùng ngành với Brief Case có số liệu/nguồn và Harm Map cho từng case; giảng viên mở được repo và lịch sử trên hệ thống đã ghi nhận đúng link bài của bạn.
