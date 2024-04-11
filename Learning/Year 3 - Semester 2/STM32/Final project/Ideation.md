# Thiết bị định vị
---
## Hệ thống định vị (gọi chung là GNSS - Global Navigation Stateline System)
- **GPS** (General Positioning System): Hệ thống định vị toàn cầu, được Mỹ phát triển với khoảng hơn 30 vệ tinh đang hoạt động.
	> Đây sẽ là hệ thống định vị chính được sử dụng trong dự án lần này.
	
- GLONASS (Nga)
- Beidou (Trung Quốc)
- Galileo (EU)

## Các thành phần của GPS
Gồm có 3 thành phần chính:
- Phần không gian: Bao gồm các vệ tinh hoạt động trên 6 mặt phẳng quỹ đạo.
- Phần kiểm soát: Có chức năng đảm bảo vệ tinh di chuyển đúng quỹ đạo và truyền nhận thông tin chính xác.
- Các thiết bị nhận tín hiệu vệ tinh được người dùng sử dụng, được tích hợp các thuật toán ước tính và hoàn thiện kết quả đầu ra một cách chính xác.

## Cách thức hoạt động của GPS
Thiết bị nhận sẽ tính toán được khoảng thời gian kể từ khi vệ tinh bắt đầu phát tín hiệu cho đến khi nhận được tín hiệu, từ đó tính toán được độ dài quãng đường truyền nhận. 
Từ mỗi vệ tinh, ta vẽ được đường tròn tập hợp các điểm với khoảng cách đến vệ tinh là bằng nhau. Với 3 vệ tinh sẽ dễ dàng xác định được kinh độ và vĩ độ của thiết bị.
![[Pasted image 20240412002628.png]]