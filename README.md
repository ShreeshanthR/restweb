# Ex.07 Restaurant Website
## Date:11.10.2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
home.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>OXHEART - Home</title>
  <link rel="stylesheet" href="home.css">
</head>
<body class="home-bg">
  <div class="overlay">
    <nav>
      <div class="logo">
        <img src="Screenshot 2025-10-09 011444.png" alt="Oxheart logo">
        <h1>OXHEART</h1>
      </div>
      <ul>
        <li><a href="home.html">Home</a></li>
        <li><a href="menu.html">Menu</a></li>
        <li><a href="admin.html">Admin</a></li>
        <li><a href="contact.html">Contact Us</a></li>
      </ul>
    </nav>

    <main class="hero">
      <h2 align="left">Shreeshanth R - 25012265</h2>
      <div class="quotes">
        <h2 class="big-quote">"WHERE FLAVOR MEETS PASSION"</h2>
        <h2 class="big-quote">"COOKING WITH HEART, SERVING WITH SOUL"</h2>
        <p class="lead">Welcome to Oxheart — where every dish tells a story of warmth, taste, and creativity.</p>
        <p class="lead">We believe great food is an art form crafted with love and dedication.</p>
      </div>

      <figure class="restaurant-figure">
        <img src="frontp.avif" alt="Restaurant Interior - RESTAURANT">
        <figcaption>RESTAURANT</figcaption>
      </figure>
    </main>

    <footer>
      © 2025 OXHEART RESTAURANT — ALL RIGHTS RESERVED
    </footer>
  </div>
</body>
</html>

home.css
:root{
  --accent: #ed2334;
  --bg-dk: #121212;
  --card: #1f1f1f;
  --muted: #d3d3d3;
}

html,body{height:100%; margin:0;}
body.home-bg{
  background-image: url('https://images.unsplash.com/photo-1501117716987-c8e5a4a7f7d6?auto=format&fit=crop&w=2000&q=80');
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  font-family: "Poppins", Arial, sans-serif;
  color: #fff;
  min-height: 100vh;
}

.overlay{
  min-height:100vh;
  background: linear-gradient(rgba(0,0,0,0.55), rgba(0,0,0,0.55));
  display: flex;
  flex-direction: column;
}

