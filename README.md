# smash-arena
Premium Badminton Court and Academy Website
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>SMASH ARENA | Premium Badminton Academy</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:Arial,Helvetica,sans-serif;
    background:#07111f;
    color:#ffffff;
    overflow-x:hidden;
}

/* ================= NAVBAR ================= */

header{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    z-index:1000;

    padding:20px 7%;

    display:flex;
    justify-content:space-between;
    align-items:center;

    background:rgba(7,17,31,.92);
    backdrop-filter:blur(12px);

    border-bottom:1px solid rgba(255,255,255,.08);
}

.logo{
    font-size:26px;
    font-weight:900;
    letter-spacing:1px;
}

.logo span{
    color:#39ff88;
}

nav a{
    color:white;
    text-decoration:none;
    margin-left:28px;
    font-size:14px;
    font-weight:bold;
    transition:.3s;
}

nav a:hover{
    color:#39ff88;
}

/* ================= HERO ================= */

.hero{

    min-height:100vh;

    display:flex;
    align-items:center;

    padding:120px 7% 70px;

    position:relative;

    background:
    linear-gradient(90deg,
    rgba(3,10,18,.95) 0%,
    rgba(3,10,18,.72) 45%,
    rgba(3,10,18,.25) 100%),

    url("https://images.unsplash.com/photo-1626224583764-f87db24ac4ea?auto=format&fit=crop&w=1800&q=90");

    background-size:cover;
    background-position:center;
}

.hero-content{
    max-width:800px;
    animation:fadeUp 1s ease;
}

.badge{
    display:inline-block;

    padding:10px 18px;

    border:1px solid #39ff88;
    border-radius:30px;

    color:#39ff88;

    font-size:13px;
    font-weight:bold;

    margin-bottom:25px;
}

.hero h1{
    font-size:75px;
    line-height:1.02;

    margin-bottom:25px;

    letter-spacing:-3px;
}

.hero h1 span{
    color:#39ff88;
}

.hero p{
    color:#d1d5db;

    font-size:19px;
    line-height:1.7;

    max-width:650px;

    margin-bottom:35px;
}

.buttons{
    display:flex;
    gap:12px;
    flex-wrap:wrap;
}

.btn{
    display:inline-block;

    padding:15px 28px;

    border-radius:8px;

    text-decoration:none;

    font-weight:bold;

    transition:.3s;
}

.primary{
    background:#39ff88;
    color:#03100a;
}

.primary:hover{
    transform:translateY(-3px);
    box-shadow:0 10px 30px rgba(57,255,136,.25);
}

.outline{
    border:1px solid rgba(255,255,255,.5);
    color:white;
}

.outline:hover{
    border-color:#39ff88;
    color:#39ff88;
}

/* ================= STATS ================= */

.stats{

    display:grid;
    grid-template-columns:repeat(4,1fr);

    gap:1px;

    background:#263244;

    border-top:1px solid #263244;
    border-bottom:1px solid #263244;
}

.stat{
    text-align:center;

    padding:30px 15px;

    background:#0b1728;
}

.stat h2{
    color:#39ff88;
    font-size:32px;
}

.stat p{
    color:#9ca3af;
    margin-top:7px;
    font-size:13px;
}

/* ================= GENERAL SECTION ================= */

.section{
    padding:100px 7%;
}

.section-header{
    max-width:700px;
    margin-bottom:55px;
}

.section-header.center{
    text-align:center;
    margin-left:auto;
    margin-right:auto;
}

.eyebrow{
    color:#39ff88;

    font-size:13px;

    font-weight:bold;

    text-transform:uppercase;

    letter-spacing:2px;

    margin-bottom:15px;
}

.section h2{
    font-size:45px;
    margin-bottom:18px;
}

.section-header p{
    color:#9ca3af;
    line-height:1.7;
}

/* ================= FEATURES ================= */

.features{

    display:grid;

    grid-template-columns:repeat(3,1fr);

    gap:22px;
}

.feature{

    background:#0d1a2c;

    border:1px solid #1c2a3d;

    padding:35px;

    border-radius:15px;

    transition:.3s;
}

.feature:hover{

    transform:translateY(-7px);

    border-color:#39ff88;

}

.feature-icon{
    font-size:38px;
    margin-bottom:22px;
}

.feature h3{
    font-size:20px;
    margin-bottom:12px;
}

.feature p{
    color:#9ca3af;
    line-height:1.6;
}

/* ================= PRICING ================= */

.pricing-section{
    background:#f5f7fa;
    color:#07111f;
}

