customer reviews   




<meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Customer Reviews - Elite Home Services | London, ON</title>

  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&amp;family=Inter:wght@300;400;500;600;700&amp;display=swap" rel="stylesheet">

  <style>
    *{margin:0;padding:0;box-sizing:border-box}
    :root{
      --background:#faf8f6;
      --foreground:#2d2520;
      --primary:#5D4037;
      --primary-foreground:#faf8f6;
      --accent:#c4784a;
      --muted:#6b5c52;
      --card:#f5f2ef;
      --border:#e8e2dc;
      --radius:16px;
      --shadow:0 14px 40px -14px rgba(45,37,32,0.18);
    }

    body{
      font-family:'Inter',sans-serif;
      background:var(--background);
      color:var(--foreground);
      line-height:1.6;
    }
    h1,h2,h3,h4{font-family:'Playfair Display',serif}
    a{color:inherit}
    .container{max-width:1100px;margin:0 auto;padding:0 16px}

    /* HEADER */
    .header{
      background:var(--primary);
      color:var(--primary-foreground);
      border-bottom:1px solid rgba(255,255,255,0.12);
    }
    .header-wrap{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
      padding:14px 0;
      flex-wrap:wrap;
    }
    .brand{display:flex;flex-direction:column;gap:2px;min-width:220px}
    .brand h1{font-size:18px;font-weight:700;letter-spacing:.2px;line-height:1.15}
    .brand p{font-size:12.5px;opacity:.85}

    .header-actions{
      display:flex;
      gap:10px;
      flex-wrap:wrap;
      justify-content:flex-end;
    }
    .pill{
      display:inline-flex;
      align-items:center;
      gap:8px;
      text-decoration:none;
      padding:10px 12px;
      border-radius:999px;
      border:1px solid rgba(255,255,255,0.18);
      background:rgba(255,255,255,0.08);
      font-size:13px;
      font-weight:600;
      transition:transform .15s ease, opacity .15s ease;
      white-space:nowrap;
    }
    .pill:hover{opacity:0.9;transform:translateY(-1px)}
    .pill strong{font-weight:700}

    /* HERO */
    .hero{
      position:relative;
      background:
        linear-gradient(to bottom, rgba(45,37,32,0.78), rgba(45,37,32,0.35)),
        url("https://i.pinimg.com/736x/1a/29/68/1a296886149f29bdf2296c27ba723aba.jpg") center/cover no-repeat;
      color:var(--primary-foreground);
    }
    .hero .container{padding:34px 16px 28px}
    .hero-card{
      max-width:720px;
      background:rgba(0,0,0,0.15);
      border:1px solid rgba(255,255,255,0.14);
      border-radius:var(--radius);
      padding:18px;
      box-shadow:0 18px 50px -26px rgba(0,0,0,0.55);
      backdrop-filter: blur(8px);
    }
    .hero h2{font-size:28px;line-height:1.15;margin-bottom:10px;color:#fff}
    .hero p{font-size:15.5px;opacity:.92;margin-bottom:14px;max-width:60ch}
    .hero-cta{display:flex;gap:10px;flex-wrap:wrap;margin-bottom:14px}
    .btn{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      gap:10px;
      padding:12px 16px;
      border-radius:999px;
      text-decoration:none;
      font-weight:700;
      font-size:14px;
      border:1px solid rgba(255,255,255,0.0);
      transition:transform .15s ease, opacity .15s ease;
      white-space:nowrap;
    }
    .btn:hover{transform:translateY(-1px);opacity:0.95}
    .btn-primary{
      background:var(--accent);
      color:#1f140f;
      border:1px solid rgba(255,255,255,0.12);
    }
    .btn-outline{
      background:rgba(255,255,255,0.10);
      color:var(--primary-foreground);
      border:1px solid rgba(255,255,255,0.18);
    }
    .badges{display:flex;flex-wrap:wrap;gap:8px}
    .badge{
      display:inline-flex;
      align-items:center;
      gap:8px;
      padding:8px 12px;
      border-radius:999px;
      background:rgba(255,255,255,0.10);
      border:1px solid rgba(255,255,255,0.16);
      font-size:12.5px;
      font-weight:600;
    }
    .dot{width:8px;height:8px;border-radius:50%;background:var(--accent)}

    /* REVIEWS SECTION */
    .reviews-section{
      padding:48px 16px;
      background:var(--card);
    }
    .reviews-intro{
      text-align:center;
      max-width:800px;
      margin:0 auto 32px;
      color:var(--muted);
      font-size:15px;
      line-height:1.8;
    }
    .reviews-grid{
      display:grid;
      grid-template-columns:1fr;
      gap:14px;
      max-width:1100px;
      margin:0 auto;
    }
    .review-card{
      background:#fff;
      border:1px solid var(--border);
      border-radius:var(--radius);
      padding:18px;
      box-shadow:var(--shadow);
      transition:transform 0.2s ease, box-shadow 0.2s ease;
    }
    .review-card:hover{
      transform:translateY(-2px);
      box-shadow:0 18px 48px -18px rgba(45,37,32,0.24);
    }
    .review-header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      margin-bottom:10px;
      gap:12px;
      flex-wrap:wrap;
    }
    .review-name{
      font-weight:700;
      font-size:15px;
      color:var(--foreground);
    }
    .review-stars{
      color:#f4b400;
      font-size:16px;
      letter-spacing:2px;
    }
    .review-text{
      font-size:14px;
      color:var(--muted);
      line-height:1.7;
    }
    .review-card.hidden{
      display:none;
    }

    /* REVIEWS ACTIONS */
    .reviews-actions{
      margin-top:24px;
      display:flex;
      justify-content:center;
    }
    .more-btn{
      padding:12px 24px;
      border-radius:999px;
      border:none;
      background:var(--primary);
      color:var(--primary-foreground);
      font-weight:700;
      font-size:14px;
      cursor:pointer;
      transition:transform 0.15s ease, opacity 0.15s ease;
    }
    .more-btn:hover{
      transform:translateY(-1px);
      opacity:0.95;
    }

    /* CTA SECTION */
    .cta-section{
      padding:48px 16px;
      background:var(--primary);
      color:var(--primary-foreground);
      text-align:center;
    }
    .cta-section h2{
      font-size:28px;
      margin-bottom:12px;
      color:#fff;
    }
    .cta-section p{
      font-size:15px;
      margin-bottom:20px;
      opacity:0.92;
    }

    @media (min-width: 640px){
      .container{padding:0 20px}
      .hero .container{padding:44px 20px 34px}
      .hero h2{font-size:34px}
      .reviews-grid{grid-template-columns:repeat(2, minmax(0,1fr))}
      .review-card{padding:20px}
    }
    @media (min-width: 980px){
      .hero .container{padding:68px 24px 48px}
      .hero-card{padding:22px}
      .hero h2{font-size:44px}
      .hero p{font-size:16.5px}
      .reviews-grid{grid-template-columns:repeat(2, minmax(0,1fr))}
    }
    html{scroll-behavior:smooth}
  </style>



  <!-- HEADER -->
  <header class="header">
    <div class="container">
      <div class="header-wrap">
        <div class="brand">
          <h1>Elite Home Services</h1>
          <p>Professional Home Improvement • London, ON</p>
        </div>

        <div class="header-actions">
          <a class="pill" href="tel:+15198518887">📞 <strong>+1 (519) 851-8887</strong></a>
          <a class="pill" href="mailto:contact@elitehomeservices.ca">✉️ <strong>contact@elitehomeservices.ca</strong></a>
        </div>
      </div>
    </div>
  </header>

  <!-- HERO -->
  <section class="hero">
    <div class="container">
      <div class="hero-card">
        <h2>Customer Reviews</h2>
        <p>
          See what our customers have to say about our work. Real feedback from real homeowners who trust Elite Home Services for their home improvement needs.
        </p>

        <div class="hero-cta">
          <a class="btn btn-primary" href="/contact/">Get Your Free Quote</a>
          <a class="btn btn-outline" href="/services/">View Our Services</a>
        </div>

        <div class="badges">
          <span class="badge"><span class="dot"></span> 100% Customer Satisfaction</span>
          <span class="badge"><span class="dot"></span> Clean Professional Work</span>
          <span class="badge"><span class="dot"></span> Trusted in London, ON</span>
        </div>
      </div>
    </div>
  </section>

  <!-- REVIEWS SECTION -->
  <section class="reviews-section">
    <div class="container">
      <p class="reviews-intro">
        Our customers appreciate the quality of our work, our attention to detail, and our commitment to clean, professional finishing. From the first consultation to the final result, we focus on delivering reliable service, clear communication, and results that homeowners can feel confident about. Their feedback reflects the care we put into every project, no matter the size.
      </p>

      <div class="reviews-grid" id="reviewsGrid">
        
        <div class="review-card">
          <div class="review-header">
            <span class="review-name">Michael Carter</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Great work on our laminate flooring. Clean cuts and finished on time.</p>
        </div>

        <div class="review-card">
          <div class="review-header">
            <span class="review-name">Sarah Mitchell</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">They repaired our walls and repainted the living room. Perfect finish.</p>
        </div>

        <div class="review-card">
          <div class="review-header">
            <span class="review-name">Daniel Thompson</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Hired for a backyard wooden fence. Solid build, straight lines.</p>
        </div>

        <div class="review-card">
          <div class="review-header">
            <span class="review-name">Emily Johnson</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Professional and honest. Clean edges and no mess left behind.</p>
        </div>

        <div class="review-card">
          <div class="review-header">
            <span class="review-name">Jason Walker</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Door installation was done perfectly. Attention to detail is great.</p>
        </div>

        <div class="review-card">
          <div class="review-header">
            <span class="review-name">Olivia Parker</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Removed old flooring and installed vinyl. Fast and clean.</p>
        </div>

        <div class="review-card">
          <div class="review-header">
            <span class="review-name">Andrew Lewis</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">TV wall décor came out amazing with clean finishing.</p>
        </div>

        <div class="review-card">
          <div class="review-header">
            <span class="review-name">Hannah Reed</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Interior painting and wall repairs. Very respectful team.</p>
        </div>

        <div class="review-card">
          <div class="review-header">
            <span class="review-name">David Brooks</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Wood staining on our stairs looks beautiful. No streaks.</p>
        </div>

        <div class="review-card">
          <div class="review-header">
            <span class="review-name">Sophia Adams</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Upgraded our laundry room with better storage. Great ideas.</p>
        </div>

        <div class="review-card">
          <div class="review-header">
            <span class="review-name">Mohammed Alhassan</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Door installation was done perfectly. Attention to detail is great.</p>
        </div>

        <!-- HIDDEN REVIEWS -->
        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Ryan Collins</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Exterior paint looks durable and even. Sharp results.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Natalie Bennett</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Very reliable service. Finished the job as promised.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Kevin Rogers</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Installed new baseboards. Everything looks clean.</p>
        </div>
