### Clone source

    npm install

    npm start : để chạy source (npm playwright test --trace on)

    npm show-report : để xem view report (npx playwright show-report)

### Research

1. Cài đặt:
   npm init playwright@latest

   đợi khá lâu

2. Init:

   - Viết code ở thư mục tests
   - Xem source test dự án todo ở tests-examples

   - Chạy lệnh để test: npx playwright test [<folder>][<file>] ... more options

   - Test chạy xong thì có thể: npx playwright show-report để view result
     NOTE: có thể cài extension: Playwright test for vscode để chạy từng lệnh test nếu không muốn test toàn bộ
     khi này sẽ có 1 tab ở menu bên trái (hình lọ dung dịch) là Testing = có thể xem cấu trúc code test
   - Chạy lệnh để có GUI test UI: npx playwright test --ui
   - Chạy lệnh: npx playwright test --trace on để có thể mở GUI xem quá trình lỗi chi tiết

3. CI GitHub Actions: giúp theo dõi quá trình thay đổi source - sẽ tự động chạy test = cách GitHub Actions dựa vào file .github/workflows/playwright.yml
   nó sẽ tự sinh ra runner trên git và test (có thể set domain sau khi deploy và chạy test hoặc ko thì nó sẽ chạy runner của nó)

   - Xem kết quả ở tab Actions trên github

4. Coding
   - Tạo file và nhìn docs để code :D
   - Hoặc có thể ở menu trái, chọn Testing, tiếp đến chọn new record, nó sẽ tự động tạo 1 file test + mở ra trình duyệt, thao tác trên trình duyệt đó sẽ được chuyển đổi thành code cho user
