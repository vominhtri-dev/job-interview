1.  JSON là gì ?

    JSON là viết tắt của JavaScript Object Notation, là một kiểu định dạng dữ liệu tuân theo một quy luật nhất định mà hầu hết các ngôn ngữ lập trình hiện nay đều có thể đọc được.

2.  Cú pháp

    -   Định dạng JSON sử dụng các cặp `key – value` .
    -   Chuỗi JSON được bao lại bởi dấu ngoặc nhọn `{}`.
    -   Các key, value của JSON bắt buộc phải đặt trong dấu nháy kép `""`.
    -   Nếu có nhiều dữ liệu thì dùng dấu phẩy `,` để ngăn cách.
    -   Các key của JSON bạn nên đặt chữ cái không dấu hoặc số, và không có khoảng trắng, chấm, chấm phẩy, ký tự đầu tiên không nên đặt là số.
    -   File json nó được lưu dưới phần mở rộng là `.json`

3.  Tại sao lại sử dung json

    -   Định dạng JSON về mặt cú pháp tương tự như mã để tạo các đối tượng JavaScript. Do đó, một chương trình JavaScript có thể dễ dàng chuyển đổi dữ liệu JSON thành các đối tượng JavaScript.

    -   Vì định dạng chỉ là văn bản nên dữ liệu JSON có thể dễ dàng được gửi giữa các máy tính và được sử dụng bởi bất kỳ ngôn ngữ lập trình nào.
    -   JavaScript có một chức năng tích hợp để chuyển đổi các chuỗi JSON thành các đối tượng JavaScript: `JSON.parse() `

    -   JavaScript cũng có một hàm tích hợp để chuyển đổi một đối tượng thành một chuỗi JSON:`JSON.stringify()`

4.  Kiểu dữ liệu json

-   Các kiểu dữ liệu json

    -   Kiểu string
    -   Kiểu number
    -   Kiểu object (JSON object)
    -   Kiểu array
    -   kiểu boolen
    -   Kiểu null

-   Giá trị JSON không được là một trong các kiểu dữ liệu sau

    -   Là funtion
    -   Là date
    -   Là undefined

5. JSON.parse()

    Phân tích cú pháp dữ liệu bằng `JSON.parse()` và dữ liệu trở thành một đối tượng JavaScript.

    ```javascript
    const myJSON = '{"name":"John", "age":30, "city":"New York"}';
    const obj = JSON.parse(myJSON);
    console.log(obj.name); // "John"
    ```

6. JSON.stringify()

    Cách sử dụng phổ biến của JSON là trao đổi dữ liệu đến từ máy chủ web. Khi gửi dữ liệu đến máy chủ web, dữ liệu phải là một chuỗi. Chuyển đổi một đối tượng JavaScript thành một chuỗi với JSON.stringify().

    ```javascript
    const obj = {
        name: "John",
        age: 30,
        city: "New York",
    };
    const myJSON = JSON.stringify(obj);
    console.log(myJSON); // '{"name":"John", "age":30, "city":"New York"}'
    ```
