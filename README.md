# Giới thiệu

Đây là đồ án môn dự án công nghệ thông tin 1 thuộc khoa Công Nghệ Thông Tin - Đại Học Tôn Đức Thắng

Đồ án này được thực hiện bởi:



|   Họ và tên               | MSSV         |
|:-------------------------:|:------------:|
| Đinh Thị Ngọc Phượng      | 52100923     |
| Đinh TPhú Quốc            | 52100927     |




# Cách chạy code


## Bước 1 : Upload source code lên google drive

Git clone repo này về máy : 

Tiếp theo, upload toàn bộ repo lên google drive của bạn 

Bạn có thể xóa file .git trong thư mục để tăng tốc độ tải lên 1 chút



![Hình ảnh upload folder lên google drive](image/upload_colab_folder.png)

Đây là hình ảnh bên trong folder

![Hình ảnh upload folder lên google drive](image/upload_colab_folder_inside.png)



## Bước 2 : Thiết lập lại các thông số

Truy cập vào file "52100923_52100927_RAG.ipynb" bằng google colab.

Trong phần mục lục, navigate đến mục **Set up Global Variable**


![Hình ảnh navigate](image/colab_first_screen.png)



Sau khi đã navigate, Kéo xuống gần cuối của cell này, bạn sẽ cần chỉnh sửa những thông số trong ô màu đỏ

![Hình ảnh navigate](image/colab_second_screen.png)

Tại đây, bạn cần chỉnh sửa các thông số sau:


1. repo_folder : đây là đường dẫn đến thư mục mà file này đang nằm trên google drive (đường dẫn này không chứa dấu "/" cuối cùng).

2. llm_api_key : đây là api key của google gemini, bạn có thể tự tạo cho mình một api key [tại đây](https://aistudio.google.com/apikey).


3. ngrok_api_key : đây là api key của ngrok, bạn có thể truy cập trang chủ của ngrok và làm theo hướng dẫn để có thể có được api key của riêng mình [tại đây](https://ngrok.com/).


## Bước 3 : Sử dụng

Kiểm tra xem môi trường hiện tại có phải là T4 GPU hay không, nếu không phải, bạn có thể thay đổi sang môi trường này trong mục "Change runtime type".

Nếu không kết nối được với GPU, bạn cần sử dụng 1 tài khoản Google khác và thực hiện lại từ đầu.

Sau khi đã kiểm tra môi trường chạy, chọn "Runtime" -> "Run all"

![Hình ảnh môi trường chạy](image/colab_third_screen.png)


Sau khi toàn bộ source code đã chạy xong, navigate đến mục "Run app" và click vào link ngrok


![Hình ảnh môi trường chạy](image/colab_run_screen.png)


Sau đó, bạn sẽ được chuyển hướng đến trang giao diện của chatbot

![Hình ảnh visit site](image/ui_first_screen.png)

Bạn chờ 1 khoảng thời gian ngắn (khoãng 30s)để giao diện được load lên lần đầu tiên.

![Hình ảnh chatbot](image/ui_second_screen.png)


Vậy là bạn đã có thể sử dụng chatbot này để hỗ trợ công việc tư vấn pháp luật lĩnh vực luật doanh nghiệp Việt Nam rồi.

## Lưu ý:

Sau khi sử dụng xong, bạn cần truy cập vào ngrok , mục "Agent" và kết thúc phiên chạy hiện tại.

Vì đây là phiên bản miễn phí, vì thế ngrok có giới hạn mỗi tài khoản chỉ được chạy 3 agent 1 lúc, vì thế bạn cần kết thúc phiên ngrok hiện tại trước khi có thể chạy lại toàn bộ source code.

![Hình ảnh kết thúc ngrok](image/ngrok_agent.png)
