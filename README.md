:root { --green:#1f6b3a; --leaf:#e7f3ea; --ink:#1d2a22; --line:#d5e2d9; --bg:#fbfaf5; }
* { box-sizing:border-box; }
body { margin:0; font-family:"Trebuchet MS",system-ui,sans-serif; background:var(--bg); color:var(--ink); }
header { display:flex; justify-content:space-between; align-items:center; gap:1rem; flex-wrap:wrap;
  padding:1rem 1.5rem; background:var(--green); color:#fff; }
header h1 { margin:0; font-size:1.6rem; }
input { padding:.6rem .8rem; border:1px solid var(--line); border-radius:6px; font:inherit; }
header input { width:260px; max-width:100%; }
main { display:grid; grid-template-columns:1fr 320px; gap:1.5rem; padding:1.5rem; max-width:1200px; margin:auto; }
#categories { display:flex; gap:.5rem; flex-wrap:wrap; margin-bottom:1rem; }
#categories button { padding:.4rem .9rem; border:1px solid var(--green); border-radius:20px; background:#fff; color:var(--green); cursor:pointer; font:inherit; }
#categories button.active { background:var(--green); color:#fff; }
.grid { display:grid; grid-template-columns:repeat(auto-fill,minmax(160px,1fr)); gap:1rem; }
.card { background:#fff; border:1px solid var(--line); border-radius:10px; padding:1rem; text-align:center; }
.card .emoji { font-size:2.6rem; }
.card h3 { margin:.4rem 0; font-size:1rem; }
.card .price { color:var(--green); font-weight:bold; }
.card small { display:block; color:#6b7a70; margin-bottom:.5rem; }
button.add, #checkout { background:var(--green); color:#fff; border:0; border-radius:6px; padding:.5rem .9rem; cursor:pointer; font:inherit; }
button:disabled { background:#aab5ae; cursor:not-allowed; }
button:focus-visible, input:focus-visible { outline:3px solid #f2b705; }
#cart { background:var(--leaf); border-radius:10px; padding:1rem; height:fit-content; position:sticky; top:1rem; display:flex; flex-direction:column; gap:.6rem; }
#cart h2 { margin:0; }
#cart ul { list-style:none; padding:0; margin:0; }
#cart li { display:flex; justify-content:space-between; align-items:center; gap:.4rem; padding:.4rem 0; border-bottom:1px solid var(--line); font-size:.9rem; }
#cart li button { border:1px solid var(--green); background:#fff; border-radius:4px; width:26px; cursor:pointer; }
.total { margin:.3rem 0; }
#msg { margin:0; font-size:.9rem; }
.error { color:#b3261e; } .ok { color:var(--green); }
@media (max-width:800px) { main { grid-template-columns:1fr; } #cart { position:static; } }
