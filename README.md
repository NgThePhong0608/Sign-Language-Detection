# ML_Projects: Sign language detection
> Đây là dự án cuối kỳ đối với môn học "Học máy". Tên đề tài được chọn là "Sign language detection".
## Thành viên nhóm:
Nguyễn Thế Phong - 20002150 (<b>C</b>) 

Đinh Khả Vy - 20002183

Chu Phạm Đình Tú - 20002173

Dương Xuân Đức - 20002114

Nguyễn Kiều Trang - 20002168

## Lý do lựa chọn đề tài
Ngôn ngữ ký hiệu có tiềm năng lớn trong việc nâng cao khả năng giao tiếp và tương tác giữa người khiếm thính/câm và những người không biết ngôn ngữ ký hiệu, cũng như đem lại sự tiện lợi và đa dạng trong việc truyền đạt thông tin và ý nghĩa.

## Cấu trúc dự án
- requirements.txt: chứa các package sử dụng trong dự án
- collect_images: dùng để thu thập dữ liệu hình ảnh của các class cần detect
- convert_img_to_csv: dùng để lấy các điểm landmark của các ảnh vừa thu thập được
- train_model: huấn luyện mô hình với SVM 
- main: chương trình chính 
- model_1.pkl: model được lưu lại sau khi huấn luyện

## Công nghệ được sử dụng
- Ngôn ngữ sử dụng:
<p>
  <a>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f8/Python_logo_and_wordmark.svg/1280px-Python_logo_and_wordmark.svg.png" height="30" width="120">
  </a>
</p>

- Xây dựng mô hình học máy (Thư viện sử dụng): 
<p>
  <a>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/84/Matplotlib_icon.svg/1200px-Matplotlib_icon.svg.png" height="30" width="30">
  </a>

  <a>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/32/OpenCV_Logo_with_text_svg_version.svg/831px-OpenCV_Logo_with_text_svg_version.svg.png" height="30" width="30">
  </a>

  <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/2560px-NumPy_logo_2020.svg.png" height="30" width="80">
  </a>
  
   <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/2560px-Pandas_logo.svg.png" height="30" width="80">
  </a>
  
  <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Scikit_learn_logo_small.svg/1200px-Scikit_learn_logo_small.svg.png" height="30" width="50">
  </a>

  <a>
    <img src="https://steam.oxxostudio.tw/image/python/ai/ai-mediapipe.jpg" height="30" width="50">
  </a>
</p>

- Các ide được sử dụng:
<p>
  <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Visual_Studio_Code_1.35_icon.svg/2048px-Visual_Studio_Code_1.35_icon.svg.png" height="30" width="30">
  </a>
</p>

### Cách thức cài đặt
- Sử dụng git clone: 
- Truy cập vào thư mục "Hand-Gesture-Recognition". 
- Tạo 1 môi trường ảo python với câu lệnh: ```python -m venv env_name ```
- Trong đó ```env_name``` là tên môi trường mà bạn muốn đặt. Sau khi cài xong môi trường ảo kích hoạt môi trường đó thông qua câu lệnh ```python.\env_name\Script\Activate.ps1```
- Thực hiện cài đặt các package cần sử dụng thông qua câu lệnh ```python pip install -r requirements.txt ```

### Chạy chương trình
- Lần lượt chạy các file: 
    + ```colect_images.py``` để thu thập dữ liệu cá nhân của bạn
    + ```convert_img_to_csv.py``` để lấy các landmark
    + ```train_model.ipynb``` để huấn luyện mô hình
    + ```main.py``` chạy trương chính

## Kết luận
Qua bài tập lớn trên nhóm chúng em đã làm được ứng dụng được việc sử dụng các mô hình học máy để giải quyết các bài toán về  **Nhận diện ký tự qua ngôn ngữ cơ thể**.
### Hạn chế của dự án
Dự án dù đã chạy theo đúng kết quả nhóm mong muốn tuy nhiên vẫn còn hạn chế trong số lượng các loại ký hiệu có thể nhận diện (cụ thể dự án này nhóm chỉ thực hiện detect 7 ký tự bao gôm (A, B, C, D, E và 2 ký tự custom (Like và Heart))). 
### Định hướng phát triển trong tương lai
Nhóm sẽ tiếp tục nghiên cứu để có thể nhận diện được toàn bộ 37 ký tự theo bảng chữ số và chữ cái alphabet. Không chỉ dừng lại ở việc detect, nhóm sẽ cố gắng cải tiến thêm để có thể nhận diện và dịch thành câu qua các ký hiệu đó.

