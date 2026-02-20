<!DOCTYPE html>
<html>
<head>
<style>
.container {
  display: grid;
  grid-template-columns: repeat(3, 100px);
  grid-template-rows: repeat(3, 100px);
  gap: 10px;
}

.box {
  background-color: red;
}

.box:nth-child(1){background: red;}
.box:nth-child(2){background: blue;}
.box:nth-child(3){background: green;}
.box:nth-child(4){background: orange;}
.box:nth-child(5){background: purple;}
.box:nth-child(6){background: pink;}
.box:nth-child(7){background: yellow;}
.box:nth-child(8){background: cyan;}
.box:nth-child(9){background: brown;}
</style>
</head>
<body>

<div class="container">
  <div class="box"></div>
  <div class="box"></div>
  <div class="box"></div>
  <div class="box"></div>
  <div class="box"></div>
  <div class="box"></div>
  <div class="box"></div>
  <div class="box"></div>
  <div class="box"></div>
</div>

</body>
</html>

<!DOCTYPE html>
<html>
<head>
<style>
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
  grid-template-columns: 1fr 3fr;
  grid-template-rows: auto 1fr auto;
  gap: 10px;
  height: 100vh;
}

header { grid-area: header; background: lightblue; }
aside { grid-area: sidebar; background: lightgreen; }
main { grid-area: main; background: lightgray; }
footer { grid-area: footer; background: lightcoral; }

header, aside, main, footer {
  padding: 20px;
}
</style>
</head>
<body>

<div class="container">
  <header>Header</header>
  <aside>Sidebar</aside>
  <main>Main Content</main>
  <footer>Footer</footer>
</div>

</body>
</html>

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>

body{
  margin:0;
  padding:20px;
  font-family: Arial;
  background:#f4f4f4;
}

.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 15px;
}

.gallery img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 8px;
}

</style>
</head>
<body>

<h2>Responsive Image Gallery</h2>

<div class="gallery">
  <img src="https://picsum.photos/id/1015/600/400" alt="Image1">
  <img src="https://picsum.photos/id/1016/600/400" alt="Image2">
  <img src="https://picsum.photos/id/1020/600/400" alt="Image3">
  <img src="https://picsum.photos/id/1024/600/400" alt="Image4">
  <img src="https://picsum.photos/id/1035/600/400" alt="Image5">
  <img src="https://picsum.photos/id/1041/600/400" alt="Image6">
</div>

</body>
</html>

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>

body{
  margin:0;
  padding:20px;
  font-family: Arial;
  background:#f4f4f4;
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
  gap: 20px;
}

.card {
  background:white;
  border-radius:10px;
  box-shadow:0 4px 8px rgba(0,0,0,0.1);
  overflow:hidden;
}

.card img {
  width:100%;
  height:180px;
  object-fit:cover;
}

.card h3{
  margin:10px;
}

.card p{
  margin:10px;
  font-size:14px;
  color:#555;
}

</style>
</head>
<body>

<h2>Card Layout</h2>

<div class="cards">

  <div class="card">
    <img src="https://picsum.photos/id/1050/600/400" alt="">
    <h3>Nature View</h3>
    <p>Beautiful natural scenery with mountains and lake.</p>
  </div>

  <div class="card">
    <img src="https://picsum.photos/id/1060/600/400" alt="">
    <h3>City Life</h3>
    <p>Modern city skyline during sunset.</p>
  </div>

  <div class="card">
    <img src="https://picsum.photos/id/1074/600/400" alt="">
    <h3>Beach</h3>
    <p>Relaxing beach with blue water and clear sky.</p>
  </div>

</div>

</body>
</html>