<div class="review-card">
  <div class="review-header">
    <span class="review-name">Jason Walker</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Door installation was done perfectly. Attention to detail is great.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Michael Brown</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Very professional service and clean finishing. Highly recommended.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Daniel Thompson</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Painting job was excellent and completed on time.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Chris Anderson</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Fence installation looks solid and very well done.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Ryan Mitchell</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Great communication and professional work from start to finish.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Andrew Wilson</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Clean work and very respectful of my home.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Kevin Harris</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Flooring installation was smooth and looks amazing.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Brian Lewis</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Reliable service and fair pricing. Very happy with the result.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Steven Clark</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Professional team and excellent finishing quality.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Matthew Rodriguez</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">They completed the job faster than expected with great quality.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Joshua Martinez</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Very organized and professional from the first call.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Anthony Moore</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Outstanding workmanship and attention to details.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Justin Taylor</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Great experience overall. Will definitely hire again.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Mark Johnson</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">High quality work and very professional attitude.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Adam White</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">The final result exceeded my expectations.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Eric Young</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">On-time service and very clean finishing.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Patrick King</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">They were honest, reliable, and professional.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Nathan Scott</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Excellent service and very friendly team.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Jonathan Green</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">The work was done perfectly and on schedule.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Kyle Adams</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Very professional and detail-oriented work.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Brandon Nelson</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Great craftsmanship and excellent communication.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Dylan Carter</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Smooth process and high-quality results.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Sean Phillips</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Reliable service with clean and professional finishing.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Tyler Evans</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Very satisfied with the work and the professionalism.</p>