.pricing{

    display:grid;

    grid-template-columns:repeat(3,1fr);

    gap:25px;
}

.price-card{

    background:white;

    padding:35px;

    border-radius:18px;

    border:1px solid #e5e7eb;

    position:relative;

    transition:.3s;
}

.price-card:hover{
    transform:translateY(-8px);
}

.price-card.featured{

    border:3px solid #39c878;

    box-shadow:0 20px 50px rgba(0,0,0,.12);

}

.popular{

    position:absolute;

    top:-15px;
    right:20px;

    background:#39c878;

    color:#03100a;

    padding:7px 14px;

    border-radius:20px;

    font-size:12px;

    font-weight:bold;
}

.price-card h3{
    font-size:22px;
}

.price{

    font-size:45px;

    font-weight:900;

    margin:20px 0;
}

.price small{
    font-size:14px;
    color:#6b7280;
}

.price-card ul{

    list-style:none;

    margin:20px 0 30px;

    line-height:2.2;

    color:#4b5563;
}

/* ================= COACHING ================= */

.coaching{

    display:grid;

    grid-template-columns:1fr 1fr;

    gap:30px;
}

.coach{

    min-height:300px;

    padding:35px;

    display:flex;

    flex-direction:column;

    justify-content:flex-end;

    border-radius:18px;

    overflow:hidden;

    background-size:cover;

    background-position:center;

    position:relative;
}

.coach::before{

    content:"";

    position:absolute;

    inset:0;

    background:linear-gradient(
        transparent,
        rgba(0,0,0,.9)
    );
}

.coach-content{

    position:relative;

    z-index:1;
}

.coach h3{
    font-size:27px;
    margin-bottom:10px;
}

.coach p{
    color:#d1d5db;
    line-height:1.6;
}

/* ================= BOOKING ================= */

.booking-section{
    background:#0b1728;
}

.booking-container{

    max-width:850px;

    margin:auto;

    background:#101f32;

    padding:40px;

    border-radius:20px;

    border:1px solid #24344a;
}

.form-grid{

    display:grid;

    grid-template-columns:1fr 1fr;

    gap:18px;
}

.form-group label{

    display:block;

    margin-bottom:8px;

    font-size:13px;

    color:#9ca3af;
}

.form-group input,
.form-group select{

    width:100%;

    padding:15px;

    border-radius:8px;

    border:1px solid #304157;

    background:#07111f;

    color:white;

    outline:none;
}

.form-group input:focus,
.form-group select:focus{

    border-color:#39ff88;

}

.full{
    grid-column:1/-1;
}

.submit-btn{

    width:100%;

    margin-top:20px;

    padding:16px;

    border:none;

    border-radius:8px;

    background:#39ff88;

    color:#03100a;

    font-weight:bold;

    font-size:16px;

    cursor:pointer;

}

/* ================= REVIEWS ================= */

.reviews{

    display:grid;

    grid-template-columns:repeat(3,1fr);

    gap:22px;
}

.review{

    background:#0d1a2c;

    padding:30px;

    border-radius:15px;

    border:1px solid #1c2a3d;
}

.stars{

    color:#39ff88;

    font-size:20px;

    margin-bottom:15px;
}

.review p{

    color:#cbd5e1;

    line-height:1.7;

    margin-bottom:20px;
}

.review strong{
    color:white;
}

/* ================= CTA ================= */

.cta{

    padding:90px 7%;

    text-align:center;

    background:

    linear-gradient(
        rgba(57,200,120,.9),
        rgba(57,200,120,.9)
    ),

    url("https://images.unsplash.com/photo-1626224583764-f87db24ac4ea?auto=format&fit=crop&w=1600&q=80");

    background-size:cover;

    color:#03100a;
}

.cta h2{
    font-size:48px;
    margin-bottom:15px;
}

.cta p{
    margin-bottom:28px;
}

.dark-btn{
    background:#07111f;
    color:white;
}

/* ================= FOOTER ================= */

footer{

    background:#030912;

    padding:50px 7%;

    display:flex;

    justify-content:space-between;

    align-items:center;

    flex-wrap:wrap;

    gap:20px;
}

footer p{
    color:#6b7280;
    font-size:13px;
}

/* ================= CHAT ================= */

.chat-button{

    position:fixed;

    right:25px;

    bottom:25px;

    width:62px;
    height:62px;

    border-radius:50%;

    border:none;

    background:#39ff88;

    font-size:27px;

    cursor:pointer;

    z-index:3000;

    box-shadow:0 10px 30px rgba(0,0,0,.4);

    transition:.3s;
}

