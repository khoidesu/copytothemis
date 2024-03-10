# Chương trình copy file .cpp, .inp, .out sang thư mục themis


## 1: Giới thiệu
Việc copy từng file sang thư mục themis mất khá nhiều thời gian nên việc chỉ cần sử dụng 1 câu lệnh là có thể chuyển sang thư mục themis rất tiện lợi


## 2: Nền tảng
python

## 3: Yêu cầu
* có python và shutil (nếu code bị lỗi có thể do thiếu thư viện shutil [tại đây](https://pypi.org/project/shutils/))
* IDE sử dụng input từ file (không phải nhập khi chạy)

## 4: Cách sử dụng
1. Tải phần mềm themis từ [Themis 1.9](https://drive.google.com/file/d/1XK5TB67ckmvWppSJz-0y5Ipa9DVWrNn2/view?usp=sharing)

2. Tạo thư mục chấm bài như sau:
```cpp
cham bai --- bai lam --- tenccuaban --- (chua *file.cpp*)
        |
        ---- botest --- *file* --- TEST --- (chua *file.inp*, *file.out*)
```
### lưu ý: 
* phải tạo trước các file .cpp, .inp, .out vào các folder trên có thể đổi tên ở các * name *

* file: phải được đặt giống nhau 
    
    *ví dụ*: TASK.cpp, TASK.inp, TASK.out

* các file trong IDE (vscode, sublime, codeblock...) phải đặt tên giống như trên

3. chạy file bằng lệnh:
```python copy.py```

## 5: code
```py
import shutil

file_to_copy = 'D:/CPP/.MAIN/main.cpp' # change your destination

destination_directory = 'D:/chambai/bailam/khoidesu/TASK.cpp' # change your destination

shutil.copy(file_to_copy, destination_directory)

#===========================================================#

file_to_copy = 'D:/CPP/.MAIN/TASK.inp' # change your destination

destination_directory = 'D:/chambai/botest/TASK/TEST1/TASK.inp' # change your destination

shutil.copy(file_to_copy, destination_directory)

#===========================================================#

file_to_copy = 'D:/CPP/.MAIN/TASK.out' # change your destination

destination_directory = 'D:/chambai/botest/TASK/TEST1/TASK.out' # change your destination

shutil.copy(file_to_copy, destination_directory)

#===========================================================#
```
