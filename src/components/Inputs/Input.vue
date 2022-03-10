<template>
  <input type="text" placeholder="Имя" />
</template>

<script>
export default {};
</script>

<style scoped>
input {
  outline: none;
  padding: 15px 20px;
  border-radius: 5px;
  border: 1px solid #666;
  background-color: transparent;
  font-family: Gilroy;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 19px;
  color: #ffffff;
}
input::placeholder,
input::-webkit-input-placeholder {
  font-family: Gilroy;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 19px;
  color: #ffffff;
}
</style>