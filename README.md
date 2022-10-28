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
4.  Khai báo var được định danh là toàn cục (global) hoặc hàm (function) trong khi let và const được định phạm vi là khối mã (block)
    Biến var có thể được cập nhật và khai báo lại trong phạm vi tồn tại, biến let có thể được câp nhật nhưng không thể khai báo lại, biến const không thể cập nhật cũng không thể khai báo lại
    Khai báo biến var, let, const đều được dịch chuyển lên đầu của phạm vi
    Nhưng trong khi biến var được khởi gán giá trị là underfined, biến let và const không được gởi gán giá trị
    Trong khi var và let có thể được khai báo không khởi gán giá trị, const phải khởi gán giá trị khi khai báo
