<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <meta name="description" content="Noorain Skincare & Cosmetics - Natural, handmade skincare crafted for men and women." />
  <meta name="keywords" content="Noorain, skincare, cosmetics, handmade, natural, lip balm, night cream, SPF, face wash" />
  <meta name="author" content="Noorain Skincare & Cosmetics" />
  <meta property="og:title" content="Noorain Skincare & Cosmetics" />
  <meta property="og:description" content="Glow Naturally – Skincare Crafted for Confidence." />
  <meta property="og:image" content="https://i.postimg.cc/KYBZbktv/Noorain-Logo-Rosegold.png" />
  <meta property="og:url" content="https://noorainskincare.vercel.app" />
  <title>Noorain Skincare & Cosmetics</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom, #fff6f7, #ffe6eb);
      overflow-x: hidden;
      color: #4b2c2c;
    }
    header { background: #f9e6e8; text-align: center; padding: 1rem; }
    header img { max-width: 160px; }
    nav { background: #ffe3e3; display: flex; justify-content: center; gap: 1.5rem; padding: 1rem; font-weight: bold; }
    nav a { text-decoration: none; color: #a33658; }
    .carousel { display: flex; overflow: hidden; width: 100%; max-height: 350px; margin: 0 auto; position: relative; }
    .carousel img { width: 100%; height: auto; object-fit: cover; flex-shrink: 0; animation: slide 12s infinite; }
    @keyframes slide {
      0% { transform: translateX(0%); }
      33% { transform: translateX(-100%); }
      66% { transform: translateX(-200%); }
      100% { transform: translateX(0%); }
    }
    .flower { position: fixed; top: -50px; font-size: 20px; animation: fall 10s linear infinite; }
    @keyframes fall {
      0% { transform: translateY(-50px); opacity: 1; }
      100% { transform: translateY(100vh); opacity: 0; }
    }
    .product, .testimonial-card {
      background: white;
      padding: 1rem;
      border-radius: 12px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      text-align: center;
    }
    .product img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      border-radius: 8px;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 1.5rem;
      padding: 2rem;
    }
    .testimonial-section {
      display: flex;
      gap: 1.5rem;
      overflow-x: auto;
      padding: 2rem;
      scroll-snap-type: x mandatory;
    }
    .testimonial-card {
      min-width: 250px;
      flex: 0 0 auto;
      scroll-snap-align: start;
    }
    form input, form textarea, form button {
      width: 100%;
      padding: 0.8rem;
      margin: 0.5rem 0;
      border-radius: 8px;
    }
    form button {
      background: #c83b6f;
      color: white;
      border: none;
    }
    .whatsapp-btn {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #25D366;
      color: white;
      padding: 0.75rem 1rem;
      border-radius: 50%;
      font-size: 24px;
      text-decoration: none;
      z-index: 1000;
    }
    footer {
      background: #ffe6eb;
      text-align: center;
      padding: 3rem 1rem;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>
<header>
  <img src="https://i.postimg.cc/KYBZbktv/Noorain-Logo-Rosegold.png" alt="Noorain Logo"/>
</header>

<div class="carousel">
  <img src="https://i.postimg.cc/3RFLXjQK/model1.jpg" alt="Model 1">
  <img src="https://i.postimg.cc/nLZynsn6/model2.jpg" alt="Model 2">
  <img src="https://i.postimg.cc/VLf3kQFH/model3.jpg" alt="Model 3">
</div>

<nav>
  <a href="#home">Home</a>
  <a href="#shop">Shop</a>
  <a href="#about">About</a>
  <a href="#checkout">Checkout</a>
</nav>

<section class="hero" id="home" style="text-align:center;padding:3rem 1rem;">
  <h1>Skincare Crafted For Confidence for Men and Women</h1>
  <p>Handcrafted skincare powered by nature, designed for confidence and love.</p>
</section>

<h2 style="text-align:center;" id="about">Founder Story & Vision</h2>
<section style="padding: 1rem 2rem; max-width: 800px; margin: auto;">
  <p>I created Noorain Skincare & Cosmetics to offer safe, effective, natural skincare that promotes confidence, peace, and self-love. Handcrafted in small batches, our products serve both men and women with love and care.</p>
</section>

<h2 style="text-align:center;" id="shop">Shop All Products</h2>
<section class="products">
  <div class="product"><img src="https://i.postimg.cc/43ZKvvFq/night-cream.jpg"><h3>Brightening Night Cream</h3><p>₹750</p><button onclick="addToCart('Brightening Night Cream',750)">Add to Cart</button></div>
  <div class="product"><img src="https://i.postimg.cc/MpZfVw6x/glow & grain-facewash.jpg"><h3>Glow & Grain Facewash </h3><p>₹199</p><button onclick="addToCart('Glow & Grain-Facewash',199)">Add to Cart</button></div>
  <div class="product"><img src="https://i.postimg.cc/zX4YgG31/rose-facewash.jpg"><h3>Rose Face Wash</h3><p>₹199</p><button onclick="addToCart('Rose Face Wash',199)">Add to Cart</button></div>
  <div class="product"><img src="https://i.postimg.cc/qMCmN7nK/ginseng-facewash.jpg"><h3>Ginseng Energize Glow Face Wash</h3><p>₹199</p><button onclick="addToCart('Ginseng Energize Glow Face Wash',199)">Add to Cart</button></div>
  <div class="product"><img src="https://i.postimg.cc/tJC44TRr/irish-soap.jpg"><h3>Irish Illumination Soap</h3><p>₹129</p><button onclick="addToCart('Irish Illumination Soap',129)">Add to Cart</button></div>
  <div class="product"><img src="https://i.postimg.cc/yY0kY5Kz/beetroot-lip.jpg"><h3>Beetroot-Rose Lip Butter</h3><p>₹149</p><button onclick="addToCart('Beetroot-Rose Lip Butter',149)">Add to Cart</button></div>
  <div class="product"><img src="https://i.postimg.cc/SRKG1F3g/strawberry-lip.jpg"><h3>Strawberry Lip Butter</h3><p>₹149</p><button onclick="addToCart('Strawberry Lip Butter',149)">Add to Cart</button></div>
  <div class="product"><img src="https://i.postimg.cc/Zq2zFDPK/chocolate-lip.jpg"><h3>Chocolate Lip Butter</h3><p>₹149</p><button onclick="addToCart('Chocolate Lip Butter',149)">Add to Cart</button></div>
  <div class="product"><img src="https://i.postimg.cc/j5xNQLZT/sunscreen.jpg"><h3>Lumi_Glow SPF 50 Tinted Sunscreen</h3><p>₹399</p><button onclick="addToCart('Lumi_Glow SPF 50 Tinted Sunscreen',399)">Add to Cart</button></div>
  <div class="product"><img src="https://i.postimg.cc/6qFWXCG7/hydra-rose-mist.jpg"><h3>Hydra-Rose Mist</h3><p>₹199</p><button onclick="addToCart('Hydra-Rose Mist',199)">Add to Cart</button></div>
</section>

<h2 style="text-align:center;">Customer Testimonials 💖</h2>
<section class="testimonial-section">
  <div class="testimonial-card"><blockquote>“Glowing skin in a week – magic in a jar!” – Ayesha</blockquote></div>
  <div class="testimonial-card"><blockquote>“That lip balm? OBSESSED.” – Zara</blockquote></div>
  <div class="testimonial-card"><blockquote>“Night cream + sunscreen = my new ritual.” – Arman</blockquote></div>
</section>

<h2 style="text-align:center;" id="checkout">Checkout</h2>
<section style="max-width: 600px; margin: auto; padding: 2rem;">
  <div id="cart-summary"></div>
  <button id="rzp-button1" style="padding: 0.8rem 1.5rem; background: #000; color: white; border: none; border-radius: 8px; margin-top: 1rem;">Pay with Razorpay</button>
</section>

<a href="https://wa.me/message/FCDYEGMJYSJ6O1" class="whatsapp-btn" target="_blank">💬</a>

<footer>
  <p>
    <a href="https://www.instagram.com/noorain_skincare_cosmetics">Instagram</a> |
    <a href="https://wa.me/message/FCDYEGMJYSJ6O1">WhatsApp</a> |
    <a href="https://www.facebook.com/share/1586dWhFzkk/">Facebook</a>
  </p>
  <p>&copy; 2024 Noorain Skincare & Cosmetics. All rights reserved.</p>
</footer>

<script src="https://checkout.razorpay.com/v1/checkout.js"></script>
<script>
  const cart = [];
  function addToCart(name, price) {
    cart.push({ name, price });
    let summary = '<h3>Your Cart:</h3><ul>';
    cart.forEach(item => summary += `<li>${item.name} – ₹${item.price}</li>`);
    summary += '</ul>';
    summary += `<p><strong>Total: ₹${cart.reduce((s, i) => s + i.price, 0)}</strong></p>`;
    document.getElementById('cart-summary').innerHTML = summary;
  }

  document.getElementById('rzp-button1').onclick = async function () {
    const amount = cart.reduce((sum, item) => sum + item.price, 0);
    const res = await fetch("/api/create-order", {
      method: "POST",
      headers: { "Content-Type": "application/json" },
      body: JSON.stringify({ amount }),
    });
    const data = await res.json();
    const options = {
      key: "rzp_live_Db1Y0UmrcNXmlw",
      amount: data.amount,
      currency: "INR",
      name: "Noorain Skincare & Cosmetics",
      description: "Product Purchase",
      order_id: data.id,
      handler: async function (response) {
        const verify = await fetch("/api/verify-payment", {
          method: "POST",
          headers: { "Content-Type": "application/json" },
          body: JSON.stringify(response),
        });
        const resData = await verify.json();
        if (resData.success) {
          window.location.href = "/thank-you.html";
        } else {
          alert("Payment verification failed.");
        }
      },
      theme: { color: "#c83b6f" }
    };
    const rzp1 = new Razorpay(options);
    rzp1.open();
  };

  // Falling flowers animation
  setInterval(() => {
    const flower = document.createElement("div");
    flower.className = "flower";
    flower.style.left = Math.random() * window.innerWidth + "px";
    flower.style.animationDuration = (5 + Math.random() * 5) + "s";
    flower.innerHTML = "🌸";
    document.body.appendChild(flower);
    setTimeout(() => flower.remove(), 10000);
  }, 500);
</script>
</body>
</html>
