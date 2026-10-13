# BÀI LÀM: CHỌN CÁCH DỰ BÁO PHẠM VI CHO SPRINT 6 – RIKKEIGO

## Phần 1 – Đề xuất 2 cách dự báo phạm vi Sprint 6

### 1.1. Phân tích dữ liệu đầu vào

Velocity của 5 Sprint gần nhất là: 18, 20, 19, 15, 13 SP.

Average Velocity:

18+20+19+15+135=17 SP\frac{18+20+19+15+13}{5}=17\text{ SP}518+20+19+15+13=17 SP

Velocity Range:

* Velocity thấp nhất: 13 SP.

* Velocity cao nhất: 20 SP.

* Khoảng Velocity lịch sử: 13–20 SP.

Thay đổi Capacity:

212−186212×100%≈12,26%\frac{212-186}{212}\times100\%\approx12,26\%212212−186×100%≈12,26%

Capacity Sprint 6 giảm 26 giờ, tương đương khoảng 12,26% so với Sprint 5. Tuy nhiên, không thể kết luận Velocity Sprint 6 sẽ giảm đúng 12,26%, vì còn phụ thuộc vào nhân sự mới, độ phức tạp và mức độ rõ ràng của các PBI.

### 1.2. Cách 1 – Dự báo dựa trên Average Velocity

Nguyên tắc: Sử dụng Velocity trung bình trong quá khứ làm mốc tham khảo để dự báo phạm vi Sprint tiếp theo.

* Average Velocity: 17 SP.

* Dự báo Sprint 6: khoảng 17 SP.

* Danh sách PBI dự kiến:

| Thứ tự | PBI                        | SP    |
| ------ | -------------------------- | ----- |
| 1      | Hẹn giờ đặt xe trước       | 5     |
| 2      | Gửi SMS khi tài xế sắp đến | 3     |
| 3      | Chat với tài xế            | 5     |
| 4      | Giao diện chủ đề Tết       | 2     |
|        | Tổng                       | 15 SP |

Đội chọn 4 PBI có Acceptance Criteria đầy đủ hoặc có điều kiện triển khai rõ ràng. Tổng phạm vi là 15 SP, thấp hơn mốc Average Velocity 17 SP.

Lý do không cố chọn đủ 17 SP: PBI “Theo dõi vị trí tài xế trên bản đồ” có 13 SP nhưng chưa có Acceptance Criteria cho trường hợp mất tín hiệu GPS. Ngoài ra, Sprint 6 có nhân sự mới chưa quen dự án, nên không nên lấy Average Velocity làm cam kết cứng.

### 1.3. Cách 2 – Dự báo dựa trên Capacity và điều kiện thực tế

Nguyên tắc: Lấy Capacity Sprint 6, tình trạng nhân sự, độ sẵn sàng của PBI và Sprint Goal làm cơ sở chính; Velocity lịch sử chỉ là dữ liệu tham khảo.

Sprint 6 có 186 giờ, giảm so với 212 giờ ở Sprint 5. Minh chỉ dành khoảng một nửa thời gian cho công việc Sprint do đang làm quen dự án. Hà nghỉ phép 3 ngày, và ảnh hưởng này đã được tính vào Capacity 186 giờ.

Dự báo ban đầu: 15 SP, với danh sách PBI:

| Thứ tự | PBI                        | SP    | Lý do chọn                 |
| ------ | -------------------------- | ----- | -------------------------- |
| 1      | Hẹn giờ đặt xe trước       | 5     | Acceptance Criteria đầy đủ |
| 2      | Gửi SMS khi tài xế sắp đến | 3     | Hợp đồng SMS đã ký         |
| 3      | Chat với tài xế            | 5     | Acceptance Criteria đầy đủ |
| 4      | Giao diện chủ đề Tết       | 2     | Acceptance Criteria đầy đủ |
|        | Tổng                       | 15 SP |                            |

Cách này không lấy Capacity giảm 12,26% để tính máy móc ra Velocity mới. Thay vào đó, Developers sử dụng Capacity để xem xét khối lượng công việc thực tế, đồng thời ưu tiên những PBI đã đủ rõ ràng để có khả năng hoàn thành trong Sprint.

Lưu ý: 15 SP vẫn là dự báo ban đầu, không phải kết quả chắc chắn. Developers cần đánh giá thêm công sức, phụ thuộc kỹ thuật và khả năng hoàn thành từng PBI trong Sprint Planning.

## Phần 2 – So sánh hai cách dự báo