</div>

<div class="review-card">
  <div class="review-header">
    <span class="review-name">Alex Parker</span>
    <div class="review-stars">★★★★★</div>
  </div>
  <p class="review-text">Top-quality service with great attention to detail.</p>
</div>

    <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Grace Phillips</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Corrected uneven wall areas and repainted perfectly.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Justin Evans</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Fence repair and gate adjustment done properly.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Chloe Murphy</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Helped mount our TV and install shelves. Secure work.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Brandon Scott</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Vinyl flooring installation was excellent. No gaps.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Megan Turner</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Painted our hallway and fixed cracks. Perfect results.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Ethan Howard</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Custom bedroom décor turned out beautiful.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Lily Cooper</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">On-time work and exceeded our expectations.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Noah Bailey</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Installed a new door and did finishing. Aligned perfectly.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Ava Richardson</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Smooth walls, clean corners, and no paint splatter.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Logan Price</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Backyard fence installation was strong and looks fantastic.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Zoe Watson</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Updated laundry room. Great workmanship.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Tyler King</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Small home improvements done right. Respectful team.</p>
        </div>

        <div class="review-card hidden">
          <div class="review-header">
            <span class="review-name">Nabush Alwadi</span>
            <div class="review-stars">★★★★★</div>
          </div>
          <p class="review-text">Exterior paint looks durable and even. Sharp results.</p>
        </div>

      </div>

      <div class="reviews-actions">
        <button class="more-btn" id="toggleReviews">See More Reviews</button>
      </div>
    </div>
  </section>

  <!-- CTA SECTION -->
  <section class="cta-section">
    <div class="container">
      <h2>Ready to Start Your Project?</h2>
      <p>Join our satisfied customers. Contact us today for a free estimate.</p>
      <a class="btn btn-primary" href="/contact/">Get Your Free Quote</a>
    </div>
  </section>

  <script>
    (function() {
      const btn = document.getElementById('toggleReviews');
      const hiddenReviews = document.querySelectorAll('.review-card.hidden');
      let expanded = false;

      btn.onclick = () => {
        expanded = !expanded;
        hiddenReviews.forEach(card => {
          card.style.display = expanded ? 'block' : 'none';
        });
        btn.textContent = expanded ? 'See Less Reviews' : 'See More Reviews';
      };
    })();
  </script>















