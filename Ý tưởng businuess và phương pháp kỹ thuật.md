# ENEWS-LÀM NHƯ THẾ NÀO

## Xây dưng một website với các chức năng sau:

1. Tổng hợp tất cả thông tin nổi bật từ các website tiếng anh
- Có một tập hợp các website tin tức tiếng anh nổi tiếng trong cơ sở dữ liệu. Các website này do người quản lý hệ thống nhập vào, và cập nhật theo thời gian, theo tiêu chí chọn các web có nội dung phong phú và có lượng người đọc cao. Các website đó có thể là:
  - Website tin tức của nước ngoài như VOA, BBC, USA Today, The New York Times,...
  - Website bằng tiếng anh của các báo ở Việt Nam như tuoitrenews.vn,thanhniennews.com, dtinews.vn,  english.vietnamnet.vn,...
  - Các trang mạng xã hội với nội dụng tiếng anh, như Facebook, youtube tiếng anh,...

- Website sẽ tự động hàng ngày duyệt hết các trang tin trên, duyệt hết các tin đăng trong thời gian gần đây (trong vòng 1 tuần), và sẽ lấy 10% tin có số lượt xem nhiều nhất của mỗi trang web và tải về máy.

2. Mỗi tin tức được tải về lưu trong hệ thống sẽ được các thuật toán phân loại tự động theo 2 tiêu chí sau:
- Theo chủ đề: Dựa vào tên mục đăng tin đó trong trong website gốc, và dựa vào tập hợp các từ sử dụng trong câu, thuật toán sẽ đánh giá tin đó thuộc loại chủ đề nào. VD: bóng đá, chính trị, du học,...
- Theo trình độ: Hệ thống sẽ có một danh sách hầu hết các từ vựng tiếng anh, được phân theo cấp độ khó, từ 1 đến 10. Sau đó, thuật toán đánh giá sẽ duyệt hết các từ trong bản tin đó, thống kê số lượng từ vựng ở mỗi cấp độ, từ đó cho điểm đánh giá độ khó từ vựng của bản tin đó, từ 1 đến 10.

3. Tạo cho mỗi người dùng một tài khoản để sử dụng, chứa những thông tin sau:
- Tên đăng nhập và mật khẩu
- Danh sách những chủ đề mà người dùng yêu thích hoặc quan tâm. Có được thông tin này bằng 2 cách sau:
  - Lần đầu tiên sử dụng website, người dùng sẽ được đưa ra một bảng chọn các chủ đề, sở thích. Người dùng sẽ tích chọn những chủ đề đúng với sở thích và quan tâm của mình.
  - Trong lúc người dùng đọc các tin được đưa ra trên trang web (sẽ được đề cập ở phần sau), người dùng sẽ nhấn vào các nút "Thú vị" ở cuối mỗi tin (tương tự nút like trên Facebook) để đánh giá độ thí vị hấp dẫn của tin, qua đó đánh giá được người dùng có yêu thích một chủ đề nào đó hay không và bổ sung thồn tin vào danh sách chủ đề của người dùng.
 - Trình độ từ vựng của người dùng (đánh giá theo điểm từ 1 đến 10). Thông tin này sẽ có được bằng 2 cách sau:
    - Lần đầu sử dụng website, người dùng sẽ trải qua 1 bài test từ vựng nhỏ để dánh giá trình độ từ vựng của người dùng
    - Trong lúc người dùng đọc các tin được đưa ra trên trang web, khi gặp một từ chưa biết, người dùng sẽ sử dụng từ điển tra cứu nhanh tích hợp vào sẵn trong trang web (sẽ đề cập ở phần sau), để tra từ đó. Qua đó hệ thống sẽ biết được người dùng không biết những từ vựng thuộc cập độ nào, đã biết
những từ thuộc cấp độ nào, từ đó thuật toán sẽ đánh giá được trình độ của người dùng
- Tài khoản này của người dùng sẽ liên kết với tài khoản facebook của họ, để có thể thực hiện các chức nay tương tác với bạn bè(sẽ đề cập ở phần sau).

4. Mỗi lần người dùng lên website để đọc tin tức, website sẽ sử dụng thuật toán, đối chiếu thông tin tài khoản của người dùng, để chọn lọc trong cơ sở dữ liệu, những tin tức phù hợp nhất với người dùng đó, để đưa ra cho người đọc dưới dạng timeline:
- Mỗi mục trong timeline sẽ chứa nôi dung tin đó, kèm theo link đến bản tin gốc.
- Dưới mỗi mục(mỗi tin) sẽ có những nút để đánh giá mức độ thú vị, phần để viết bình luận cũng như nút share tin này cho bạn bè trên facebook nếu thấy tin bổ ích.
- Website tích hợp một từ điển dịch nhanh, khi người dùng không biết từ nào thì click đúp vào từ đó để dịch. Đồng thời lúc đó, hệ thống sẽ đựa trên mức độ của từ đang dịch để đánh giá trình độ người dùng.

5. Vì quá trình học tiếng anh cần kiên trì, nên nếu một thời gian người dùng không lên web hoặc người dùng sử dụng web với thời gian chưa đủ, trang web sẽ có thông báo trên email hoặc facebook để nhắc nhở người dùng.
 Ngoài ra, cứ sau một khoảng thời gian nhất đinh, website sẽ cho người dùng thực hiện lại một bài test nhỏ, với từ vựng đã học được trong thời gian gần đây qua các bản tin, để người dùng có thể đánh giá mức độ tiến bộ của mình