.chat-button:hover{
    transform:scale(1.08);
}

.chat-box{

    display:none;

    position:fixed;

    right:25px;

    bottom:100px;

    width:340px;

    background:white;

    color:#111;

    border-radius:18px;

    overflow:hidden;

    z-index:3000;

    box-shadow:0 20px 60px rgba(0,0,0,.4);
}

.chat-header{

    background:#07111f;

    color:white;

    padding:18px;

    font-weight:bold;
}

.chat-status{

    color:#39ff88;

    font-size:12px;

    margin-top:5px;
}

.chat-body{
    padding:20px;
}

.chat-message{

    background:#f1f5f9;

    padding:12px;

    border-radius:10px;

    font-size:14px;

    margin-bottom:15px;

    line-height:1.5;
}

.chat-body input{

    width:100%;

    padding:13px;

    border:1px solid #ddd;

    border-radius:8px;

    outline:none;
}

.chat-body button{

    width:100%;

    margin-top:10px;

    padding:13px;

    border:none;

    border-radius:8px;

    background:#39c878;

    font-weight:bold;

    cursor:pointer;
}

/* ================= ANIMATION ================= */

@keyframes fadeUp{

    from{

        opacity:0;

        transform:translateY(30px);

    }

    to{

        opacity:1;

        transform:translateY(0);

    }

}

/* ================= MOBILE ================= */

@media(max-width:800px){

    nav{
        display:none;
    }

    .hero h1{
        font-size:48px;
        letter-spacing:-2px;
    }

    .hero p{
        font-size:16px;
    }

    .stats{
        grid-template-columns:1fr 1fr;
    }

    .features,
    .pricing,
    .reviews{
        grid-template-columns:1fr;
    }

    .coaching{
        grid-template-columns:1fr;
    }

    .form-grid{
        grid-template-columns:1fr;
    }

    .full{
        grid-column:auto;
    }

    .section h2{
        font-size:34px;
    }

    .chat-box{
        right:15px;
        bottom:90px;
        width:calc(100% - 30px);
    }

    footer{
        text-align:center;
        justify-content:center;
    }

}

</style>
</head>


<body>


<!-- NAVBAR -->

<header>

<div class="logo">
🏸 <span>SMASH</span> ARENA
</div>

<nav>

<a href="#home">Home</a>

<a href="#facilities">Facilities</a>

<a href="#pricing">Pricing</a>

<a href="#coaching">Coaching</a>

<a href="#booking">Booking</a>

<a href="#contact">Contact</a>

</nav>

</header>


<!-- HERO -->

<section class="hero" id="home">

<div class="hero-content">

<div class="badge">
PREMIUM BADMINTON EXPERIENCE
</div>

<h1>

PLAY HARD.<br>

<span>SMASH HARDER.</span>

</h1>

<p>

Train. Compete. Improve.

Experience premium badminton courts,
professional coaching and a community
built for players who love the game.

</p>

<div class="buttons">

<a href="#booking" class="btn primary">
🏸 BOOK YOUR COURT
</a>

<a href="#coaching" class="btn outline">
VIEW COACHING
</a>

</div>

</div>

</section>


<!-- STATS -->

<section class="stats">

<div class="stat">

<h2>6+</h2>

<p>Premium Courts</p>

</div>

<div class="stat">

<h2>500+</h2>

<p>Active Players</p>

</div>

<div class="stat">

<h2>8+</h2>

<p>Expert Coaches</p>

</div>

<div class="stat">

<h2>4.9★</h2>

<p>Player Rating</p>

</div>

</section>


<!-- FACILITIES -->

<section class="section" id="facilities">

<div class="section-header center">

<div class="eyebrow">
THE SMASH EXPERIENCE
</div>

<h2>
Built For Players.
</h2>

<p>
Everything you need to train, compete and enjoy
badminton at your best.
</p>

</div>


<div class="features">


<div class="feature">

<div class="feature-icon">
🏸
</div>

<h3>
Professional Courts
</h3>

<p>
Premium badminton courts designed
for comfortable recreational and
competitive play.
</p>

</div>


<div class="feature">

<div class="feature-icon">
💡
</div>

<h3>
Tournament Lighting
</h3>

<p>
Bright professional lighting provides
excellent visibility during every match.
</p>

</div>


<div class="feature">

<div class="feature-icon">
❄️
</div>

<h3>
Comfortable Environment
</h3>

<p>
A clean and comfortable environment
so you can focus completely on your game.
</p>

</div>


