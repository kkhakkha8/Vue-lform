<template>
  <form>
      <label for="email">Email</label>
      <input type="email" id="email" required v-model="email">

      <label for="password">Password</label>
      <input type="password" id="password" required v-model="password">

      <label for="">Roles:</label>
      <select v-model="role">
          <option value="developer">Web Developer</option>
          <option value="designer">Web Designer</option>       
      </select>
  </form>
  <p>email {{email}}</p>
  <p>password {{password}}</p>
  <p>Role =  {{role}}</p>
</template>

<script>
export default {
    data () {
        return {
            email : "",
            password : "",
            role : ""
        }
    }
}
</script>

<style>
form{
    max-width : 400px;
    
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
input,select{
    display : block;
    box-sizing: border-box;
    border: none;
    border-bottom: 1px solid #ddd;
    width: 100%;
    padding : 10px;
    color: #555;
}
</style>