# FAQs 





<meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>FAQs - Elite Home Services | London, ON</title>

  <link href="https://i.pinimg.com/736x/fb/19/04/fb1904497db64d0689e360c560623815.jpg" rel="stylesheet">

  <style>
    *{margin:0;padding:0;box-sizing:border-box}
    :root{
      --background:#faf8f6;
      --foreground:#2d2520;
      --primary:#5D4037;
      --primary-foreground:#faf8f6;
      --accent:#c4784a;
      --muted:#6b5c52;
      --card:#f5f2ef;
      --border:#e8e2dc;
      --radius:16px;
      --shadow:0 14px 40px -14px rgba(45,37,32,0.18);
    }

    body{
      font-family:'Inter',sans-serif;
      background:var(--background);
      color:var(--foreground);
      line-height:1.6;
    }
    h1,h2,h3,h4{font-family:'Playfair Display',serif}
    a{color:inherit}
    .container{max-width:1100px;margin:0 auto;padding:0 16px}

    /* HEADER */
    .header{
      background:var(--primary);
      color:var(--primary-foreground);
      border-bottom:1px solid rgba(255,255,255,0.12);
    }
    .header-wrap{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
      padding:14px 0;
      flex-wrap:wrap;
    }
    .brand{display:flex;flex-direction:column;gap:2px;min-width:220px}
    .brand h1{font-size:18px;font-weight:700;letter-spacing:.2px;line-height:1.15}
    .brand p{font-size:12.5px;opacity:.85}

    .header-actions{
      display:flex;
      gap:10px;
      flex-wrap:wrap;
      justify-content:flex-end;
    }
    .pill{
      display:inline-flex;
      align-items:center;
      gap:8px;
      text-decoration:none;
      padding:10px 12px;
      border-radius:999px;
      border:1px solid rgba(255,255,255,0.18);
      background:rgba(255,255,255,0.08);
      font-size:13px;
      font-weight:600;
      transition:transform .15s ease, opacity .15s ease;
      white-space:nowrap;
    }
    .pill:hover{opacity:0.9;transform:translateY(-1px)}
    .pill strong{font-weight:700}

    /* HERO */
    .hero{
      position:relative;
      background:
        linear-gradient(to bottom, rgba(45,37,32,0.78), rgba(45,37,32,0.35)),
        url("https://i.pinimg.com/736x/fb/19/04/fb1904497db64d0689e360c560623815.jpg") center/cover no-repeat;
      color:var(--primary-foreground);
    }
    .hero .container{padding:34px 16px 28px}
    .hero-card{
      max-width:720px;
      background:rgba(0,0,0,0.15);
      border:1px solid rgba(255,255,255,0.14);
      border-radius:var(--radius);
      padding:18px;
      box-shadow:0 18px 50px -26px rgba(0,0,0,0.55);
      backdrop-filter: blur(8px);
    }
    .hero h2{font-size:28px;line-height:1.15;margin-bottom:10px;color:#fff}
    .hero p{font-size:15.5px;opacity:.92;margin-bottom:14px;max-width:60ch}
    .hero-cta{display:flex;gap:10px;flex-wrap:wrap;margin-bottom:14px}
    .btn{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      gap:10px;
      padding:12px 16px;
      border-radius:999px;
      text-decoration:none;
      font-weight:700;
      font-size:14px;
      border:1px solid rgba(255,255,255,0.0);
      transition:transform .15s ease, opacity .15s ease;
      white-space:nowrap;
    }
    .btn:hover{transform:translateY(-1px);opacity:0.95}
    .btn-primary{
      background:var(--accent);
      color:#1f140f;
      border:1px solid rgba(255,255,255,0.12);
    }
    .btn-outline{
      background:rgba(255,255,255,0.10);
      color:var(--primary-foreground);
      border:1px solid rgba(255,255,255,0.18);
    }
    .badges{display:flex;flex-wrap:wrap;gap:8px}
    .badge{
      display:inline-flex;
      align-items:center;
      gap:8px;
      padding:8px 12px;
      border-radius:999px;
      background:rgba(255,255,255,0.10);
      border:1px solid rgba(255,255,255,0.16);
      font-size:12.5px;
      font-weight:600;
    }
    .dot{width:8px;height:8px;border-radius:50%;background:var(--accent)}

    /* FAQ SECTION */
    .faq-section{
      padding:48px 16px;
      background:var(--card);
    }
    .faq-container{
      max-width:800px;
      margin:0 auto;
    }
    .faq-item{
      background:#fff;
      border:1px solid var(--border);
      border-radius:var(--radius);
      margin-bottom:12px;
      box-shadow:var(--shadow);
      overflow:hidden;
    }
    .faq-question{
      width:100%;
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:16px;
      padding:18px 20px;
      background:#fff;
      border:none;
      cursor:pointer;
      text-align:left;
      font-family:'Inter',sans-serif;
      font-size:15px;
      font-weight:600;
      color:var(--foreground);
      transition:background 0.2s ease;
    }
    .faq-question:hover{
      background:var(--card);
    }
    .faq-question.active{
      background:var(--card);
    }
    .faq-icon{
      width:28px;
      height:28px;
      border-radius:50%;
      background:linear-gradient(135deg, var(--accent), #d89364);
      display:flex;
      align-items:center;
      justify-content:center;
      flex-shrink:0;
      color:#fff;
      font-size:18px;
      font-weight:400;
      transition:transform 0.3s ease;
    }
    .faq-question.active .faq-icon{
      transform:rotate(45deg);
    }
    .faq-answer{
      max-height:0;
      overflow:hidden;
      transition:max-height 0.3s ease, padding 0.3s ease;
    }
    .faq-answer.open{
      max-height:500px;
    }
    .faq-answer-content{
      padding:0 20px 20px 20px;
      font-size:14px;
      color:var(--muted);
      line-height:1.8;
    }

    /* CTA SECTION */
    .cta-section{
      padding:48px 16px;
      background:var(--primary);
      color:var(--primary-foreground);
      text-align:center;
    }
    .cta-section h2{
      font-size:28px;
      margin-bottom:12px;
      color:#fff;
    }
    .cta-section p{
      font-size:15px;
      margin-bottom:20px;
      opacity:0.92;
    }

    @media (min-width: 640px){
      .container{padding:0 20px}
      .hero .container{padding:44px 20px 34px}
      .hero h2{font-size:34px}
      .faq-question{font-size:16px;padding:20px 24px}
      .faq-answer-content{padding:0 24px 24px 24px;font-size:15px}
    }
    @media (min-width: 980px){
      .hero .container{padding:68px 24px 48px}
      .hero-card{padding:22px}
      .hero h2{font-size:44px}
      .hero p{font-size:16.5px}
    }
    html{scroll-behavior:smooth}
  </style>



  <!-- HEADER -->
  <header class="header">
    <div class="container">
      <div class="header-wrap">
        <div class="brand">
          <h1>Elite Home Services</h1>
          <p>Professional Home Improvement • London, ON</p>
        </div>

        <div class="header-actions">
          <a class="pill" href="tel:+15198518887">📞 <strong>+1 (519) 851-8887</strong></a>
          <a class="pill" href="mailto:contact@elitehomeservices.ca">✉️ <strong>contact@elitehomeservices.ca</strong></a>
        </div>
      </div>
    </div>
  </header>

  <!-- HERO -->
  <section class="hero">
    <div class="container">
      <div class="hero-card">
        <h2>Frequently Asked Questions</h2>
        <p>
          Find answers to common questions about our services, pricing, and process. Can't find what you're looking for? Contact us directly.
        </p>

        <div class="hero-cta">
          <a class="btn btn-primary" href="/contact/">Contact Us</a>
          <a class="btn btn-outline" href="/services/">Our Services</a>
        </div>

        <div class="badges">
          <span class="badge"><span class="dot"></span> Transparent Pricing</span>
          <span class="badge"><span class="dot"></span> Free Estimates</span>
          <span class="badge"><span class="dot"></span> Fully Insured</span>
        </div>
      </div>
    </div>
  </section>

  <!-- FAQ SECTION -->
  <section class="faq-section">
    <div class="faq-container">

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>1. What services do you offer?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            We provide a wide range of home services including flooring installation, fencing, painting, and general home improvements. Our goal is to handle your project from start to finish with professional results.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>2. Do you work on both small and large projects?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Yes. We take on projects of all sizes, from small repairs to full home upgrades. Every job receives the same level of care and attention.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>3. How can I request a quote?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            You can contact us by phone, through our contact form, or by email. We'll review your project details and provide a clear and fair estimate.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>4. Is the estimate free?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Yes, all estimates are completely free and come with no obligation.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>5. How long does a typical project take?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Project timelines depend on the size and type of work. After reviewing your project, we'll give you a clear timeframe before starting.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>6. Do you help with material selection?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Absolutely. We can guide you in choosing the right materials, styles, and finishes that suit your space and budget.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>7. Are your prices fixed or can they change?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Our prices are transparent. Once the scope is agreed upon, there are no unexpected charges unless additional work is requested.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>8. Do you provide a warranty on your work?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Yes, we stand behind our workmanship and ensure every project meets our quality standards.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>9. Are you insured?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Yes, we are fully insured to protect both our team and our clients.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>10. Do I need to prepare my home before work starts?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            We'll let you know in advance if any preparation is needed. Our team also takes care to protect your home during the project.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>11. Will my home be left clean after the job is done?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Yes. Clean finishing and proper cleanup are a core part of our service.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>12. Can I see examples of your previous work?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Yes, you can view our completed projects in the <a href="/Our Projects/" style="color:var(--accent);font-weight:600;">Our Projects</a> section of our website.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>13. Do you work on residential properties only?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Our primary focus is residential projects, but feel free to contact us to discuss your specific needs.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>14. How far in advance should I book a service?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            We recommend booking as early as possible, especially during busy seasons, to secure your preferred time.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>15. Do you work year-round?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Yes, we operate year-round, with scheduling depending on weather conditions for certain outdoor services.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>16. What makes your company different from others?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            We focus on reliable service, clean finishing, honest pricing, and clear communication from start to finish.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>17. Can I make changes during the project?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Yes, changes can be discussed during the project. We'll always explain any impact on time or cost before proceeding.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>18. Do you offer emergency or urgent services?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Depending on availability, we do our best to accommodate urgent requests. Contact us directly for faster assistance.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>19. How do I contact you if I have questions during the project?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            You can reach us anytime by phone or message, and we'll keep you updated throughout the process.
          </div>
        </div>
      </div>

      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span>20. How do I get started?</span>
          <span class="faq-icon">+</span>
        </button>
        <div class="faq-answer">
          <div class="faq-answer-content">
            Simply contact us and tell us about your project. We'll take care of the rest—from planning to completion.
          </div>
        </div>
      </div>

    </div>
  </section>

  <!-- CTA SECTION -->
  <section class="cta-section">
    <div class="container">
      <h2>Still Have Questions?</h2>
      <p>We're here to help. Reach out to us anytime.</p>
      <a class="btn btn-primary" href="/contact/">Contact Us Today</a>
    </div>
  </section>

  <script>
    function toggleFaq(button) {
      const answer = button.nextElementSibling;
      const isOpen = answer.classList.contains('open');
      
      // Close all other FAQs
      document.querySelectorAll('.faq-answer').forEach(item => {
        item.classList.remove('open');
      });
      document.querySelectorAll('.faq-question').forEach(item => {
        item.classList.remove('active');
      });
      
      // Toggle current FAQ
      if (!isOpen) {
        answer.classList.add('open');
        button.classList.add('active');
      }
    }
  </script>











# Footer





<meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elite Home Services Footer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&amp;display=swap" rel="stylesheet">
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
        }
    </style>



    <section class="py-12 text-white" style="background: linear-gradient(135deg, rgb(93,64,55) 0%, rgb(120,85,70) 50%, rgb(196,120,74) 100%);">
        <div class="container max-w-4xl mx-auto px-4 text-center">
            <h2 class="text-3xl md:text-4xl font-bold mb-4">Looking for Reliable Home Services?</h2>
            <p class="text-base md:text-lg opacity-90 mb-10 max-w-2xl mx-auto">
                Contact us today for a free estimate. We focus on quality workmanship, transparent pricing, and customer satisfaction.
            </p>
            
            <div class="flex flex-col justify-center items-center gap-3 mb-16">
                <a href="tel:+15198518887" class="flex items-center gap-2 bg-white/10 hover:bg-white/20 border border-white/20 rounded-full px-4 py-2 transition-all duration-300 hover:scale-105 text-sm md:text-base">
                    <span class="w-7 h-7 rounded-full bg-green-500 flex items-center justify-center flex-shrink-0">
                        <svg class="h-4 w-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path>
                        </svg>
                    </span>
                    <span class="font-bold">Call Now</span>
                </a>

                <a href="mailto:contact@elitehomeservices.ca" class="flex items-center gap-2 bg-white/10 hover:bg-white/20 border border-white/20 rounded-full px-4 py-2 transition-all duration-300 hover:scale-105 text-sm md:text-base">
                    <span class="w-7 h-7 rounded-full bg-amber-600 flex items-center justify-center flex-shrink-0">
                        <svg class="h-4 w-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
                        </svg>
                    </span>
                    <span class="font-bold">Email Us</span>
                </a>

                <a href="https://wa.me/15198518887" class="flex items-center gap-2 bg-white/10 hover:bg-white/20 border border-white/20 rounded-full px-4 py-2 transition-all duration-300 hover:scale-105 text-sm md:text-base">
                    <span class="w-7 h-7 rounded-full bg-emerald-500 flex items-center justify-center flex-shrink-0">
                        <svg class="h-4 w-4 text-white" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.890-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"></path>
                        </svg>
                    </span>
                    <span class="font-bold">WhatsApp</span>
                </a>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-left border-t border-white/10 pt-12">
                
                <div class="bg-white/5 backdrop-blur-sm border border-white/10 rounded-2xl p-6">
                    <div class="text-2xl font-bold mb-4" style="font-family: 'Playfair Display', serif;">Elite Home Services</div>
                    <p class="opacity-80 text-sm leading-relaxed mb-4">
                        Professional home improvement based in London, Ontario. We pride ourselves on clean finishing and reliable scheduling.
                    </p>
                    <div class="flex flex-wrap gap-2 mb-4">
                        <span class="text-xs font-bold px-3 py-1 rounded-full bg-white/10 border border-white/20">Clean Finishing</span>
                        <span class="text-xs font-bold px-3 py-1 rounded-full bg-white/10 border border-white/20">Reliable Scheduling</span>
                        <span class="text-xs font-bold px-3 py-1 rounded-full bg-white/10 border border-white/20">Quality Results</span>
                    </div>
                </div>

                <div class="bg-white/5 backdrop-blur-sm border border-white/10 rounded-2xl p-6">
                    <h4 class="text-base font-bold mb-4 pb-2 border-b border-amber-400 inline-block">Navigation</h4>
                    <div class="grid grid-cols-2 gap-4">
                        <ul class="space-y-2 text-sm opacity-80">
                            <li><a href="/" class="hover:underline hover:opacity-100">Home</a></li>
                            <li><a href="/services/" class="hover:underline hover:opacity-100">Services</a></li>
                            <li><a href="/Our Projects/" class="hover:underline hover:opacity-100">Our Projects</a></li>
                        </ul>
                        <ul class="space-y-2 text-sm opacity-80">
                            <li><a href="/about/" class="hover:underline hover:opacity-100">About Us</a></li>
                            <li><a href="/faqs/" class="hover:underline hover:opacity-100">FAQs</a></li>
                            <li><a href="/customer-reviews/" class="hover:underline hover:opacity-100">Reviews</a></li>
                            <li><a href="/contact/" class="hover:underline hover:opacity-100">Contact</a></li>
                        </ul>
                    </div>
                </div>

                <div class="bg-white/5 backdrop-blur-sm border border-white/10 rounded-2xl p-6">
                    <h4 class="text-base font-bold mb-4 pb-2 border-b border-amber-400 inline-block">Our Team</h4>
                    
                    <div class="space-y-2">
                        <div class="flex justify-between items-center bg-black/20 p-3 rounded-lg border border-white/5">
                            <span class="text-sm font-bold">Isa Hasan</span>
                            <a href="tel:+15196972361" class="text-sm opacity-90 hover:text-amber-300 font-mono">(519) 697-2361</a>
                        </div>
                        <div class="flex justify-between items-center bg-black/20 p-3 rounded-lg border border-white/5">
                            <span class="text-sm font-bold">Musa Hasan</span>
                            <a href="tel:+12265040348" class="text-sm opacity-90 hover:text-amber-300 font-mono">(226) 504-0348</a>
                        </div>
                        <div class="flex justify-between items-center bg-black/20 p-3 rounded-lg border border-white/5">
                            <span class="text-sm font-bold">Abdul Alali</span>
                            <a href="tel:+12264486508" class="text-sm opacity-90 hover:text-amber-300 font-mono">(226) 448-6508</a>
                        </div>
                    </div>

                    <div class="mt-4 pt-4 border-t border-white/10 flex flex-col gap-2">
                        <div class="flex gap-2 items-center text-sm opacity-80">
                            <span>📍</span> 1157 Oakcrossing Rd, London, ON
                        </div>
                        <div class="flex gap-2 items-center text-sm opacity-80">
                            <span>✉️</span> contact@elitehomeservices.ca
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="mt-12 text-center text-xs opacity-50">
                © 2026 Elite Home Services. Serving Ontario with Excellence.
            </div>
        </div>
    &lt;/</section>