<div class="feature">

<div class="feature-icon">
🚿
</div>

<h3>
Player Facilities
</h3>

<p>
Changing rooms, drinking water and
essential facilities for players.
</p>

</div>


<div class="feature">

<div class="feature-icon">
🏆
</div>

<h3>
Competition Ready
</h3>

<p>
Train with players of different levels
and prepare for competitive matches.
</p>

</div>


<div class="feature">

<div class="feature-icon">
👥
</div>

<h3>
Player Community
</h3>

<p>
Meet badminton enthusiasts and
find new partners to play with.
</p>

</div>


</div>

</section>


<!-- PRICING -->

<section class="section pricing-section" id="pricing">

<div class="section-header center">

<div class="eyebrow">
MEMBERSHIP
</div>

<h2>
Simple Pricing.
</h2>

<p>
Choose the plan that fits your game.
</p>

</div>


<div class="pricing">


<div class="price-card">

<h3>
Hourly Court
</h3>

<div class="price">
₹250 <small>/ hour</small>
</div>

<ul>

<li>✓ Premium court</li>

<li>✓ Professional lighting</li>

<li>✓ Player facilities</li>

<li>✓ Flexible booking</li>

</ul>

<a href="#booking" class="btn primary">
Book Court
</a>

</div>


<div class="price-card featured">

<div class="popular">
MOST POPULAR
</div>

<h3>
Monthly Member
</h3>

<div class="price">
₹2,499 <small>/ month</small>
</div>

<ul>

<li>✓ Regular court access</li>

<li>✓ Priority booking</li>

<li>✓ Member benefits</li>

<li>✓ Community access</li>

</ul>

<a href="#booking" class="btn primary">
Become Member
</a>

</div>


<div class="price-card">

<h3>
Academy Training
</h3>

<div class="price">
₹1,999 <small>/ month</small>
</div>

<ul>

<li>✓ Professional coaching</li>

<li>✓ Training sessions</li>

<li>✓ Fitness development</li>

<li>✓ Performance guidance</li>

</ul>

<a href="#coaching" class="btn primary">
Join Academy
</a>

</div>


</div>

</section>


<!-- COACHING -->

<section class="section" id="coaching">

<div class="section-header center">

<div class="eyebrow">
SMASH ACADEMY
</div>

<h2>
Train Like A Champion.
</h2>

<p>
Structured programs for every level of player.
</p>

</div>


<div class="coaching">


<div class="coach"

style="background-image:url('https://images.unsplash.com/photo-1626224583764-f87db24ac4ea?auto=format&fit=crop&w=900&q=80');">

<div class="coach-content">

<h3>
Beginner Program
</h3>

<p>
Learn fundamentals, footwork,
serving and basic strokes.
</p>

</div>

</div>


<div class="coach"

style="background-image:url('https://images.unsplash.com/photo-1624526267942-ab0ff8a3e972?auto=format&fit=crop&w=900&q=80');">

<div class="coach-content">

<h3>
Advanced Training
</h3>

<p>
Improve speed, power, strategy,
smashes and competitive skills.
</p>

</div>

</div>


<div class="coach"

style="background-image:url('https://images.unsplash.com/photo-1626224583764-f87db24ac4ea?auto=format&fit=crop&w=900&q=80');">

<div class="coach-content">

<h3>
Kids Academy
</h3>

<p>
Fun and structured training designed
for young players.
</p>

</div>

</div>


<div class="coach"

style="background-image:url('https://images.unsplash.com/photo-1624526267942-ab0ff8a3e972?auto=format&fit=crop&w=900&q=80');">

<div class="coach-content">

<h3>
Performance Training
</h3>

<p>
Build agility, stamina, coordination
and match fitness.
</p>

</div>

</div>


</div>

</section>


<!-- BOOKING -->

<section class="section booking-section" id="booking">

<div class="section-header center">

<div class="eyebrow">
COURT RESERVATION
</div>

<h2>
Book Your Court.
</h2>

<p>
Choose your preferred date and time.
</p>

</div>


<div class="booking-container">

<div class="form-grid">


<div class="form-group">

<label>
Full Name
</label>

<input
type="text"
id="name"
placeholder="Enter your name"
>

</div>


<div class="form-group">

<label>
Phone Number
</label>

<input
type="tel"
id="phone"
placeholder="Enter phone number"
>

</div>


<div class="form-group">

<label>
Date
</label>

<input
type="date"
id="date"
>

</div>


<div class="form-group">

<label>
Time Slot
</label>

<select id="time">

