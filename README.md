      color: var(--text);
      background: radial-gradient(1200px 800px at 80% -10%, #0ea5e91a, transparent 60%), var(--bg);
      -webkit-font-smoothing: antialiased; text-rendering: optimizeLegibility;
    }
    a{color: var(--accent); text-decoration: none}
    a:hover{opacity:.9}
    .container{max-width:var(--maxw); margin-inline:auto; padding: 0 20px}
    header{
      position: sticky; top:0; z-index:50; backdrop-filter: saturate(1.2) blur(8px);
      background: color-mix(in srgb, var(--bg) 70%, transparent);
      border-bottom: 1px solid color-mix(in srgb, var(--muted) 20%, transparent);
    }
    .nav{
      display:flex; align-items:center; justify-content:space-between; gap:16px; height:64px;
    }
    .brand{display:flex; align-items:center; gap:12px; font-weight:700; letter-spacing:.2px}
    .brand-badge{
      width:36px; height:36px; border-radius:10px; background: linear-gradient(135deg,var(--brand),#86efac);
      display:grid; place-items:center; color:#052e16; font-weight:900;
      box-shadow: var(--shadow);
    }
    .navlinks{display:flex; gap:20px; align-items:center}
    .navlinks a{color:var(--text); opacity:.9; padding:8px 10px; border-radius:10px}
    .navlinks a:hover{background: color-mix(in srgb, var(--card) 90%, transparent)}
    .cta{
      background: var(--brand); color:#052e16; font-weight:700; padding:10px 14px; border-radius:12px; box-shadow: var(--shadow);
    }
    .cta:hover{transform: translateY(-1px); transition: .2s ease}
    .menu-btn{display:none; background:transparent; border:1px solid color-mix(in srgb,var(--muted) 30%, transparent); color:var(--text); padding:8px 12px; border-radius:10px}
    @media (max-width:880px){
      .navlinks{display:none}
      .menu-btn{display:inline-flex; align-items:center; gap:8px}
      #mobileMenu{display:none}
      #mobileMenu.open{display:grid}
    }
    /* Hero */
    .hero{padding: 56px 0 24px}
    .hero-grid{
      display:grid; grid-template-columns: 1.2fr .8fr; gap:28px; align-items:center;
    }
    @media (max-width:880px){ .hero-grid{grid-template-columns: 1fr} }
    .pill{
      display:inline-flex; gap:8px; align-items:center; padding:8px 12px; border-radius:999px;
      border:1px solid color-mix(in srgb,var(--muted) 30%, transparent);
      background: color-mix(in srgb, var(--card) 80%, transparent); color: var(--muted); font-weight:600
    }
    h1{font-size: clamp(28px, 4.6vw, 54px); line-height:1.05; margin: 14px 0}
    .lead{color:var(--muted); font-size: clamp(15px, 1.8vw, 18px)}
    .hero-card{
      background: linear-gradient(180deg, color-mix(in srgb, var(--card) 85%, transparent), color-mix(in srgb, var(--card) 98%, transparent));
      border:1px solid color-mix(in srgb,var(--muted) 25%, transparent);
      padding:24px; border-radius: var(--radius); box-shadow: var(--shadow);
    }
    .badges{display:flex; flex-wrap:wrap; gap:10px; margin-top:14px}
    .badge{background:#11182733; border:1px solid #94a3b833; color:var(--text); padding:8px 12px; border-radius:999px; font-weight:600}
    /* Sections */
    section{padding: 36px 0}
    .section-title{font-size: clamp(22px, 3vw, 32px); margin: 0 0 8px}
    .muted{color:var(--muted)}
    .cards{display:grid; grid-template-columns: repeat(3, 1fr); gap:18px}
    @media (max-width:980px){ .cards{grid-template-columns: repeat(2, 1fr)} }
    @media (max-width:640px){ .cards{grid-template-columns: 1fr} }
    .card{
      background: color-mix(in srgb, var(--card) 96%, transparent);
      border:1px solid color-mix(in srgb, var(--muted) 25%, transparent);
      border-radius: var(--radius); padding:20px; box-shadow: var(--shadow);
    }
    .card h3{margin:0 0 6px}
    .list{margin:10px 0 0; padding:0; list-style:none; display:grid; gap:8px}
    .list li{display:flex; align-items:flex-start; gap:10px}
    .dot{width:8px; height:8px; border-radius:999px; background: var(--brand); margin-top:8px}
    /* Contact */
    .contact{
      display:grid; grid-template-columns: 1fr 1fr; gap:20px; align-items:start
    }
    @media (max-width:880px){ .contact{grid-template-columns:1fr} }
    form{
      background: color-mix(in srgb, var(--card) 96%, transparent);
      border:1px solid color-mix(in srgb, var(--muted) 25%, transparent);
      border-radius: var(--radius);
      padding:18px; box-shadow: var(--shadow)
    }
    label{display:block; font-weight:600; margin:12px 0 6px}
    input, textarea{
      width:100%; padding:12px 14px; border-radius:12px; border:1px solid color-mix(in srgb,var(--muted) 30%, transparent);
      background: color-mix(in srgb, var(--card) 92%, transparent); color: var(--text); outline: none;
    }
    input:focus, textarea:focus{box-shadow: 0 0 0 4px var(--ring)}
    textarea{min-height:120px; resize:vertical}
    .btn{display:inline-flex; align-items:center; gap:10px; padding:12px 16px; border-radius:12px; border:none; background: var(--brand); color:#052e16; font-weight:800; cursor:pointer}
    .btn.secondary{background: transparent; color: var(--text); border:1px solid color-mix(in srgb,var(--muted) 30%, transparent)}
    /* Footer */
    footer{
      margin-top: 36px; border-top:1px solid color-mix(in srgb,var(--muted) 20%, transparent);
      background: color-mix(in srgb, var(--card) 95%, transparent);
    }
    .footgrid{display:grid; grid-template-columns: 1.4fr .8fr .8fr; gap:18px; padding: 22px 0}
    @media (max-width:880px){ .footgrid{grid-template-columns:1fr} }
    .copyright{
      padding:12px 0 30px; color: var(--muted); font-size:14px
    }
  </style>
  <script>
    const onReady = (fn)=> document.readyState!=="loading"?fn():document.addEventListener("DOMContentLoaded",fn);
    onReady(()=>{
      const btn = document.getElementById("menuBtn");
      const mob = document.getElementById("mobileMenu");
      if(btn){
        btn.addEventListener("click", ()=> mob.classList.toggle("open"));
      }
      const form = document.querySelector("form#contact");
      if(form){
        form.addEventListener("submit", (e)=>{
          e.preventDefault();
          const data = Object.fromEntries(new FormData(form).entries());
          if(!data.name || !data.email || !data.message){
            alert("Please fill in your name, email, and message.");
            return;
          }
          // TODO: Replace with your backend endpoint or mail provider
          const mailto = `mailto:info@your-domain.com?subject=${encodeURIComponent("Website enquiry")}&body=${encodeURIComponent(
            `Name: ${data.name}\nEmail: ${data.email}\nPhone: ${data.phone || ""}\n\nMessage:\n${data.message}`
          )}`;
          window.location.href = mailto;
        });
      }
    });
  </script>
</head>
<body>
  <header>
    <div class="container nav" role="navigation" aria-label="Main">
      <a class="brand" href="#top" aria-label="WC Industrial home">
        <span class="brand-badge">WC</span>
        <span>WC Industrial</span>
      </a>
      <nav class="navlinks" aria-label="Primary">
        <a href="#services">Services</a>
        <a href="#products">Products</a>
        <a href="#about">About</a>
        <a href="#contact" class="cta">Contact</a>
      </nav>
      <button id="menuBtn" class="menu-btn" aria-expanded="false" aria-controls="mobileMenu">Menu ▾</button>
    </div>
    <div id="mobileMenu" class="container" role="menu" aria-label="Mobile menu">
      <div class="card" style="display:grid; gap:10px; margin:10px 0 14px">
        <a href="#services">Services</a>
        <a href="#products">Products</a>
        <a href="#about">About</a>
        <a href="#contact" class="cta" style="justify-self:start">Contact</a>
      </div>
    </div>
  </header>

  <main id="top">
    <section class="hero">
      <div class="container hero-grid">
        <div>
          <span class="pill">Quick, economical responses</span>
          <h1>Engineering, fabrication, and industrial supplies — done right.</h1>
          <p class="lead">We provide responsive service, reliable support, and quality products across engineering, machining, manufacturing, and rubber moulding.</p>
          <div class="badges" aria-label="Capabilities">
            <span class="badge">Engineering</span>
            <span class="badge">Fabrication</span>
            <span class="badge">Industrial Supplies</span>
            <span class="badge">Machining</span>
            <span class="badge">Manufacturing</span>
            <span class="badge">Rubber Moulding</span>
          </div>
          <div style="display:flex; gap:12px; margin-top:16px">
            <a href="#contact" class="btn" aria-label="Contact us">Get a quote</a>
            <a href="#products" class="btn secondary" aria-label="View products">Browse products</a>
          </div>
          <p class="muted" style="margin-top:12px">We strive for the highest standards in customer service, support, and product quality. — WC Industrial</p>
        </div>
        <div class="hero-card" role="complementary" aria-label="At-a-glance">
          <h3 style="margin:0 0 8px">Why work with us</h3>
          <ul class="list">
            <li><span class="dot"></span><div><strong>Fast turnarounds</strong><br/><span class="muted">Quick responses to urgent industrial needs.</span></div></li>
            <li><span class="dot"></span><div><strong>Broad product access</strong><br/><span class="muted">Sourcing across a diverse industrial catalogue.</span></div></li>
            <li><span class="dot"></span><div><strong>Quality-first</strong><br/><span class="muted">Trusted materials and workmanship you can rely on.</span></div></li>
            <li><span class="dot"></span><div><strong>Local partner</strong><br/><span class="muted">Hands-on support from enquiry to delivery.</span></div></li>
          </ul>
        </div>
      </div>
    </section>

    <div class="container" style="text-align:center; margin-bottom:24px">
    <img src=https://i.imghippo.com/files/Fhm5925GNU.png alt="Industrial workshop with machinery and tools" style="max-width:100%; border-radius:var(--radius); box-shadow:var(--shadow)" />

    <section id="services">
      <div class="container">
        <h2 class="section-title">Core services</h2>
        <p class="muted">From precision machining to on-spec fabrication, our team delivers durable results on time.</p>
        <div class="cards" style="margin-top:12px">
          <article class="card">
            <h3>Engineering & Design</h3>
            <p class="muted">Problem-solving, prototyping, and production-ready drawings.</p>
            <ul class="list">
              <li><span class="dot"></span><div>Design-for-manufacture consulting</div></li>
              <li><span class="dot"></span><div>Reverse engineering</div></li>
              <li><span class="dot"></span><div>Prototyping</div></li>
            </ul>
          </article>
          <article class="card">
            <h3>Fabrication</h3>
            <p class="muted">On-spec metalwork and assemblies.</p>
            <ul class="list">
              <li><span class="dot"></span><div>Cutting, bending, finishing</div></li>
              <li><span class="dot"></span><div>Custom frames and housings</div></li>
            </ul>
          </article>
          <article class="card">
            <h3>Machining</h3>
            <p class="muted">Precision, repeatable parts and repairs.</p>
            <ul class="list">
              <li><span class="dot"></span><div>CNC/Manual turning and milling</div></li>
              <li><span class="dot"></span><div>Tolerances to spec</div></li>
              <li><span class="dot"></span><div>Small to medium runs</div></li>
            </ul>
          </article>
          <article class="card">
            <h3>Manufacturing</h3>
            <p class="muted">Reliable output from prototype to production.</p>
            <ul class="list">
              <li><span class="dot"></span><div>Batch production</div></li>
              <li><span class="dot"></span><div>Assembly and QA</div></li>
              <li><span class="dot"></span><div>Packaging and dispatch</div></li>
            </ul>
          </article>
          <article class="card">
            <h3>Rubber Moulding</h3>
            <p class="muted">Durable elastomer parts for industrial applications.</p>
            <ul class="list">
              <li><span class="dot"></span><div>Custom tooling</div></li>
              <li><span class="dot"></span><div>Material selection guidance</div></li>
              <li><span class="dot"></span><div>Prototyping to production</div></li>
            </ul>
          </article>
          <article class="card">
            <h3>Sourcing & Supplies</h3>
            <p class="muted">Diverse catalogue backed by quick procurement.</p>
            <ul class="list">
              <li><span class="dot"></span><div>Bearings, belts, fasteners</div></li>
              <li><span class="dot"></span><div>Tools, abrasives, PPE</div></li>
              <li><span class="dot"></span><div>Hydraulics and pneumatics</div></li>
            </ul>
          </article>
        </div>
      </div>
    </section>

    <section id="products">
      <div class="container">
        <h2 class="section-title">Products</h2>
        <p class="muted">We can provide any industrial product you need. If it’s not listed, ask and we’ll source it.</p>
        <div class="cards" style="margin-top:12px">
          <article class="card">
            <h3>PPE & Safety</h3>
            <p class="muted">Gloves, eyewear, respirators, hearing protection.</p>
            <a class="cta" href="#contact" aria-label="Enquire about PPE">Enquire</a>
          </article>
          <article class="card">
            <h3>Mechanical</h3>
            <p class="muted">Bearings, chains, belts, seals, couplings.</p>
            <a class="cta" href="#contact" aria-label="Enquire about mechanical products">Enquire</a>
          </article>
          <article class="card">
            <h3>Tools & Consumables</h3>
            <p class="muted">Cutting tools, abrasives, adhesives, lubricants.</p>
            <a class="cta" href="#contact" aria-label="Enquire about tools and consumables">Enquire</a>
          </article>
        </div>
      </div>
    </section>

    <section id="about">
      <div class="container">
        <h2 class="section-title">About</h2>
        <p class="muted">We’re proud of the work we do for our clients and aim to give you the information you need to decide whether to work with us.</p>
        <div class="cards" style="margin-top:12px">
          <article class="card">
            <h3>Our promise</h3>
            <p class="muted">Highest standards in customer service, support, and product quality.</p>
          </article>
          <article class="card">
            <h3>Where we help</h3>
            <p class="muted">From urgent repairs to planned projects across sectors.</p>
          </article>
          <article class="card">
            <h3>Let’s talk</h3>
            <p class="muted">If there’s an industrial or safety item not listed, get in touch and we’ll source it.</p>
          </article>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <h2 class="section-title">Contact</h2>
        <p class="muted">Tell us what you need and we’ll respond quickly with timing and options.</p>
        <div class="contact">
          <form id="contact" aria-label="Contact form">
            <label for="name">Name</label>
            <input id="name" name="name" placeholder="Your name" autocomplete="name" required />
            <label for="email">Email</label>
            <input id="email" name="email" type="email" placeholder="you@example.com" autocomplete="email" required />
            <label for="phone">Phone</label>
            <input id="phone" name="phone" type="tel" placeholder="0832265765" autocomplete="tel" />
            <label for="message">How can we help?</label>
            <textarea id="message" name="message" placeholder="Briefly describe your request..." required></textarea>
            <div style="display:flex; gap:10px; margin-top:12px">
              <button type="submit" class="btn">Send enquiry</button>
              <a class="btn secondary" href="tel:0832265765" aria-label="Call us">Call us</a>
            </div>
            <p class="muted" style="font-size:13px; margin-top:8px">By contacting us, you agree to be reached about your enquiry.</p>
          </form>
          <div class="card" role="complementary">
            <h3>Details</h3>
            <ul class="list" style="margin-top:8px">
              <li><span class="dot"></span><div><strong>Phone</strong><br/>0832265765<!-- TODO: Replace --></div></li>
              <li><span class="dot"></span><div><strong>Email</strong><br/>sales@wcindustrial.co za <!-- TODO: Replace --></div></li>
              <li><span class="dot"></span><div><strong>Address</strong><br/>2 Waterson Street Rynfield Benoni  <!-- TODO: Replace --></div></li>
              <li><span class="dot"></span><div><strong>Hours</strong><br/>Mon–Fri 08:00–17:00 <!-- TODO: Replace --></div></li>
            </ul>
            <div style="margin-top:12px">
              <a class="cta" href="mailto:info@sales@wcindustrial.co.za">Email us</a>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer role="contentinfo">
    <div class="container footgrid">
      <div>
        <div class="brand">
          <span class="brand-badge">WC</span>
          <span>WC Industrial</span>
        </div>
        <p class="muted" style="margin-top:8px">Quick and economical responses to your industrial needs.</p>
      </div>
      <div>
        <h4 style="margin:0 0 6px">Explore</h4>
        <div style="display:grid; gap:8px">
          <a href="#services">Services</a>
          <a href="#products">Products</a>
          <a href="#about">About</a>
          <a href="#contact">Contact</a>
        </div>
      </div>
      <div>
        <h4 style="margin:0 0 6px">Get in touch</h4>
        <div style="display:grid; gap:8px">
          <a href="mailto:sales@wcindustrial.co.za">sales@wcindustrial.co za</a>
          <a href="tel:011 915 5282">011 915 5282</a>
          <a href="#">Google Maps</a>
        </div>
      </div>
    </div>
    <div class="container" style="border-top:1px dashed color-mix(in srgb,var(--muted) 30%, transparent)"></div>
    <div class="container copyright" style="padding:18px 0; text-align:center; font-size:14px">
      <p style="margin:0">&copy; 2023 WC Industrial. All rights reserved.</p>
    </div>
  </footer>
</body>
</html>
