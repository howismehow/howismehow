<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{
            background-color: beige;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        .menu {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex; 
}

.menu li {
  margin: 0 10px; 
}

.menu li a {
  display: block; 
  text-decoration: none; 
  color: #333; 
  padding: 10px;
  border-radius: 5px; 
  transition: background-color 0.3s ease;
}

.menu li a:hover {
  background-color: #333; 
  color: #fff; 
}

#login-toggle:hover {
  background-color: #333; 
  color: #fff; 
}
#login-toggle {
  background-color: #fff;
  color: #333;
  padding: 20px;
  border-radius: 5px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
  max-width: 400px;
  margin: 0 auto;
}
.login-box form input[type="email"],
.login-box form input[type="password"] {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border-radius: 5px;
  border: none;
  box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.1);
}

.login-box form input[type="checkbox"] {
  margin-right: 5px;
}

input[type="submit"] {
  background-color: #fff;
  color: #6d6565;
  border: none;
  border-radius: 5px;
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

input[type="submit"]:hover {
  background-color: #333;
}

input[type="email"],
input[type="password"] {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
  border-radius: 5px;
  border: none;
  box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.1);
}
input[type="email"]:focus,
input[type="password"]:focus {
  box-shadow: 0px 0px 10px #333;
}

input[type="email"]:hover,
input[type="password"]:hover {
  box-shadow: 0px 0px 10px #ffffff;
}
#login-toggle {
  background-color: #fff; 
  color: #333; 
  border: none; 
  padding: 10px; 
  border-radius: 5px; 
  cursor: pointer; 
  transition: background-color 0.3s ease; 
}

#login-toggle:hover {
  background-color: #333; 
  color: #fff; 
}
    </style>
</head>
<body>
    <nav>
        <ul class="menu">
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
            <button id="login-toggle" onclick="toggleLogin()">Login</button>
          </ul>
    </nav>
    <br><br><br>
<div id="login-toggle" class="container">
    <form>

        <h2>
            Login
        </h2>
        <input type="email" placeholder="Enter Your Email" required>
        <br>
        <input type="password" id="myInput" placeholder=" Enter your password"><br><br>
    <input type="checkbox" onclick="myFunction()">Show Password
    <script>
    function myFunction() {
      var x = document.getElementById("myInput");
      if (x.type === "password") {
        x.type = "email";
      } else {
        x.type = "password";
      }
    }
    </script>
    <br><br>
    <input type="submit" value="submit">
    </div>
    </form>
</body>
</html>
