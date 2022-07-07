1. Git là gì ?

    Git là một hệ thống kiểm soát phiên bản (Version Control System). Nó theo dõi các project và file khi chúng thay đổi theo thời gian.

2. Khởi tạo với git

    Khởi tạo git

    ```
    git init
    ```

    Thêm vào git

    ```
    git add <filename_one>
    ```

    Commit thay đổi

    ```
    git commit <filename_one>
    ```

    Đẩy lên repo

    ```
    git push
    ```

3. Các thuật ngữ quan trọng trong Git

    - `Repository`: Kho lưu trữ là một tập hợp các mã nguồn. Repository là nơi chứa tất cả commit của dự án.

    - `Commit` : commit ghi lại một thay đổi hoặc một loạt các thay đổi mà bạn đã thực hiện đối với một file trong repo.

    - `Branch` : Một branch (nhánh) về cơ bản là một tập hợp các mã thay đổi duy nhất với một tên duy nhất. Mỗi repo có thể có một hoặc nhiều branch.

    - `Checkout`: Bạn có thể sử dụng lệnh `git checkout` để chuyển các branch.

    - `Fork` : Fork là một bản sao của kho lưu trữ (repository).

    - `Fetch`: Sử dụng lệnh `git fetch` để tìm nạp các bản sao và tải xuống các tệp branch vào máy tính của bạn.
