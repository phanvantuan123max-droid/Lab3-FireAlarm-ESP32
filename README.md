# Lab3 - Đề 3 : Hệ thống báo cháy gia đình (khí Gas và nhiệt độ )
He thong canh bao chay gia dinh su dung ESP32 FreeRTOS MQTT

Sinh viên : Phan Văn Tuấn 

Mã sinh viên : 231432386

Lớp : Kỹ sư KTĐTVT - chuyên nghành KT Viễn thông (N01)

# link wokwi: https://wokwi.com/projects/480311296032210945

# link báo cáo : https://1drv.ms/w/c/e7b270d7fc49c93a/IQAFDKgQNhT_T4lbkEHLjvmlAepdCWbOFJ5qGmG6iO7JUfc?e=yS8Omg

# link web : https://phanvantuan123max-droid.github.io/fire-alarm2/

# Mô Tả 
ESP32 sử dụng cảm biến khí gas MQ-2 và cảm biến nhiệt độ DS18B20 để giám sát nguy cơ cháy. Hệ thống tự động bật quạt hút khi nồng độ khí gas vượt ngưỡng 2000 và bật máy bơm khi nhiệt độ vượt 50°C. Dữ liệu cảm biến được gửi lên MQTT Broker (broker.hivemq.com). Website hiển thị thông số, 2 biểu đồ real-time và hỗ trợ điều khiển quạt, máy bơm bằng các nút ON/OFF/AUTO.

Hệ thống sử dụng FreeRTOS với 3 Task (đọc dữ liệu và xử lý cảnh báo chạy trên Core 1; truyền dữ liệu chạy trên Core 0) cùng 2 hàng đợi dataQueue và dataAlert để trao đổi dữ liệu giữa các Task.