| Tiêu chí                        | Cách 1: Average Velocity                                                                                         | Cách 2: Capacity và điều kiện thực tế                                                                      |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| Phản ánh thay đổi Capacity      | (–) Average Velocity dựa trên dữ liệu quá khứ, chưa trực tiếp phản ánh việc Capacity giảm và Minh mới vào dự án. | (+) Xem xét trực tiếp Capacity 186 giờ, thời gian làm quen của Minh và các điều kiện thực tế.              |
| Bảo vệ Sprint Goal              | (+) Có thể bảo vệ Sprint Goal nếu chọn PBI phù hợp; không cần ép đủ 17 SP.                                       | (+) Bắt đầu từ Sprint Goal, sau đó chọn PBI có giá trị và đủ rõ ràng để tăng khả năng hoàn thành mục tiêu. |
| Dễ giải thích với Product Owner | (+) Dễ giải thích bằng số liệu lịch sử và phép tính Average Velocity.                                            | (–) Cần giải thích thêm về Capacity, mức độ sẵn sàng của PBI và những bất định của Sprint.                 |

Nhận xét: Cả hai cách đều có thể đưa ra dự báo hợp lý. Tuy nhiên, trong bối cảnh Sprint 6 có thay đổi nhân sự và Capacity, cách 2 phù hợp hơn vì phản ánh tình hình hiện tại thay vì dựa chủ yếu vào kết quả quá khứ.

## Phần 3 – Lựa chọn phương án và chuẩn bị Sprint Planning

### 3.1. Lựa chọn cách dự báo

Tôi chọn Cách 2 – Dự báo dựa trên Capacity và điều kiện thực tế.

Lý do:

* Capacity Sprint 6 giảm từ 212 giờ xuống 186 giờ.

* Minh cần thời gian làm quen với dự án, nên năng suất thực tế có thể khác đội hình Sprint trước.

* PBI “Theo dõi vị trí tài xế trên bản đồ” chưa đủ Acceptance Criteria cho trường hợp mất tín hiệu GPS, do đó chưa nên đưa vào Sprint khi chưa làm rõ.

* Dự báo phải hướng đến khả năng hoàn thành Sprint Goal, không phải cố đạt một con số Velocity nhất định.

### 3.2. Sprint Goal đề xuất

> Giúp khách hàng chủ động hơn khi chờ tài xế thông qua việc đặt xe trước và nhận thông báo SMS khi tài xế sắp đến.

Sprint Goal này có giá trị nghiệp vụ cụ thể, tập trung vào khả năng chủ động của khách hàng và phù hợp với những PBI đã đủ điều kiện triển khai.

### 3.3. Danh sách PBI đề xuất mang vào Sprint Planning

| Thứ tự | PBI                        | SP    | Mức ưu tiên trong Sprint                          |
| ------ | -------------------------- | ----- | ------------------------------------------------- |
| 1      | Hẹn giờ đặt xe trước       | 5     | Ưu tiên cao                                       |
| 2      | Gửi SMS khi tài xế sắp đến | 3     | Ưu tiên cao                                       |
| 3      | Chat với tài xế            | 5     | Có thể xem xét nếu hỗ trợ mục tiêu và đủ Capacity |
| 4      | Giao diện chủ đề Tết       | 2     | Ưu tiên thấp hơn Sprint Goal                      |
|        | Tổng dự báo                | 15 SP |                                                   |

Điểm cần lưu ý: Khi Sprint Goal đã xác định, PBI Chat và Giao diện chủ đề Tết không trực tiếp phục vụ mục tiêu bằng hai PBI đầu tiên. Vì vậy, trong Sprint Planning, Developers và Product Owner nên xem xét lại việc đưa hai PBI này vào Sprint. Nếu muốn ưu tiên chặt chẽ Sprint Goal hơn, có thể chọn hai PBI chính với tổng 8 SP, sau đó chỉ bổ sung PBI khác khi có lý do nghiệp vụ phù hợp và đội đánh giá có đủ Capacity.

PBI “Theo dõi vị trí tài xế trên bản đồ” chưa được chọn vì thiếu Acceptance Criteria cho trường hợp mất GPS. Product Owner cần làm rõ hành vi hệ thống khi mất tín hiệu, cách thông báo cho khách hàng và điều kiện khôi phục theo dõi trước khi PBI được đưa vào Sprint.

### 3.4. Phản hồi đề nghị nhận 20 SP của quản lý

Bài viết

Velocity 20 SP nằm trong khoảng Velocity lịch sử của đội, nhưng điều đó không có nghĩa Sprint 6 chắc chắn có thể hoàn thành 20 SP. Capacity hiện chỉ còn 186 giờ, đồng thời Minh cần thời gian làm quen dự án và một PBI lớn vẫn chưa đủ Acceptance Criteria. Vì vậy, chúng tôi đề xuất dự báo dựa trên Capacity, Sprint Goal và mức độ sẵn sàng của PBI; Velocity được dùng để tham khảo và cải thiện dự báo, không phải KPI hay chỉ tiêu bắt buộc phải tăng.

## Kết luận

Phương án phù hợp nhất là dự báo dựa trên Capacity và điều kiện thực tế, sử dụng Velocity lịch sử làm dữ liệu tham khảo. Đội không nên cố đạt 20 SP chỉ để làm Velocity tăng trở lại; điều quan trọng là chọn phạm vi phù hợp, hoàn thành các PBI đạt Definition of Done và tạo ra giá trị cho khách hàng trong Sprint 6.