nav{
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:18px 36px;
  background: rgba(0,0,0,0.25);
  backdrop-filter: blur(4px);
}
.logo{display:flex; align-items:center; gap:12px;}
.logo img{width:48px;height:48px;}
.logo h1{margin:0; font-size:22px; color:var(--accent); letter-spacing:1px;}
nav ul{list-style:none; margin:0; padding:0; display:flex; gap:20px;}
nav a{color:#fff; text-decoration:none; font-weight:600;}
nav a:hover{color:var(--accent);}

.hero{flex:1; display:flex; flex-direction:column; align-items:center; justify-content:center; padding:30px;}
.quotes{max-width:1000px; text-align:center;}
.big-quote{margin:6px 0; font-size:26px; font-weight:800; color:var(--accent);}
.lead{color:var(--muted); margin:6px 0; font-size:18px;}

.restaurant-figure{margin-top:28px; text-align:center; width:85%; max-width:1100px;}
.restaurant-figure img{
  width:100%;
  border-radius:16px;
  box-shadow: 0 10px 40px rgba(0,0,0,0.6);
  display:block;
}
.restaurant-figure figcaption{
  margin-top:10px;
  font-weight:700;
  letter-spacing:1px;
  color:#fff;
}

footer{
  padding:14px 20px;
  text-align:center;
  background: rgba(0,0,0,0.25);
  color:#bdbdbd;
  font-size:13px;
}

@media (max-width:700px){
  .big-quote{font-size:18px;}
  .logo h1{font-size:18px;}
  nav{padding:12px 18px;}
  .restaurant-figure{width:95%;}
}

menu.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>OXHEART - Menu</title>
  <link rel="stylesheet" href="menu.css">
</head>
<body>
  <nav>
    <div class="logo">
      <img src="https://cdn-icons-png.flaticon.com/512/857/857681.png" alt="Oxheart logo">
      <h1>OXHEART</h1>
    </div>
    <ul>
      <li><a href="home.html">Home</a></li>
      <li><a href="menu.html">Menu</a></li>
      <li><a href="admin.html">Admin</a></li>
      <li><a href="contact.html">Contact Us</a></li>
    </ul>
  </nav>

  <main class="menu-main">
    <h2 class="page-title">OUR MENU</h2>

    <!-- Starters -->
    <section class="menu-section">
      <h3>STARTERS</h3>
      <div class="menu-grid">
        <article class="card">
          <img src="tomato-soup-recipe.jpg" alt="Tomato Soup">
          <div class="card-body">
            <h4>TOMATO SOUP</h4>
            <p class="price">₹99</p>
          </div>
        </article>

        <article class="card">
          <img src="vegsoup.jpg" alt="Vegetable Soup">
          <div class="card-body">
            <h4>VEGETABLE SOUP</h4>
            <p class="price">₹119</p>
          </div>
        </article>

        <article class="card">
          <img src="mutton.jpg" alt="Mutton Soup">
          <div class="card-body">
            <h4>MUTTON SOUP</h4>
            <p class="price">₹149</p>
          </div>
        </article>
      </div>
    </section>

    <!-- Biriyani -->
    <section class="menu-section">
      <h3>BIRIYANI</h3>
      <div class="menu-grid">
        <article class="card">
          <img src="chicken_biryani.jpg" alt="Chicken Biriyani">
          <div class="card-body">
            <h4>CHICKEN BIRIYANI (HYDERABAD STYLE)</h4>
            <p class="price">₹249</p>
          </div>
        </article>

        <article class="card">
          <img src="Mutton-Biryani.jpg" alt="Mutton Biriyani">
          <div class="card-body">
            <h4>MUTTON BIRIYANI</h4>
            <p class="price">₹299</p>
          </div>
        </article>

        <article class="card">
          <img src="veg-biriyani.jpg" alt="Veg Biriyani">
          <div class="card-body">
            <h4>VEG BIRIYANI</h4>
            <p class="price">₹99</p>
          </div>
        </article>
      </div>
    </section>

    <!-- Breads -->
    <section class="menu-section">
      <h3>BREADS</h3>
      <div class="menu-grid">
        <article class="card small">
          <img src="naan.jpg" alt="Naan">
          <div class="card-body">
            <h4>NAAN</h4><p class="price">₹49</p>
          </div>
        </article>

        <article class="card small">
          <img src="parotta.jpg" alt="Parotta">
          <div class="card-body">
            <h4<P>PAROTTA</h4>
            <p class="price">₹39</p>
          </div>
        </article>

        <article class="card small">
          <img src="roti.jpg" alt="Roti">
          <div class="card-body">
            <h4>ROTI</h4><p class="price">₹29</p>
          </div>
        </article>
      </div>
    </section>

    <!-- Gravies / Main Course -->
    <section class="menu-section">
      <h3>GRAVIES</h3>
      <div class="menu-grid">
        <article class="card">
          <img src="paneer.jpg" alt="Paneer Tikka">
          <div class="card-body">
            <h4>PANEER TIKKA</h4>
            <p class="price">₹179</p>
          </div>
        </article>

        <article class="card">
          <img src="panner_bm.jpg" alt="Paneer Butter Masala">
          <div class="card-body">
            <h4>PANEER BUTTER MASALA</h4>
            <p class="price">₹159</p>
          </div>
        </article>

        <article class="card">
          <img src="chicken_g.jpg" alt="Chicken Gravy">
          <div class="card-body">
            <h4>CHICKEN GRAVY</h4>
            <p class="price">₹199</p>
          </div>
        </article>
      </div>
    </section>

    <!-- Juices & Shakes -->
    <section class="menu-section">
      <h3>JUICES & MILKSHAKES</h3>
      <div class="menu-grid">
        <article class="card small">
          <img src="lemon.jpg" alt="Lemon Juice">
          <div class="card-body"><h4>LEMON JUICE</h4><p class="price">₹49</p></div>
        </article>

        <article class="card small">
          <img src="apple.jpg" alt="Apple Juice">
          <div class="card-body"><h4>APPLE JUICE</h4><p class="price">₹59</p></div>
        </article>

        <article class="card small">
          <img src="chocolate.jpg" alt="Chocolate Milkshake">
          <div class="card-body"><h4>CHOCOLATE MILKSHAKE</h4><p class="price">₹49</p></div>
        </article>

        <article class="card small">
          <img src="oreo.jpg" alt="Oreo Milkshake">
          <div class="card-body"><h4>OREO MILKSHAKE</h4><p class="price">₹69</p></div>
        </article>
      </div>
    </section>

    <!-- Ice Creams -->
    <section class="menu-section">
      <h3>ICE CREAMS</h3>
      <div class="menu-grid">
        <article class="card small">
          <img src="choco_ice.jpg" alt="Chocolate Ice Cream">
          <div class="card-body"><h4>CHOCOLATE ICE CREAM</h4><p class="price">₹59</p></div>
        </article>

        <article class="card small">
          <img src="butterscotch-ice-cream-recipe.jpg" alt="Butterscotch Ice Cream">
          <div class="card-body"><h4>BUTTERSCOTCH</h4><p class="price">₹99</p></div>
        </article>

        <article class="card small">
          <img src="black-currant-ice-cream.jpeg" alt="Blackcurrant Ice Cream">
          <div class="card-body"><h4>BLACKCURRANT</h4><p class="price">₹99</p></div>
        </article>
      </div>
    </section>

  </main>
</body>
</html>

menu.css
:root{
  --accent:#e63946; --bg:#121212; --panel:#1f1f1f; --muted:#cfcfcf;
}
*{box-sizing:border-box;}
body{margin:0; font-family:"Poppins", Arial, sans-serif; background:var(--bg); color:#fff;}
nav{display:flex; justify-content:space-between; align-items:center; padding:16px 32px; background:#141414;}
.logo{display:flex;align-items:center;gap:12px;}
.logo img{width:46px;height:46px;}
.logo h1{color:var(--accent); margin:0;}
nav ul{display:flex; gap:18px; list-style:none; margin:0; padding:0;}
nav a{color:#fff; text-decoration:none; font-weight:600;}
nav a:hover{color:var(--accent);}

.menu-main{padding:28px;}
.page-title{text-align:center;color:var(--accent); margin:8px 0 20px 0; font-size:28px;}

.menu-section{margin:28px auto; width:92%; max-width:1100px; background:transparent; padding:0 6px;}
.menu-section h3{color:var(--accent); margin:12px 0;}

.menu-grid{
  display:grid;
  grid-template-columns: repeat(auto-fit,minmax(220px,1fr));
  gap:18px;
}

.card{
  background:var(--panel);
  border-radius:12px;
  overflow:hidden;
  box-shadow:0 8px 24px rgba(0,0,0,0.5);
  display:flex;
  flex-direction:column;
}
.card.small{min-height:220px;}
.card img{width:100%; height:170px; object-fit:cover; display:block;}
.card-body{padding:12px;}
.card-body h4{margin:0 0 8px 0; font-size:16px; text-transform:uppercase;}
.price{font-weight:700; color:var(--muted);}

@media (max-width:520px){
  .card img{height:140px;}
  nav{padding:12px;}
}

admin.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>OXHEART - Admin</title>
  <link rel="stylesheet" href="admin.css">
</head>
<body>
  <h2>Shreeshanth R - 25012265</h2>
  <nav>
    <div class="logo">
      <img src="https://cdn-icons-png.flaticon.com/512/857/857681.png" alt="logo">
      <h1>OXHEART</h1>
    </div>
    <ul>
      <li><a href="home.html">Home</a></li>
      <li><a href="menu.html">Menu</a></li>
      <li><a href="admin.html">Admin</a></li>
      <li><a href="contact.html">Contact Us</a></li>
    </ul>
  </nav>

  <main>
    <h2 class="title">ADMIN TEAM</h2>

    <section class="team">
      <figure class="member">
        <div class="badge">1</div>
        <img src="founder.avif" alt="member 1">
        <figcaption>
          <div class="role">FOUNDER</div>
          <div class="name">ALEX TURNER</div>
        </figcaption>
      </figure>

      <figure class="member">
        <div class="badge">2</div>
        <img src="manger.jpg" alt="member 2">
        <figcaption>
          <div class="role">MANAGER CHAIRMAN</div>
          <div class="name">SHAWN MENDES</div>
        </figcaption>
      </figure>

      <figure class="member">
        <div class="badge">3</div>
        <img src="lana.jpg" alt="member 3">
        <figcaption>
          <div class="role">EXECUTIVE CHIEF</div>
          <div class="name">LANA DEL REY</div>
        </figcaption>
      </figure>

      <figure class="member">
        <div class="badge">4</div>
        <img src="messi.avif" alt="member 4">
        <figcaption>
          <div class="role">DIRECTOR</div>
          <div class="name">LIONEL MESSI</div>
        </figcaption>
      </figure>
    </section>
  </main>
</body>
</html>

admin.css
:root{--accent:#e63946; --bg:#121212; --panel:#1f1f1f;}
*{box-sizing:border-box;}
body{margin:0; font-family:"Poppins", Arial, sans-serif; background:var(--bg); color:#fff;}
nav{display:flex; justify-content:space-between; align-items:center; padding:16px 32px; background:#141414;}
.logo{display:flex;align-items:center;gap:12px;}
.logo img{width:46px;height:46px;}
.logo h1{color:var(--accent); margin:0;}
nav ul{display:flex; gap:18px; list-style:none; margin:0; padding:0;}
nav a{color:#fff; text-decoration:none;}
nav a:hover{color:var(--accent);}

.title{text-align:center; color:var(--accent); margin-top:26px; font-size:26px;}
.team{display:flex; gap:28px; justify-content:center; flex-wrap:wrap; padding:28px;}

.member{
  background:var(--panel);
  width:260px;
  border-radius:12px;
  overflow:hidden;
  position:relative;
  box-shadow:0 10px 30px rgba(0,0,0,0.5);
  text-align:center;
}
.member img{width:100%; height:260px; object-fit:cover; display:block;}
.member figcaption{padding:14px;}
.role{font-weight:800; text-transform:uppercase; color:var(--accent); margin-bottom:6px;}
.name{font-weight:900; text-transform:uppercase; color:#fff; letter-spacing:0.6px;}


.badge{
  position:absolute;
  left:12px; top:12px;
  background:var(--accent);
  width:36px; height:36px;
  border-radius:50%;
  display:flex; align-items:center; justify-content:center;
  font-weight:800; color:#fff;
  box-shadow: 0 6px 18px rgba(0,0,0,0.5);
}
@media (max-width:600px){
  .member{width:46%;}
}
@media (max-width:420px){
  .member{width:100%;}
}

contact.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <title>OXHEART - Contact</title>
  <link rel="stylesheet" href="contact.css">
</head>
<body class="contact-bg">
  <nav>
    <div class="logo">
      <img src="https://cdn-icons-png.flaticon.com/512/857/857681.png" alt="Oxheart logo">
      <h1>OXHEART</h1>
    </div>
    <ul>
      <li><a href="home.html">Home</a></li>
      <li><a href="menu.html">Menu</a></li>
      <li><a href="admin.html">Admin</a></li>
      <li><a href="contact.html">Contact Us</a></li>
    </ul>
  </nav>

  <main class="contact-main">
    <div class="contact-card">
      <h2>CONTACT US</h2>
      <p><strong>CONTACT NUMBER:</strong> 9933345459</p>
      <p><strong>ADDRESS:</strong> NO.210/A, GRAND AVENUE STREET, COIMBATORE, TAMIL NADU - 641001</p>
      <p><strong>EMAIL:</strong> INFO@OXHEARTRESTAURANT.COM</p>
    </div>
  </main>

  <!-- small hidden img if you want the raw file named "bg" accessible in markup -->
  <img src="restaurent.jpg" alt="bg" style="display:none;">
</body>
</html>

contact.css
:root{--accent:#e63946; --bg:#121212; --panel:#1f1f1f;}
*{box-sizing:border-box;}
html,body{height:100%; margin:0; font-family:"Poppins", Arial, sans-serif; color:#fff;}
.contact-bg{
  background-image: url('restaurent.jpg');
  background-size: cover;
  background-position: center;
  min-height:100vh;
}

.contact-main{
  min-height:100vh;
  background: linear-gradient(rgba(0,0,0,0.55), rgba(0,0,0,0.55));
  display:flex;
  align-items:center;
  justify-content:center;
  padding:40px;
}
.contact-card{
  width:82%;
  max-width:720px;
  background: rgba(0,0,0,0.62);
  padding:34px;
  border-radius:14px;
  box-shadow:0 12px 40px rgba(0,0,0,0.6);
  text-align:left;
}
.contact-card h2{color:var(--accent); margin-top:0; text-transform:uppercase;}
.contact-card p{font-size:16px; margin:8px 0;}
@media (max-width:600px){
  .contact-card{width:94%; padding:20px;}
  nav{padding:12px;}
}
```

## OUTPUT:
![alt text](<Screenshot (50).png>)
![alt text](<Screenshot (51).png>)
![alt text](<Screenshot (52).png>)
![alt text](<Screenshot (53).png>)
![alt text](<Screenshot (54).png>)
![alt text](<Screenshot (56).png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
