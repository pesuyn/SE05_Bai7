# SE05_Bai7
1.Mục tiêu: Xây dựng app quản lý khách sạn dành cho quản lý, nhân viên bán hàng,lễ tân
  -Thiết bị: Máy tính cá nhân
  -Chức năng:
    Đối với quản lý:
    +Thêm thông tin phòng
    +Sửa thông tin phòng
    +Xóa thông tin phòng
    +Xem các báo cáo doanh thu theo thời gian
    +Xem các báo cáo doanh thu theo phòng
    +Xem các báo cáo doanh thu theo loại phòng
    +Xem báo cáo tỉ lệ phòng trống theo thời gian/theo phòng/theo loại phòng
    +Xem báo cáo tỉ lệ phòng trống theo theo phòng
    +Xem báo cáo tỉ lệ phòng trống theo theo loại phòng
    +Xem báo cáo khách hàng đặt nhiều theo thời gian
    Xem báo cáo khách hàng đặt nhiều theo nguồn gốc khách hàng
    Đối với nhân viên lễ tân:
    +Tìm phòng trống theo yêu cầu trực tiếp của khách
    +Checkin cho khách đã đặt phòng hoặc đặt phòng trực tiếp
    +Checkout cho khách
    +In hóa đơn thanh toán cho khách
    Đối với nhân viên bán hàng:
    +Tìm phòng trống 
    +Đặt phòng theo yêu cầu của khách
2. Thực thể:
  - Khách sạn: : Tên, địa chỉ, số sao, mô tả (bao gồm mô tả bằng text và bằng hình ảnh).
  - Phòng:tên phòng (duy nhất, để phân biệt các phòng), loại phòng, giá niêm yết, các loại dịch vụ đi kèm, mô tả phòng.
  - Khách hàng: Số CMND (số passport nếu là người nước ngoài), loại giấy tùy thân (CMND, passport), họ tên đầy đủ, địa chỉ, số điện thoại, ghi chú về phục vụ đặc biệt như cho người khuyết tật, ăn chay...
3. Mô tả hệ thóng:
  -	Mỗi phòng có thể được đặt/ở bởi nhiều khách hàng khác nhau tại những thời điểm khác nhau.
  -	Mỗi khách hàng có thể đặt/ở nhiều phòng khác nhau tại những thời điểm khác nhau.
  -	Tại một thời điểm, chỉ có một khách ở trong một phòng, và xác định một giá phòng cụ thể.
  -	Khách hàng chỉ có thể đặt phòng nếu phòng đó còn trống trong suốt thời gian khách hàng muốn đặt.
  -	Khách hàng có thể thanh toán nhiều lần cho đến ngày trả phòng.
  -	Mỗi lần thanh toán, lễ tân sẽ in hóa đơn cho lần thanh toán đó bao gồm các thông tin: họ tên và địa chỉ khách hàng, số phòng, ngày đến, ngày đi, giá phòng, các dịch vụ đi kèm (mỗi dịch vụ bao gồm tên dịch vụ, đơn vị tính, đơn giá, tổng tiền), số tiền thanh toán.
  -	Khách hàng có thể hủy đặt phòng (miên phí) nếu hủy trước ngày đến. Nếu khách hàng hủy sau ngày đặt thì khách hàng bị lưu vào danh sách đen và có thể bị từ chối đặt phòng trong các lần tiếp theo.
 


