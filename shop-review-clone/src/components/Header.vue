<script setup>
import { ref } from 'vue';
const dropdown = [
  {
    value: 'leu-cam-trai',
    name: 'Lều cắm trại'
  },
  {
    value: 'den-pha-nang-luong-mat-troi',
    name: 'Đèn Pha Năng Lượng Mặt Trời'
  },
  {
    value: 'den-pin-cam-trai',
    name: 'Đèn pin cắm trại'
  },
  {
    value: 'den-trang-tri-nang-luong-mat-troi',
    name: 'Đèn Trang Trí Năng Lượng Mặt Trời'
  },
  {
    value: 'den-tru-cong-tru-cot',
    name: 'Đèn Trụ Cổng, Trụ Cột'
  },
  {
    value: 'leu-tre-em',
    name: 'Lều Trẻ Em'
  },
  {
    value: 'may-do-nong-do-oxy-trong-mau',
    name: 'Máy Đo Nồng Độ Oxy Trong Máu'
  },
  {
    value: 'may-khu-doc-thuc-pham',
    name: 'Máy khử độc thực phẩm'
  },
  {
    value: 'nhiet-ke-hong-ngoai',
    name: 'Nhiệt Kế Hồng Ngoại'
  },
  {
    value: 'phu-kien-cam-trai',
    name: 'Phụ kiện cắm trại'
  },
  {
    value: 'tam-pin-nang-luong-mat-troi',
    name: 'Tấm Pin Năng Lượng Mặt Trời'
  },
  {
    value: 'tuong-de-xe-oto',
    name: 'Tượng Để Xe Ô Tô'
  }
];

const selected = ref('all');

const dropdowChange = () => {
  console.log(selected.value);
};
</script>

<template>
  <div class="bg-white">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex justify-between items-center py-2">
        <!-- Logo -->
        <router-link to="/">
          <div class="w-52">
            <img
              src="https://shopreview.vn/wp-content/uploads/2020/12/logo-Copy-2.png"
              alt=""
              class="w-full h-auto"
            /></div
        ></router-link>

        <!-- Tìm kiếm -->
        <div class="flex items-center border border-primary rounded-md">
          <select
            class="outline-none bg-gray-100 py-3 rounded-tl-md rounded-bl-md text-sm"
            name=""
            id=""
            v-model="selected"
            @change="dropdowChange"
          >
            <option value="all" selected class="bg-white">All</option>
            <option v-for="item in dropdown" :key="item.value" :value="item.value" class="bg-white">
              {{ item.name }}
            </option>
          </select>

          <input
            type="text"
            placeholder="Tìm kiếm các danh mục, sản phẩm..."
            class="outline-none h-full py-3 pl-4 text-sm"
          />
          <button class="bg-primary-hover h-full w-full py-2 px-6 rounded-tr-md rounded-br-md">
            <font-awesome-icon icon="fa-solid fa-magnifying-glass" class="text-white" />
          </button>
        </div>

        <!-- Đăng nhập và giỏ hàng -->
        <div class="flex items-center text-[13px] font-semibold">
          <div class="mr-4 text-dark-light">ĐĂNG NHẬP</div>
          <div class="flex items-center text-primary">
            <div class="mr-2">GIỎ HÀNG</div>
            <div
              class="border-2 border-primary rounded-full h-8 w-8 flex justify-center items-center relative before:content-['4'] before:absolute before:bottom-[80%] before:left-[80%] before:w-5 before:h-5 before:rounded-full before:text-white before:text-sm before:font-bold before:flex before:items-center before:justify-center before:bg-primary"
            >
              <font-awesome-icon icon="fa-solid fa-cart-shopping" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
