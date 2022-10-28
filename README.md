Link MERN: https://baonguyendn.netlify.app/
1. <script>
    setTimeout(
    () => {
    console.log("Hello!!!\n " + new Date().toString());
    }, 1000);
    console.log("After 4 seconds will print Hello:\n " + new Date().toString());
    const seconds = new Date().getTime();
    while (true) {
        if (new Date().getTime() - seconds > 4000 ) {
            break;
        }
    }
    </script>
2. none

3. none

4.  Khai báo var được định danh là toàn cục (global) hoặc hàm (function) trong khi let và const được định phạm vi là khối mã (block)
    Biến var có thể được cập nhật và khai báo lại trong phạm vi tồn tại, biến let có thể được câp nhật nhưng không thể khai báo lại, biến const không thể cập nhật cũng không thể khai báo lại
    Khai báo biến var, let, const đều được dịch chuyển lên đầu của phạm vi
    Nhưng trong khi biến var được khởi gán giá trị là underfined, biến let và const không được gởi gán giá trị
    Trong khi var và let có thể được khai báo không khởi gán giá trị, const phải khởi gán giá trị khi khai báo
    
5.  Tham trị áp dụng cho kiểu nguyên thuỷ (String, number hoặc boolen) giá trị trước và sau khi gọi function không thay đổi
    Tham chiếu áp dụng cho kiểu Array, Object giá trị trước và sau khi gọi function có thể thay đổi
    Nếu dùng tham chiếu mà muốn giá trị không bị thay đổi ta dùng từ khóa const vào tham số đó.
    
6.  Callback có nghĩa là một function sẽ được thực thi sau khi một function khác đã được thực thi xong - do đó nó có tên là callback(gọi lại). Trong Javascript, functions là objects,do đó nó có thể nhận tham số là function, và cũng có thể trả về một function.

    Promise là một cơ chế trong JavaScript giúp bạn thực thi các tác vụ bất đồng bộ mà không rơi vào callback hell hay pyramid of doom, là tình trạng các hàm callback     lồng vào nhau ở quá nhiều tầng.

      Async - khai báo một hàm bất đồng bộ (async function someName(){...}).
    -Tự động biến đổi một hàm thông thường thành một Promise.
    -Khi gọi tới hàm async nó sẽ xử lý mọi thứ và được trả về kết quả trong hàm của nó.
    -Async cho phép sử dụng Await.
    
      Await - tạm dừng việc thực hiện các hàm async. (Var result = await someAsyncCall ()- Khi được đặt trước một Promise, nó sẽ đợi cho đến khi Promise kết thúc và trả về kết quả.- Await chỉ làm việc với Promises, nó không hoạt động với callbacks.- Await chỉ có thể được sử dụng bên trong các function async
      
7. Những gì forEach() làm được thì map() cũng có thể làm được và ngược lại.
map() cấp phát bộ nhớ và lưu trữ các giá trị trả về, forEach()) thì bỏ qua các giá trị trả về.
forEach() cho phép gọi hàm callback để thay đổi mảng hiện tại, thay vào đó map() sẽ trả về một mảng mới.
for() là biết trước số lần lặp, là vòng lặp được sử dụng lặp lại một nhiệm vụ nhất định với số lần lặp cho trước

8. Every:
    Nếu tất cả các phần tử trong mảng thoả mãn một hoặc nhiều điều kiện.    Hàm này sẽ trả về true, nhưng chỉ cần có 1 phần trử không thoả mãn điều kiện (failed), thì hàm này sẽ trả về false.
    Some:
    Lặp tất cả các phần tử trong một Array, chỉ phần 1 phần tử thoả mãn điều kiện thì Array này sẽ trả về true. Nhớ nhé, chỉ cần 1 phần tử thoả mãn điều kiện thôi sẽ lập tức trả về true luôn mà không cần quan tâm tới các phần tử khác

9. . Web Worker (hay Worker) là một đối tượng JavaScript được tạo bằng việc sử dụng Worker constructor (e.g Worker, SharedWorker, AudioWorker) với tham số là tên (đường dẫn) đến một JavaScript file. JavaScript file đó chứa các logic được khởi chạy bên trong thread của worker vừa tạo. Script bên trong Worker sẽ được thực thi ở background và tách biệt khỏi thread chính của web application.
Mô đun child_ process cho phép chúng ta truy cập các chức năng của Hệ điều hành bằng cách chạy bất kỳ lệnh hệ thống nào bên trong một tiến trình con, kiểm soát input stream và lắng nghe outout stream của nó.

10. . Blocking có nghĩa là các dòng lệnh được thực hiện một cách tuần tự. Khi một dòng lệnh ở phía trước chưa được hoàn thành thì các dòng lệnh phía sau sẽ chưa được thực hiện và phải đợi khi mà thao tác phía trước hoàn tất
Non- blocking là Bất đồng bộ giải quyết được vấn đề blocking của đồng bộ, được gọi là non-blocking. Nghĩa là khi chạy một tác vụ nặng (IO, network,...) thì những lệnh tiếp theo được phép chạy ngay mà không cần chờ tác vụ kia hoàn thành.
Nodejs chạy đơn luồng mà không bị blocking là vì node.js có cơ chế xử lý các hàm bất đồng bộ bằng Event Loop (vòng lặp sự kiện) với sự trợ giúp của Event Queue và cả Thread Pool

Many thanks !!!

