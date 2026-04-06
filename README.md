<style>
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
body {
  background: #f7f6f2;
  color: #1a1917;
  font-family: -apple-system, sans-serif;
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  text-align: center;
  padding: 2rem;
}
.card { max-width: 480px; }
.label { font-size: 0.75rem; letter-spacing: 0.1em; text-transform: uppercase; color: #6b6860; margin-bottom: 1.5rem; }
h1 { font-size: 1.5rem; font-weight: 500; line-height: 1.4; margin-bottom: 1rem; }
p { font-size: 0.9rem; color: #6b6860; line-height: 1.7; margin-bottom: 2rem; }
a.btn { display: inline-block; background: #2c5f8a; color: #fff; padding: 0.65rem 1.5rem; border-radius: 5px; font-size: 0.9rem; font-weight: 500; text-decoration: none; }
a.btn:hover { background: #1e4a6e; }
.countdown { margin-top: 1.5rem; font-size: 0.78rem; color: #6b6860; }
</style>

<meta http-equiv="refresh" content="15;url=https://kazeo57.github.io/">

<div class="card">
  <div class="label">Johannes Hounton</div>
  <h1>This portfolio has been updated.</h1>
  <p>The content is now available at a new address. You will be redirected automatically.</p>
  <a class="btn" href="https://kazeo57.github.io/">Go to new portfolio →</a>
  <div class="countdown">Automatic redirect in <span id="n">15</span> seconds...</div>
</div>

<script>
let n = 15;
const el = document.getElementById('n');
const t = setInterval(() => {
  n--;
  el.textContent = n;
  if (n <= 0) { clearInterval(t); window.location.href = 'https://kazeo57.github.io/'; }
}, 1000);
</script>