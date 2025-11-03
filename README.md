# code
Thuật toán Leo đồi được mô phỏng dựa theo các bước:
  Khởi tạo ngẫu nhiên vị trí N quân hậu trên bàn.
  Tính giá trị hàm đánh giá H (số cặp tấn công nhau).
  Tìm hàng xóm tốt nhất – tức là trạng thái có H nhỏ hơn hiện tại.
  Nếu có hàng xóm tốt hơn, di chuyển đến đó và lặp lại bước 2.
  Nếu không có hàng xóm tốt hơn → thuật toán bị kẹt.
    Có thể khởi động lại (Random Restart)
    Hoặc thực hiện bước đi ngẫu nhiên để thoát khỏi cực trị địa phương.
  Lặp lại cho đến khi tìm thấy H = 0, tức là lời giải hợp lệ.

Các chức năng nâng cao trong chương trình
  Tự động chạy (AutoRun)
    Thuật toán được thực thi liên tục, cập nhật giao diện theo thời gian thực.
    Có thể tạm dừng hoặc điều chỉnh tốc độ chạy bằng thanh trượt.
  Tua lại / Tua đi
    Lưu lịch sử trạng thái trong danh sách history[], cho phép người dùng quay lại bước trước hoặc xem lại quá trình leo đồi.
  Chiến lược khi bị kẹt (AutoStuckStrategy)
    Restart: Khởi động lại từ trạng thái ngẫu nhiên mới.
    RandomMove: Di chuyển ngẫu nhiên một quân hậu để thoát khỏi cực trị địa phương.
  Giao diện minh họa bàn cờ
    Bàn cờ được hiển thị bằng lưới (Grid CSS).
    Các ô có màu xen kẽ sáng/tối giống bàn cờ thật.
    Quân hậu hiển thị bằng biểu tượng “♕”.
