<!DOCTYPE html>
<html>
<head>
<title>Login & Register</title>
<style>
body{
  margin:0;
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  background:#3d1b1b;
  font-family:sans-serif;
}
.container{
  background:rgb(196, 49, 49);
  padding:40px;
  border-radius:10px;
  width:350px;
}
input,button{
  width:100%;
  padding:10px;
  margin:10px 0;
}
button{
  background:#8b2429;
  color:rgb(10, 0, 0);
  border:none;
}
.toggle{
  text-align:center;
  cursor:pointer;
  color:rgb(2, 0, 10);
}
</style>
<script>
function toggleForm(){
  let form=document.getElementById("formTitle");
  if(form.innerText==="Login"){
    form.innerText="Register";
  }else{
    form.innerText="Login";
  }
}
</script>
</head>
<body>
<div class="container">
<h2 id="formTitle">Login</h2>
<input placeholder="Email">
<input type="password" placeholder="Password">
<button>Submit</button>
<p class="toggle" onclick="toggleForm()">Switch Login/Register</p>
</div>
</body>
</html>
