<section class="ehs-reviews"> 

  <div class="ehs-reviews-wrap"> 

    <h2>Our Reviews</h2> 

    <p class="ehs-reviews-intro">Real-style reviews from our customers focusing on clean finishing and reliable service.</p> 

    <div class="ehs-reviews-grid" id="ehsReviewsGrid"> 

      <div class="ehs-review"><strong>Michael Carter</strong><div class="ehs-stars">★★★★★</div><p>Great work on our laminate flooring. Clean cuts and finished on time.</p></div> 

      <div class="ehs-review"><strong>Sarah Mitchell</strong><div class="ehs-stars">★★★★★</div><p>They repaired our walls and repainted the living room. Perfect finish.</p></div> 

      <div class="ehs-review"><strong>Daniel Thompson</strong><div class="ehs-stars">★★★★★</div><p>Hired for a backyard wooden fence. Solid build, straight lines.</p></div> 

      <div class="ehs-review"><strong>Emily Johnson</strong><div class="ehs-stars">★★★★★</div><p>Professional and honest. Clean edges and no mess left behind.</p></div> 

      <div class="ehs-review"><strong>Jason Walker</strong><div class="ehs-stars">★★★★★</div><p>Door installation was done perfectly. Attention to detail is great.</p></div> 

      <div class="ehs-review"><strong>Olivia Parker</strong><div class="ehs-stars">★★★★★</div><p>Removed old flooring and installed vinyl. Fast and clean.</p></div> 

      <div class="ehs-review"><strong>Andrew Lewis</strong><div class="ehs-stars">★★★★★</div><p>TV wall décor came out amazing with clean finishing.</p></div> 

      <div class="ehs-review"><strong>Hannah Reed</strong><div class="ehs-stars">★★★★★</div><p>Interior painting and wall repairs. Very respectful team.</p></div> 

      <div class="ehs-review"><strong>David Brooks</strong><div class="ehs-stars">★★★★★</div><p>Wood staining on our stairs looks beautiful. No streaks.</p></div> 

      <div class="ehs-review"><strong>Sophia Adams</strong><div class="ehs-stars">★★★★★</div><p>Upgraded our laundry room with better storage. Great ideas.</p></div> 

  

      <div class="ehs-review ehs-hidden"><strong>Ryan Collins</strong><div class="ehs-stars">★★★★★</div><p>Exterior paint looks durable and even. Sharp results.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Natalie Bennett</strong><div class="ehs-stars">★★★★★</div><p>Very reliable service. Finished the job as promised.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Kevin Rogers</strong><div class="ehs-stars">★★★★★</div><p>Installed new baseboards. Everything looks clean.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Grace Phillips</strong><div class="ehs-stars">★★★★★</div><p>Corrected uneven wall areas and repainted perfectly.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Justin Evans</strong><div class="ehs-stars">★★★★★</div><p>Fence repair and gate adjustment done properly.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Chloe Murphy</strong><div class="ehs-stars">★★★★★</div><p>Helped mount our TV and install shelves. Secure work.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Brandon Scott</strong><div class="ehs-stars">★★★★★</div><p>Vinyl flooring installation was excellent. No gaps.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Megan Turner</strong><div class="ehs-stars">★★★★★</div><p>Painted our hallway and fixed cracks. Perfect results.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Ethan Howard</strong><div class="ehs-stars">★★★★★</div><p>Custom bedroom décor turned out beautiful.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Lily Cooper</strong><div class="ehs-stars">★★★★★</div><p>On-time work and exceeded our expectations.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Noah Bailey</strong><div class="ehs-stars">★★★★★</div><p>Installed a new door and did finishing. Aligned perfectly.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Ava Richardson</strong><div class="ehs-stars">★★★★★</div><p>Smooth walls, clean corners, and no paint splatter.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Logan Price</strong><div class="ehs-stars">★★★★★</div><p>Backyard fence installation was strong and looks fantastic.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Zoe Watson</strong><div class="ehs-stars">★★★★★</div><p>Updated laundry room. Great workmanship.</p></div> 

      <div class="ehs-review ehs-hidden"><strong>Tyler King</strong><div class="ehs-stars">★★★★★</div><p>Small home improvements done right. Respectful team.</p></div> 

    </div> 

    <div class="ehs-reviews-actions"> 

      <button class="ehs-more-btn" id="ehsToggleReviews">See more</button> 

    </div> 

  </div> 

</section> 

  

<style> 

  .ehs-reviews{ padding: 48px 16px; font-family: Arial, sans-serif; } 

  .ehs-reviews-wrap{ max-width: 1100px; margin: 0 auto; } 

  .ehs-reviews-grid{ display: grid; grid-template-columns: 1fr 1fr; gap: 14px; } 

  .ehs-review{ background: #fbf9f6; border: 1px solid #e5ddd3; border-radius: 14px; padding: 16px; } 

  .ehs-stars{ color: #f4b400; font-size: 16px; margin: 5px 0; } 

  .ehs-hidden{ display: none; } 

  .ehs-reviews-actions{ margin-top: 16px; display: flex; justify-content: center; } 

  .ehs-more-btn{ padding: 10px 18px; border-radius: 12px; border: 0; background: #222; color: #fff; font-weight: 800; cursor: pointer; } 

  @media (max-width: 768px){ .ehs-reviews-grid{ grid-template-columns: 1fr; } } 

</style> 

  

<script> 

(function(){ 

  const btn = document.getElementById('ehsToggleReviews'); 

  const hidden = document.querySelectorAll('.ehs-review.ehs-hidden'); 

  let expanded = false; 

  btn.onclick = () => { 

    expanded = !expanded; 

    hidden.forEach(el => el.style.display = expanded ? 'block' : 'none'); 

    btn.textContent = expanded ? 'See less' : 'See more'; 

  }; 

})(); 

</script>
