---
id: "field-notes:linux-terminal-first-steps"
translationKey: "field-notes:linux-terminal-first-steps"
title: "Linux: bước đầu với terminal — bài mẫu"
description: "Một bài thực hành mẫu để xác định vị trí, đọc danh sách tệp và quan sát hệ thống trước khi thay đổi nó."
topics: ["linux"]
tags: ["linux", "terminal"]
date: "2026-11-04"
kind: "lab"
level: "beginner"
---

> Đây là bài mẫu cho thư viện. Bạn có thể thay bằng ghi chép và kết quả thực hành của riêng mình.

## Biết mình đang ở đâu

Mở terminal trên Linux và chạy từng lệnh. Không cần quyền quản trị cho bài này.

```sh
whoami
pwd
ls -la
```

`whoami` cho biết tên người dùng hiện tại. `pwd` in thư mục làm việc. `ls -la` liệt kê các mục, bao gồm tệp ẩn, cùng thông tin chi tiết. Quan sát kết quả thật trên máy của bạn thay vì so với một đầu ra được điền sẵn.

## Thử một thư mục riêng

Tạo thư mục thực hành trong thư mục cá nhân, rồi chuyển vào đó:

```sh
mkdir -p ~/terminal-practice
cd ~/terminal-practice
pwd
```

`~` là cách shell biểu diễn thư mục cá nhân. `cd` thay đổi thư mục làm việc; chạy `cd ..` để trở về thư mục cha.

## Quan sát trước khi sửa

```sh
uname -a
```

Lệnh này hiển thị thông tin về kernel và hệ thống. Nó không thay thế thông tin phiên bản bản phân phối. Chú ý tên máy có thể xuất hiện trong kết quả; xem lại trước khi chia sẻ ảnh terminal.

## Ghi lại sau bài thực hành

- Thư mục mặc định khi mở terminal là gì?
- Tệp bắt đầu bằng dấu chấm được hiển thị thế nào?
- Sau `cd ..`, kết quả `pwd` thay đổi ra sao?

Ghi lại ba câu trả lời này bằng lời của bạn, kèm hệ điều hành và ngày thực hành, để biến bài mẫu thành ghi chép cá nhân.

```quiz
{
  "title": "Tự kiểm tra kiến thức",
  "questions": [
    {
      "id": "q1",
      "question": "Lệnh nào in thư mục làm việc hiện tại?",
      "options": [
        "uname -a",
        "pwd",
        "whoami"
      ],
      "answer": 1,
      "explanation": "pwd hiển thị vị trí hiện tại; whoami hiển thị người dùng và uname mô tả hệ thống/kernel."
    },
    {
      "id": "q2",
      "question": "Tùy chọn -a trong ls -la giúp thấy gì?",
      "options": [
        "Tự chuyển sang thư mục cha",
        "Cả các mục có tên bắt đầu bằng dấu chấm",
        "Chỉ tệp âm thanh"
      ],
      "answer": 1,
      "explanation": "ls -a không bỏ qua các tên bắt đầu bằng dấu chấm; cd .. mới chuyển thư mục cha."
    }
  ]
}
```
