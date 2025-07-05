<template>
  <div>
    <h2>สวัสดีจาก MyComponent!</h2>
    <p>นี่คือข้อความจากคอมโพเนนต์แยก.</p>
  </div>
</template>

<script>
export default {
  name: 'MyComponent' // ชื่อของคอมโพเนนต์นี้
}
</script>

<style scoped>
h2 {
  color: rgb(160, 83, 57);
  text-align: center; /* เพิ่มให้ข้อความอยู่ตรงกลาง */
}
p {
  text-align: center; /* เพิ่มให้ข้อความอยู่ตรงกลาง */
}
</style>