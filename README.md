# THỰC TẬP CƠ SỞ NGÀNH NHÓM 10.

## Project - Dự án

- Clone web site bán hàng: [Shop Review](https://shopreview.vn)

## Preparation steps: Install nodejs and yarn - Các bước chuẩn bị: Cài đặt nodejs, yarn, git,...

#### 1. Cài đặt Nodejs

_NodeJS là một môi trường runtime chạy JavaScript đa nền tảng và có mã nguồn mở, được sử dụng để chạy các ứng dụng web bên ngoài trình duyệt của client_

- [Click để đến trang cài đặt](https://nodejs.org/en/download)
- Cài đặt xong kiểm tra bằng terminal: `node -v`

#### 2. Cài đặt yarn

_YARN là công cụ quản lý thư viện javascript mã nguồn mở tốc độ cao, tin cậy và bảo mật nhằm thay thế NPM (Node Package Management)_

_Khi cài đặt Nodejs thành công thì mặc định đã có npm, nhưng recomended sử dụng yarn để dev front end vì nó download thư viện nhanh hơn_

- Sau khi cài đặt Nodejs xong, mở terminal gõ: `npm install --global yarn`
- Để kiểm tra gõ: `yarn --version`

#### 3. Cài đặt git: [Link tải](https://git-scm.com/downloads)

#### 4. Cài đặt IDE để phát triển: [Visual Studio Code](https://code.visualstudio.com/download)

## Steps to run project - Các bước chạy dự án

_(Recomened sử dụng git bash thay vì Command Promt hay Powershell để tránh lỗi phát sinh)_

#### 1. Download project

- Mở git bash ở nơi muốn lưu trữ dự án trên máy tính
- Gõ lệnh: `git clone https://github.com/oga126/TTCSN_NHOM10.git` để tải dự án trên github về máy

#### 2. Trỏ vào dự án

- Trên git bash gõ `cd TTCSN_NHOM10`

#### 3. Mở thư mục vừa tải bằng Visual Studio Code (Có thể bỏ qua bước này và đi đến bước 4)

- Gõ lệnh `code .` để mở dự án bằng Visual Studio Code

- Mở git bash trên Visual Studio Code: Ctrl + `

#### 4. Download các thư viện và dependencies mà dự án sử dụng

- Trên git bash gõ `yarn`

#### 5. Chạy dự án trên local

- Gõ trên git bash: `yarn dev`
- Trên git bash sẽ hiện ra liên kết dẫn đến sản phẩm của project
- Giữ Ctrl và click vào đường link đó để mở trên trình duyệt

## Technology used - Công nghệ sử dụng

### 1. Vuejs: Vite + Vue 3

- Vue.js là một framework Javascript được tạo bởi Evan You, giúp chúng ta xây dựng giao diện người dùng cũng như xây dựng Single Page Application thân thiện với người dùng, chúng xây dựng từ các thư viện, cách triển khai component, các chức năng đặc trưng của nó như SFC (Single File Component).
- Giới thiệu tổng quan về Vue: [Link](https://viblo.asia/p/mot-so-kien-thuc-co-co-ban-ve-vuejs-yMnKMjpgZ7P)

### 2. Tailwind CSS

**Tailwind CSS là gì?:**

- Tailwind CSS là một utility-first CSS framework, cũng giống như Bootstrap, nó có những class built-in mà chúng ta có thể dùng.
- Tailwind CSS có nhiều các class bao gồm các thuộc tính CSS khác nhau và quan trọng, chúng ta có thể dễ dàng mở rộng tạo mới ra những class bằng chính những class của nó.

**Tại sao chúng ta nên dùng Tailwind ?**

- Framework này cũng na ná Boostrap nhưng một điều tiện lợi khi dùng framework này là chúng ta có nhiều class mới hơn tiện lợi hơn Boostrap.
- Và hơn nữa, việc có nhiều thêm những class nhưng với quy tắc đặt tên cực kỳ thân thiện với người dùng, người dùng cũng có thể nhìn vào class đó và có thể biết được class này nó đang style cái gì.
- Chúng ta cũng phải nói đến khả năng tùy biến và mở rộng cao, đem đến cho ta sự linh hoạt không giới hạn.

## Project development process - Quá trình phát triển dự án

**_BTL tập trung vào các sản phẩm năng lượng mặt trời trên website mẫu, dữ liệu các sản phẩm mang tính tương đối, tượng trưng_**

- [x] Phân tích offical website ():
  - [x] Tổng quan về giao diện, phân trang
  - [x] Xác định được các liên quan đến sản phẩm: loại, danh mục, ...
  - [x] Xác định được các chức năng chính
  - [ ] Khác...

#### 1. UI - Giao diện

- **_Components: Là các thành phần, phần tử. <br> Ví dụ về components: Header là 1 component. Button là 1 component,... <br> Mục đích chia nhiều components: tái sử dụng, sử dụng ở nhiều nơi. <br>Ví dụ về components được tái sử dụng: ProductsCard(Hiển thị ở nhiều trang khác nhau, hiển thị nhiều lần ở 1 trang),..._**

<br>

- **_Views: hay còn gọi là Pages, nơi chứa các Components. <br> Mỗi 1 View (Page) có URL (path) riêng._**

<br>

- [x] Thiết kế router để điều hướng các trang (vừa code vừa thiết kế, phát triển và bổ sung)
- [x] Chia layout: Header và Footer không đổi **=> layout chính sẽ có 2 Components này**
- [ ] Footer **=> component**
  - [x] Static UI
  - [ ] UI các trang chính sách vận chuyển, chính sách thanh toán, chính sách đổi trả **=> view**
- [ ] Header **=> component**
  - [ ] Dropdown trên thanh tìm kiếm
  - [x] Thanh navbar ngang điều hướng
  - [x] Button `Danh mục sản phẩm` **=> component**
    - [ ] Dropdown sang bên phải, chứa các loại sản phẩm theo danh mục chính
- [ ] UI trang đăng nhập, đăng ký **=> view**
- [x] UI trang chủ **=> View**
  - [x] Banner **=> Component**
  - [x] Danh sách các sản phẩm theo loại **=> component**
- [x] UI liên quan đến sản phẩm
  - [x] Product Card: hiển thị ở trang chủ, trang phân loại sản phẩm **=> component**
  - [x] Product Details: chi tiết về sản phẩm **=> component**
    - [ ] Images slide
    - [x] Chi tiết: Tên, giá, ảnh, video, mô tả,...
  - [x] Gợi ý sản phẩm liên quan (gợi ý dựa trên các sản phẩm cùng loại) **=> component**
    - [x] Slider
- [x] UI trang Liên hệ **=> view**
- [x] UI các trang phân loại sản phẩm năng lượng mặt trời (đèn pha, đèn trang trí, đèn trụ, tấm pin): **=> view**
  - [x] small navbar
- [ ] UI các trang danh mục sản phẩm (đồ cắm trại, năng lượng mặt trời, máy đo, phụ kiện ô tô): Mỗi trang sẽ có các loại sản phẩm của nó **=> view**
  - [ ] Category Card **=> component**
- [x] UI trang giỏ hàng
  - [x] Giỏ hàng mini trên headerheader
  - [x] Trang giỏ hàng trước thanh toán
- [x] UI trang thanh toán
  - [x] Form điền thông tin
- [x] UI trang thanh toán thành công, hiển thị hóa đơn

#### 2. Function - Chức năng

- **_Composables: các hàm xử lý liên quan đến hành động, hành vi của người dùng. <br> Mục đích: tái sử dụng, sử dụng ở nhiều nơi_**

<br>

- **_Pinia store: Nơi lưu trữ, quản lý dữ liệu. <br> Bao gồm biến lưu trữ dữ liệu, các hàm xử lý dữ liệu đó_**

<br>

- [ ] Cart - giỏ hàng _(Sử dụng pinia store để lưu trữ tạm thời)_
  - [x] Thêm
  - [x] Xóa
  - [x] Số lượng
  - [x] Tổng tiền
  - [ ] Lưu trữ trên local storage: khi reload website không bị reset lại giỏ hàng
- [ ] Login, register - Đăng nhập, đăng ký _(Composable)_
  - [ ] Validate form
  - [ ] Kiểm tra, lưu trữ đã đăng nhập chưa: kiểm tra ở router là chính
- [ ] Filter - Lọc _(Composable)_
  - [ ] latest
  - [ ] most popular
  - [x] price
    - [x] cheap to expensive
    - [x] expensive to cheap
    - [x] price limition: [min, max]
  - [ ] quanlity (feedback)
  - [ ] power
- [ ] Search - Tìm kiếm
  - [ ] name
  - [ ] type
  - [ ] category
  - [ ] index
  - [ ] ...

#### 3. Perfomence, UX, Development - Tối ưu, trải nghiệm, phát triển

#### 4. Database design - Thiết kế cơ sở dữ liệu (tương đối, tượng trưng)

**_Cấu trúc dữ liệu của 1 sản phẩm_**

```
const product = {
  type: '', // loại sản phẩm
  url_offical: '', // liên kết dẫn đến website mẫu
  index: '', // id
  name: '', // tên sản phẩm
  slugy_name: '', // hash trong url: chính là slugy của name
  // slug phần ký tự ngay sau tên miền domain
  // Ví dụ: slugy của " Hoàng   Đức Nam 2003 @ ? . !" là "hoang-duc-nam-2003"
  price: '', // giá gốc
  cur_price: '', // giá sau khi được giảm giá
  discount: '%', // % giảm giá
  quantity: ~~(Math.random() * 10), // số lượng
  power: 0, // công suất
  specifications: [], // thông số kỹ thuật
  features: [], // tính năng
  mode: [], // chế độ sử dụng
  suitable: [], // phù hợp cho các hoạt động
  videos: [], // videos
  thumbnail: '', // ảnh đại diện
  images: [] // ảnh chi tiết
};
```

- [ ] Thiết kế, fake database _(chỉ làm về các sản phẩm năng lượng mặt trời)_
  - [x] Đèn pha
  - [x] Đèn trang trí
  - [ ] Đèn trụ cổng, trụ cột
  - [ ] Tấm pin

#### 5. Những thứ làm cuối cùng (hoặc không)

- [ ] Auto resize dropdown in search input
- [ ] Slide for images in product details, include model when click to zoom
