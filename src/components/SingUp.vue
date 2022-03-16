<template>
  <form>
      <label for="email">Email</label>
      <input type="email" id="email" required>
  </form>
</template>

<script>
export default {

}
</script>

<style>
form{
    max-width : 400px;
    height: 150px;
    margin : 30px auto;
    padding: 40px;
    border-radius: 10px;
    background-color: white;
    text-align: left;
}
label{
    color: #aaa;
    display : inline-block;
    text-transform: uppercase;
    margin: 30px 0 15px;
    letter-spacing: 1px;
    font-weight: bold;
}
input{
    display : block;
    box-sizing: border-box;
    border: none;
    border-bottom: 1px solid #ddd;
    width: 100%;
    padding : 10px;
    color: #555;
}
</style>