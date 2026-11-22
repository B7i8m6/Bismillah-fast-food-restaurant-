# Bismillah-fast-food-restaurant-
{
  "appId": "com.bismillahhotel.app",
  "appName": "Bismillah Hotel",
  "webDir": ".",
  "bundledWebRuntime": false
}
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#17110b">
<meta name="description" content="Bismillah Hotel family restaurant in Cowl Bazar, Ballari. View our menu and order on WhatsApp.">
<title>Bismillah Hotel | Family Restaurant</title>
<link rel="manifest" href="manifest.json">
<link rel="icon" href="icon.svg" type="image/svg+xml">
<style>
:root{--bg:#100d09;--panel:#1e1710;--panel2:#2a2015;--gold:#e6b84f;--gold2:#bd8628;--cream:#fff6e5;--muted:#c5b79e;--green:#198754;--red:#b83232}
*{box-sizing:border-box}html{scroll-behavior:smooth}body{margin:0;background:#faf6ee;color:#21180e;font-family:Arial,Helvetica,sans-serif}
header{background:var(--bg);color:white;position:sticky;top:0;z-index:10;box-shadow:0 3px 14px #0003}
.top{max-width:1150px;margin:auto;padding:14px 20px;display:flex;align-items:center;justify-content:space-between;gap:12px}
.brand{font-weight:900;letter-spacing:2px;color:var(--gold);font-size:clamp(20px,4vw,28px)}.tag{font-size:11px;color:#e9dfcc;letter-spacing:2px;margin-top:4px}
nav{display:flex;gap:16px;flex-wrap:wrap}nav a{color:#fff;text-decoration:none;font-size:14px}nav a:hover{color:var(--gold)}
.hero{min-height:420px;background:linear-gradient(90deg,#080604e8,#08060488),url('https://images.unsplash.com/photo-1589302168068-964664d93dc0?auto=format&fit=crop&w=1800&q=85') center/cover;display:flex;align-items:center;color:white}
.hero-inner{max-width:1150px;margin:auto;width:100%;padding:65px 22px}.eyebrow{color:var(--gold);font-weight:bold;letter-spacing:3px;text-transform:uppercase}.hero h1{font-size:clamp(38px,7vw,68px);margin:12px 0;max-width:700px}.hero p{font-size:18px;color:#f0e8d9;max-width:520px;line-height:1.6}
.btn{border:0;border-radius:7px;padding:12px 18px;background:var(--gold);color:#1b1207;font-weight:bold;text-decoration:none;display:inline-block;cursor:pointer}.btn:hover{background:#f2cb70}.btn.dark{background:var(--panel);color:var(--gold);border:1px solid var(--gold2)}.btn.small{padding:8px 11px;font-size:13px}
section{padding:54px 20px}.wrap{max-width:1150px;margin:auto}.section-head{text-align:center;margin-bottom:28px}.section-head .eyebrow{font-size:12px}.section-head h2{font-size:clamp(26px,4vw,38px);margin:9px 0;color:#281b0d}.section-head p{color:#756958;margin:0}
.notice{background:#fff1cc;border:1px solid #e8c66e;padding:12px 15px;border-radius:9px;margin:0 auto 22px;max-width:900px;font-size:14px;line-height:1.5}
.menu-tabs{display:flex;gap:8px;justify-content:center;flex-wrap:wrap;margin-bottom:24px}.tab{border:1px solid #c9b58e;background:white;padding:10px 15px;border-radius:30px;cursor:pointer;font-weight:bold}.tab.active{background:var(--panel);color:var(--gold);border-color:var(--panel)}
.menu-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:15px}.dish{background:white;border:1px solid #eee2cc;border-radius:12px;padding:17px;box-shadow:0 5px 16px #321a090c;display:flex;flex-direction:column;gap:9px}.dish h3{margin:0;font-size:17px}.dish .price{font-size:20px;color:#9a6715;font-weight:800}.dish .desc{font-size:12px;color:#847866;min-height:15px}.dish .btn{margin-top:auto}.unavailable{opacity:.58}.unavailable .btn{background:#999;color:white;cursor:not-allowed}
.dark-section{background:var(--bg);color:white}.dark-section .section-head h2{color:var(--gold)}.dark-section .section-head p{color:var(--muted)}
.info-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:16px}.info-card{background:var(--panel);border:1px solid #49351d;border-radius:12px;padding:22px}.info-card h3{color:var(--gold);margin-top:0}.info-card p{color:#eee1cd;line-height:1.6;margin-bottom:0}
footer{background:#090705;color:#d7c9b2;text-align:center;padding:26px 16px;font-size:13px}.footer-brand{font-size:21px;color:var(--gold);font-weight:900;letter-spacing:2px}
.float-cart{position:fixed;right:18px;bottom:18px;z-index:20;box-shadow:0 4px 18px #0004}
.modal-backdrop{position:fixed;inset:0;background:#0009;display:none;align-items:center;justify-content:center;padding:15px;z-index:50}.modal-backdrop.show{display:flex}.modal{background:#fffaf0;border-radius:14px;padding:22px;width:min(520px,100%);max-height:85vh;overflow:auto}.modal h2{margin-top:0}.modal-row{display:flex;justify-content:space-between;align-items:center;gap:12px;border-bottom:1px solid #e8ddc9;padding:10px 0}.qty{display:flex;align-items:center;gap:8px}.qty button{width:28px;height:28px;border:0;border-radius:5px;background:#e9d5a8;cursor:pointer;font-weight:bold}
.admin{background:#f1eadc}.admin-box{background:#fff;border:1px solid #e0d3bb;border-radius:12px;padding:18px;margin:12px 0}.admin-row{display:grid;grid-template-columns:1fr 95px 70px;gap:10px;align-items:center;padding:10px 0;border-bottom:1px solid #eee}.admin-row:last-child{border:0}.admin-row input{width:100%;padding:8px;border:1px solid #d4c7af;border-radius:6px}.switch{border:0;border-radius:20px;padding:8px 12px;color:white;font-weight:bold;cursor:pointer}.on{background:var(--green)}.off{background:var(--red)}.hidden{display:none!important}.admin-note{font-size:13px;line-height:1.5;color:#715d3e}.two-col{display:grid;grid-template-columns:1fr 1fr;gap:12px}
@media(max-width:650px){.top{align-items:flex-start;flex-direction:column}nav{gap:12px}.hero{min-height:360px}.admin-row{grid-template-columns:1fr 78px 58px}.two-col{grid-template-columns:1fr}}
</style>
</head>
<body>
<header><div class="top">
 <div><div class="brand">BISMILLAH HOTEL</div><div class="tag">FAMILY RESTAURANT · BALLARI</div></div>
 <nav><a href="#home">Home</a><a href="#menu">Menu</a><a href="#hours">Hours</a><a href="#location">Location</a><a href="#contact">Contact</a><a href="#admin">Admin</a></nav>
</div></header>
<main>
<section class="hero" id="home"><div class="hero-inner">
 <div class="eyebrow">Welcome to Bismillah Hotel</div>
 <h1>Good Food.<br>Great Family Moments.</h1>
 <p>Enjoy biryani favourites and delicious mutton and chicken specials in a welcoming family restaurant.</p>
 <a class="btn" href="#menu">Explore Menu</a>
</div></section>

<section id="menu"><div class="wrap">
 <div class="section-head"><div class="eyebrow">Freshly prepared</div><h2>Our Menu</h2><p>Choose your favourites and send your order through WhatsApp.</p></div>
 <div class="notice"><strong>Biryani pricing:</strong> Special rates apply Wednesday, Friday and Sunday. Weekday rates apply on the other days. <strong>Mutton and chicken specials:</strong> Sunday to Friday. Availability can be changed by the restaurant.</div>
 <div class="menu-tabs" id="menuTabs"></div>
 <div class="menu-grid" id="menuGrid"></div>
</div></section>

<section class="dark-section" id="hours"><div class="wrap">
 <div class="section-head"><div class="eyebrow">Come dine with us</div><h2>Opening Hours</h2><p>We look forward to serving you.</p></div>
 <div class="info-grid">
  <div class="info-card"><h3>☀ Afternoon Session</h3><p>12:30 PM – 3:00 PM</p></div>
  <div class="info-card"><h3>☾ Evening Session</h3><p>7:00 PM – 9:00 PM</p></div>
 </div>
</div></section>

<section id="location"><div class="wrap">
 <div class="section-head"><div class="eyebrow">Find us</div><h2>Visit Bismillah Hotel</h2><p>Near Bharat Petroleum Bunk, Cowl Bazar, Ballari, Karnataka, India.</p></div>
 <div style="text-align:center"><a class="btn" target="_blank" rel="noopener" href="https://www.google.com/maps/search/?api=1&query=Near+Bharat+Petroleum+Bunk+Cowl+Bazar+Ballari+Karnataka+India">Get Directions</a></div>
</div></section>

<section class="dark-section" id="contact"><div class="wrap">
 <div class="section-head"><div class="eyebrow">We are happy to help</div><h2>Contact Us</h2><p>Call for enquiries or order through WhatsApp.</p></div>
 <div class="info-grid">
  <div class="info-card"><h3>Phone 1</h3><p><a style="color:#fff" href="tel:+917411171175">7411171175</a></p><a class="btn small" href="tel:+917411171175">Call Now</a></div>
  <div class="info-card"><h3>Phone 2</h3><p><a style="color:#fff" href="tel:+919902028146">9902028146</a></p><a class="btn small" href="tel:+919902028146">Call Now</a></div>
  <div class="info-card"><h3>WhatsApp Orders</h3><p>Send your selected dishes directly to our WhatsApp number.</p><button class="btn small" onclick="sendWhatsApp()">Order on WhatsApp</button></div>
 </div>
</div></section>

<section class="admin" id="admin"><div class="wrap">
 <div class="section-head"><div class="eyebrow">Restaurant management</div><h2>Admin Menu Control</h2><p>Manage dish availability and prices on this device.</p></div>
 <div class="admin-box" id="adminLogin">
  <h3>Admin Login</h3><p class="admin-note">Enter your admin PIN to manage the menu. Change the starter PIN in the project code before publishing.</p>
  <div class="two-col"><input id="adminPin" type="password" inputmode="numeric" placeholder="Enter admin PIN"><button class="btn" onclick="loginAdmin()">Login</button></div>
  <p id="loginError" style="color:#b83232"></p>
 </div>
 <div id="adminPanel" class="hidden">
  <div class="admin-box"><div style="display:flex;justify-content:space-between;align-items:center;gap:10px;flex-wrap:wrap"><h3>Menu Availability & Prices</h3><button class="btn dark small" onclick="logoutAdmin()">Log out</button></div><p class="admin-note">Switch a dish ON to show it to customers, or OFF to hide it. Price changes update this browser's customer menu.</p><div id="adminItems"></div></div>
  <div class="admin-box"><h3>Important setup note</h3><p class="admin-note">This starter version stores menu settings in this browser only. For changes to appear on every customer's phone, connect a shared online database and secure admin authentication before public launch.</p></div>
 </div>
</div></section>
</main>
<footer><div class="footer-brand">BISMILLAH HOTEL</div><p>Good Food, Great Memories!</p><p>Near Bharat Petroleum Bunk, Cowl Bazar, Ballari, Karnataka, India.</p><p>© <span id="year"></span> Bismillah Hotel</p></footer>

<button class="btn float-cart" onclick="openCart()">🛒 Cart (<span id="cartCount">0</span>)</button>
<div class="modal-backdrop" id="cartModal" onclick="if(event.target===this)closeCart()"><div class="modal">
 <div style="display:flex;justify-content:space-between;align-items:center"><h2>Your Order</h2><button class="btn dark small" onclick="closeCart()">Close</button></div>
 <div id="cartItems"></div><h3 id="cartTotal">Total: ₹0</h3>
 <label for="customerName">Your name (optional)</label><input id="customerName" style="width:100%;padding:11px;margin:8px 0 14px;border:1px solid #d4c7af;border-radius:7px" placeholder="Enter your name">
 <button class="btn" style="width:100%" onclick="sendWhatsApp()">Send order on WhatsApp</button>
 <p class="admin-note">Your WhatsApp app will open with the order message. Review it and press Send.</p>
</div></div>
<script>
const ADMIN_PIN = "2468"; // CHANGE THIS PIN before publishing.

const menus = {
 specialBiryani:{title:"Special Biryani · Wed, Fri & Sun",items:[
  ["Mutton Biryani",290],["Mutton Biryani Half",170],["Chicken Biryani",150],["Khushka",80]]},
 weekdayBiryani:{title:"Weekday Biryani Rates",items:[
  ["Mutton Biryani",270],["Mutton Biryani Half",170],["Chicken Biryani",150],["Khushka",80]]},
 mutton:{title:"Mutton Specials · Sun–Fri",items:[
  ["Mutton Dry",270],["Mutton Manchuri",280],["Mutton Chilli",270],["Pepper Mutton",280],["Mutton 65",280],["Mutton Andhra Dry",300],["Mutton Mongolia",300],["Mutton Ghee Roast",320],["Bismillah Special Mutton",320]]},
 chicken:{title:"Chicken Specials · Sun–Fri",items:[
  ["Chicken Dry (Only Bone)",180],["Chicken Manchuri",200],["Pepper Chicken",200],["Chilli Chicken",180],["Chicken 65 (Boneless)",220],["Chicken Andhra Dry",220],["Ginger Chicken",180],["Garlic Chicken",180],["Lemon Chicken",180],["Chicken Majestic",200],["Chicken Ghee Roast (Bone & Boneless)",230],["Chicken 555",220],["Chicken Malaysia",220]]},
 kabab:{title:"Kabab & Leg Pieces",items:[
  ["Kabab Full",150],["Kabab Half",80],["Leg Piece Big",120],["Leg Piece Small",60]]}
};
const STORE_KEY="bismillah_menu_v1";
let settings=loadSettings(), cart={}, activeMenu="specialBiryani", adminLoggedIn=false;
function loadSettings(){try{return JSON.parse(localStorage.getItem(STORE_KEY))||{}}catch(e){return {}}}
function saveSettings(){localStorage.setItem(STORE_KEY,JSON.stringify(settings))}
function keyFor(g,i){return g+"_"+i}
function getDish(g,i){const d=menus[g].items[i],k=keyFor(g,i),s=settings[k]||{};return {name:d[0],price:s.price??d[1],on:s.on!==false}}
function currentDay(){return new Date().getDay()}
function biryaniMenuForToday(){return [0,3,5].includes(currentDay())?"specialBiryani":"weekdayBiryani"}
function tabs(){
 const order=["specialBiryani","weekdayBiryani","mutton","chicken","kabab"];
 document.getElementById("menuTabs").innerHTML=order.map(k=>`<button class="tab ${activeMenu===k?'active':''}" onclick="selectMenu('${k}')">${menus[k].title.split(" · ")[0]}</button>`).join("");
}
function selectMenu(k){activeMenu=k;renderMenu()}
function renderMenu(){
 tabs();const g=activeMenu,arr=menus[g].items;
 const html=arr.map((d,i)=>{const x=getDish(g,i);if((g==="specialBiryani"||g==="weekdayBiryani")&&g!==biryaniMenuForToday())return "";
 return `<article class="dish ${x.on?'':'unavailable'}"><h3>${escapeHtml(x.name)}</h3><div class="desc">${menus[g].title}</div><div class="price">₹${x.price}</div><button class="btn" ${x.on?`onclick="addToCart('${g}',${i})"`:"disabled"}>${x.on?"Add to cart":"Currently unavailable"}</button></article>`}).join("");
 document.getElementById("menuGrid").innerHTML=html||"<p>No dishes available in this category today.</p>";
}
function escapeHtml(s){return String(s).replace(/[&<>"']/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]))}
function addToCart(g,i){const d=getDish(g,i);if(!d.on)return;const k=keyFor(g,i);cart[k]??={...d,qty:0};cart[k].qty++;updateCart()}
function updateCart(){let n=0;Object.values(cart).forEach(x=>n+=x.qty);document.getElementById("cartCount").textContent=n}
function openCart(){renderCart();document.getElementById("cartModal").classList.add("show")}
function closeCart(){document.getElementById("cartModal").classList.remove("show")}
function changeQty(k,delta){if(!cart[k])return;cart[k].qty+=delta;if(cart[k].qty<=0)delete cart[k];renderCart();updateCart()}
function renderCart(){const el=document.getElementById("cartItems"),entries=Object.entries(cart);if(!entries.length){el.innerHTML="<p>Your cart is empty.</p>";document.getElementById("cartTotal").textContent="Total: ₹0";return}
 let total=0;el.innerHTML=entries.map(([k,x])=>{total+=x.price*x.qty;return `<div class="modal-row"><div><strong>${escapeHtml(x.name)}</strong><br>₹${x.price} × ${x.qty}</div><div class="qty"><button onclick="changeQty('${k}',-1)">−</button>${x.qty}<button onclick="changeQty('${k}',1)">+</button></div></div>`}).join("");document.getElementById("cartTotal").textContent="Total: ₹"+total}
function sendWhatsApp(){const entries=Object.values(cart);if(!entries.length){alert("Please add at least one dish to your cart.");return}let total=0;const name=document.getElementById("customerName")?.value?.trim()||"Customer";let msg=`Hello Bismillah Hotel!%0AOrder from: ${name}%0A`;entries.forEach(x=>{total+=x.price*x.qty;msg+=`%0A${x.name} x ${x.qty} = ₹${x.price*x.qty}`});msg+=`%0A%0ATotal: ₹${total}%0AThank you.`;window.open("https://wa.me/917411171175?text="+encodeURIComponent(decodeURIComponent(msg)),"_blank")}
function loginAdmin(){if(document.getElementById("adminPin").value===ADMIN_PIN){adminLoggedIn=true;document.getElementById("adminLogin").classList.add("hidden");document.getElementById("adminPanel").classList.remove("hidden");renderAdminItems()}else document.getElementById("loginError").textContent="Incorrect PIN. Please try again."}
function logoutAdmin(){adminLoggedIn=false;document.getElementById("adminLogin").classList.remove("hidden");document.getElementById("adminPanel").classList.add("hidden");document.getElementById("adminPin").value=""}
function renderAdminItems(){let html="";Object.entries(menus).forEach(([g,group])=>{html+=`<h4>${group.title}</h4>`;group.items.forEach((d,i)=>{const x=getDish(g,i),k=keyFor(g,i);html+=`<div class="admin-row"><div><strong>${escapeHtml(x.name)}</strong></div><div><input aria-label="Price for ${escapeHtml(x.name)}" type="number" min="0" value="${x.price}" onchange="setPrice('${k}',this.value)"></div><button class="switch ${x.on?'on':'off'}" onclick="toggleDish('${k}')">${x.on?'ON':'OFF'}</button></div>`})});document.getElementById("adminItems").innerHTML=html}
function setPrice(k,v){const p=Number(v);if(!Number.isFinite(p)||p<0){alert("Enter a valid price.");renderAdminItems();return}settings[k]??={};settings[k].price=p;saveSettings();renderAdminItems();renderMenu()}
function toggleDish(k){settings[k]??={};settings[k].on=settings[k].on===false?true:false;saveSettings();renderAdminItems();renderMenu()}
document.getElementById("year").textContent=new Date().getFullYear();
renderMenu();updateCart();
if("serviceWorker" in navigator && location.protocol.startsWith("http"))window.addEventListener("load",()=>navigator.serviceWorker.register("./sw.js").catch(()=>{}));
</script>
</body></html>
{
  "name": "Bismillah Hotel",
  "short_name": "Bismillah",
  "start_url": "./index.html",
  "display": "standalone",
  "background_color": "#100d09",
  "theme_color": "#17110b",
  "description": "Bismillah Hotel family restaurant menu and ordering",
  "icons": [
    {
      "src": "icon.svg",
      "sizes": "any",
      "type": "image/svg+xml",
      "purpose": "any maskable"
    }
  ]
}
const CACHE="bismillah-hotel-v1";
const ASSETS=["./","./index.html","./manifest.json","./icon.svg"];
self.addEventListener("install",e=>e.waitUntil(caches.open(CACHE).then(c=>c.addAll(ASSETS))));
self.addEventListener("activate",e=>e.waitUntil(caches.keys().then(keys=>Promise.all(keys.filter(k=>k!==CACHE).map(k=>caches.delete(k))))));
self.addEventListener("fetch",e=>{if(e.request.method!=="GET")return;e.respondWith(caches.match(e.request).then(cached=>cached||fetch(e.request).then(r=>{const copy=r.clone();caches.open(CACHE).then(c=>c.put(e.request,copy));return r}).catch(()=>caches.match("./index.html"))))});
