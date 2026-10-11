1. Phân tích lỗi
Dòng lệnh gây lỗi : const basePrice = bookingReservation.priceKey;
Vì nếu dùng Dot Notation chỉ tìm được các thuộc tính có trong object đó , nhưng bookingReservation không có thuộc tính đó nên sẽ nhận về giá trị là undefined

2. Test case
TestCase 1 : Nhận phòng sớm 
Dữ liệu đầu vào : roomPrice = 1500000, checkInHour = 9
Kết quả sai thực tế : basePrice = undefined, phụ thu và tổng tiền là NaN
Kết quả đúng mong đợi : Phụ thu: 450000, tổng tiền: 1950000

TestCase 2 : Nhận phòng sau 12h
Dữ liệu đầu vào : roomPrice = 1500000, checkInHour = 14
Kết quả sai thực tế : basePrice = undefined, tổng tiền là NaN
Kết quả đúng mong đợi : Phụ thu: 0, tổng tiền: 1500000