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

      <div>
        <input type="checkbox" v-model="accept">
        <label>Accept terms and conditions</label>
      </div>

      <!-- multiple checkbox -->
      <label>Check names</label><br>
      <div>
        <input type="checkbox" value="aungaung" v-model="names">
        <label>Aung Aung</label><br>
      </div>
      <div>
          <input type="checkbox" value="mgmg" v-model="names">
          <label>Mg Mg</label><br>
      </div>
      <div>
          <input type="checkbox" value="christ" v-model="names">
          <label>Christ</label><br>
      </div>
      <div>
          <input type="checkbox" value="phillp" v-model="names">
          <label>Phillp</label><br>
      </div>
        

      

      
  </form>
  <p>email {{email}}</p>
  <p>password {{password}}</p>
  <p>Role =  {{role}}</p>
  <p>accept - {{accept}}</p>
  <p>names - {{names}}</p>
</template>

<script>
export default {
    data () {
        return {
            email : "",
            password : "",
            role : "",
            accept : false,
            names : []
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
    background-color: #eee;
}
input[type="checkbox"] {
    display: inline-block;
    margin: 0 10px 0 0;
    width: 16px;
    position: relative;
    

}
</style>