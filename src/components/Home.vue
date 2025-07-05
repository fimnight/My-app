<script>
import MyComponent from './MyComponent.vue'; // Path จะเป็น './MyComponent.vue' เพราะอยู่โฟลเดอร์เดียวกัน
export default {
  name: 'Home',
  props: {
    msg: String
  },
  components: {
    MyComponent // ลงทะเบียน
  }
}
</script>

<template>
  <div class="hello">
    <MyComponent /> </div>
</template>