1. Ajax là gì ?

    AJAX là chữ viết tắt của cụm từ Asynchronous Javascript and XML. AJAX là phương thức trao đổi dữ liệu với máy chủ và cập nhật một hay nhiều phần của trang web, hoàn toàn không reload lại toàn bộ trang.

2. Tại sao lại sử dụng AJAX?

-   AJAX được dùng để thực hiện việc truy xuất dữ liệu hoặc lưu trữ dữ liệu mà không cần phải reload lại toàn bộ trang web.
-   AJAX chỉ load lại 1 phần nhỏ để cập nhật thông tin chứ không load cả trang. Bằng cách này thì có thể giảm thiểu được tốc độ tải trang giúp người dùng có trải nghiệm tốt hơn.
-   Trang web bạn tạo ra cũng sẽ đa dạng và sống động hơn.

3.  Cách ajax hoạt động

    ![](https://www.w3schools.com/js/pic_ajax.gif "ajax work")

    1 Một sự kiện xảy ra trong một trang web (trang được tải, một nút được click)

    2 Đối tượng XMLHttpRequest được tạo bởi JavaScript

    3 Đối tượng XMLHttpRequest gửi yêu cầu đến máy chủ web

    4 Máy chủ xử lý yêu cầu

    5 Máy chủ gửi phản hồi trở lại trang web

    6 Phản hồi được đọc bởi JavaScript

    7 Hành động thích hợp (như cập nhật trang) được thực hiện bởi JavaScript

4.  AJAX - đối tượng XMLHttpRequest

    Chìa khóa của ajax là đối tượng XMLHttpRequest.

    -   Tạo một đối tượng XMLHttpRequest
    -   Xác định một callback function
    -   Mở đối tượng XMLHttpRequest
    -   Gửi yêu cầu đến máy chủ

    1 Tạo một đối tượng XMLHttpRequest

    Tất cả các trình duyệt hiện đại (Chrome, Firefox, IE, Edge, Safari, Opera) đều có đối tượng XMLHttpRequest được tích hợp sẵn.

    ```javascript
    const xhttp = new XMLHttpRequest();
    ```

    2 Xác định một callback function

    ```javascript
    xhttp.onload = function () {
        // What to do when the response is ready
    };
    ```

    3 Mở đối tượng XMLHttpRequest

    ```javascript
    xhttp.open("GET", url);
    ```

    4 Gửi yêu cầu đến máy chủ

    ```javascript
    xhttp.send();
    ```
