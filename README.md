# THỰC TẬP CƠ SỞ NGÀNH NHÓM 10.

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

## Dự án

- Clone web site bán hàng: [Shop Review](https://shopreview.vn)

## Cài đặt nodejs và yarn

1. Cài đặt Nodejs

- [Click để đến trang cài đặt](https://nodejs.org/en/download)
- Cài đặt xong kiểm tra bằng terminal: `node -v`

2. Cài đặt yarn

- Sau khi cài đặt Nodejs xong, mở terminal gõ: `npm install --global yarn`
- Để kiểm tra gõ: `yarn --version`

3. Cài đặt git: https://git-scm.com/downloads

## Các bước chạy dự án

1. Clone repo

- Mở terminal và cd đến nơi lưu thư mục
- Gõ lệnh: `git clone https://github.com/oga126/TTCSN_NHOM10.git`

2. Mở thư mục vừa tải bằng Visual Studio Code
3. Mở terminal trên Visual Studio Code: Ctrl + `
4. Trên terminal gõ: `cd shop-review-clone`, sau đó gõ: `yarn` để download thư viện
5. Để chạy dự án trên local

- Gõ trên terminal: `yarn`
- Compile and Hot-Reload: biên dịch mã nguồn và tự động reload khi mã nguồn thay đổi

## Công nghệ sử dụng

### 1. Vuejs: Vite + Vue 3

- Vue.js là một framework Javascript được tạo bởi Evan You, giúp chúng ta xây dựng giao diện người dùng cũng như xây dựng Single Page Application thân thiện với người dùng, chúng xây dựng từ các thư viện, cách triển khai component, các chức năng đặc trưng của nó như SFC (Single File Component).
- Giới thiệu tổng quan về Vue: [Link](https://viblo.asia/p/mot-so-kien-thuc-co-co-ban-ve-vuejs-yMnKMjpgZ7P)

### 2. Tailwind CSS

- Tailwind CSS là gì?:

Tailwind CSS là một utility-first CSS framework, cũng giống như Bootstrap, nó có những class built-in mà chúng ta có thể dùng. Tailwind CSS có nhiều các class bao gồm các thuộc tính CSS khác nhau và quan trọng, chúng ta có thể dễ dàng mở rộng tạo mới ra những class bằng chính những class của nó.

- Tại sao chúng ta nên dùng Tailwind ?

Framework này cũng na ná Boostrap nhưng một điều tiện lợi khi dùng framework này là chúng ta có nhiều class mới hơn tiện lợi hơn Boostrap. Và hơn nữa, việc có nhiều thêm những class nhưng với quy tắc đặt tên cực kỳ thân thiện với người dùng, người dùng cũng có thể nhìn vào class đó và có thể biết được class này nó đang style cái gì. Chúng ta cũng phải nói đến khả năng tùy biến và mở rộng cao, đem đến cho ta sự linh hoạt không giới hạn.