<option>
Select time
</option>

<option>
6:00 AM - 7:00 AM
</option>

<option>
7:00 AM - 8:00 AM
</option>

<option>
8:00 AM - 9:00 AM
</option>

<option>
5:00 PM - 6:00 PM
</option>

<option>
6:00 PM - 7:00 PM
</option>

<option>
7:00 PM - 8:00 PM
</option>

<option>
8:00 PM - 9:00 PM
</option>

</select>

</div>


<div class="form-group full">

<label>
Select Service
</label>

<select id="service">

<option>
Court Booking
</option>

<option>
Monthly Membership
</option>

<option>
Badminton Coaching
</option>

<option>
Kids Academy
</option>

</select>

</div>


</div>


<button class="submit-btn" onclick="bookCourt()">

🏸 SEND BOOKING REQUEST

</button>

</div>

</section>


<!-- REVIEWS -->

<section class="section">

<div class="section-header center">

<div class="eyebrow">
PLAYER REVIEWS
</div>

<h2>
Loved By Players.
</h2>

</div>


<div class="reviews">


<div class="review">

<div class="stars">
★★★★★
</div>

<p>
"Excellent courts and a great atmosphere.
I play here every weekend."
</p>

<strong>
— Rahul
</strong>

</div>


<div class="review">

<div class="stars">
★★★★★
</div>

<p>
"The coaching has improved my footwork
and confidence tremendously."
</p>

<strong>
— Ananya
</strong>

</div>


<div class="review">

<div class="stars">
★★★★★
</div>

<p>
"Clean courts, friendly staff and
very reasonable pricing."
</p>

<strong>
— Kiran
</strong>

</div>


</div>

</section>


<!-- CTA -->

<section class="cta" id="contact">

<h2>
READY TO PLAY?
</h2>

<p>
Book your court and experience Smash Arena.
</p>

<a
href="https://wa.me/919999999999"
target="_blank"
class="btn dark-btn"
>
📲 CHAT ON WHATSAPP
</a>

</section>


<!-- FOOTER -->

<footer>

<div>

<div class="logo">
🏸 <span>SMASH</span> ARENA
</div>

<p style="margin-top:10px;">
Premium Badminton Court & Academy
</p>

</div>

<div>

<p>
📍 Bangalore
</p>

<p style="margin-top:7px;">
📞 +91 99999 99999
</p>

</div>

</footer>


<!-- CHAT BUTTON -->

<button
class="chat-button"
onclick="toggleChat()"
>
💬
</button>


<!-- CHAT BOX -->

<div class="chat-box" id="chatBox">

<div class="chat-header">

🏸 Smash Arena Support

<div class="chat-status">
● Online
</div>

</div>


<div class="chat-body">

<div class="chat-message">

Hi! 👋 Welcome to Smash Arena.

How can we help you today?

</div>


<input
type="text"
id="chatMessage"
placeholder="Ask about booking, price..."
>


<button onclick="sendMessage()">
Send to WhatsApp
</button>

</div>

</div>


<script>

/* BOOKING */

function bookCourt(){

    let name =
    document.getElementById("name").value;

    let phone =
    document.getElementById("phone").value;

    let date =
    document.getElementById("date").value;

    let time =
    document.getElementById("time").value;

    let service =
    document.getElementById("service").value;


    if(
        name === "" ||
        phone === "" ||
        date === ""
    ){

        alert(
            "Please complete your booking details."
        );

        return;

    }


    let message =
    "Hello Smash Arena!%0A%0A" +

    "🏸 New Booking Request%0A%0A" +

    "Name: " + name + "%0A" +

    "Phone: " + phone + "%0A" +

    "Date: " + date + "%0A" +

    "Time: " + time + "%0A" +

    "Service: " + service;


    window.open(
        "https://wa.me/919999999999?text=" +
        message,
        "_blank"
    );

}


/* CHAT */

function toggleChat(){

    let chat =
    document.getElementById("chatBox");

    if(chat.style.display === "block"){

        chat.style.display = "none";

    }

    else{

        chat.style.display = "block";

    }

}


/* CHAT MESSAGE */

function sendMessage(){

    let message =
    document.getElementById("chatMessage").value;


    if(message === ""){

        alert(
            "Please type your question."
        );

        return;

    }


    let whatsappMessage =

    "Hello Smash Arena!%0A%0A" +

    "💬 Customer Question:%0A" +

    message;


    window.open(

        "https://wa.me/919999999999?text=" +

        whatsappMessage,

        "_blank"

    );

}

</script>


</body>
</html>
