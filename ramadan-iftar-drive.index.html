<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Ramadan Iftar Drive | Elwak</title>
  <style>
    :root{
      --blue1:#0f4c75; --blue2:#0b3c5d; --blue3:#06283d;
      --gold:#ffd700; --green:#1eb53a; --card:rgba(255,255,255,.10);
    }
    body{
      margin:0; font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;
      background:radial-gradient(circle at top,var(--blue1),var(--blue2),var(--blue3));
      color:#fff; min-height:100vh; display:flex; align-items:center; justify-content:center; padding:18px;
    }
    .wrap{
      width:min(860px,100%);
      background:linear-gradient(to bottom right, rgba(255,255,255,0.14), rgba(255,255,255,0.06));
      border:1px solid rgba(255,255,255,.18);
      border-radius:22px; padding:22px; box-shadow:0 24px 55px rgba(0,0,0,.35);
      backdrop-filter: blur(12px);
    }
    .top{ text-align:center; }
    h1{ margin:0; font-size:clamp(1.35rem,3vw,2.1rem); font-weight:900; letter-spacing:.6px; }
    .sub{ margin:6px 0 12px; color:var(--gold); font-weight:800; letter-spacing:1.6px; text-transform:uppercase; font-size:.85rem; }
    .text{ margin:0 0 14px; opacity:.95; line-height:1.5; }

    .grid{
      display:grid;
      grid-template-columns: repeat(4, minmax(0,1fr));
      gap:10px;
      margin: 12px 0 10px;
    }
    .btn{
      border:0; border-radius:14px; padding:12px 10px; font-weight:900; cursor:pointer;
      background: rgba(255,255,255,.16); color:#fff;
    }
    .btn:hover{ background: rgba(255,255,255,.22); }
    .btn.sel{ background: var(--green); box-shadow: 0 10px 22px rgba(30,181,58,.35); }

    .row{ display:flex; gap:10px; flex-wrap:wrap; align-items:center; justify-content:center; margin-top:10px; }
    input{
      width: 240px; max-width:100%;
      padding:12px 14px; border-radius:14px;
      border:1px solid rgba(255,255,255,.25);
      background: rgba(0,0,0,.18); color:#fff; outline:none; font-size:1rem;
    }
    input::placeholder{ color: rgba(255,255,255,.7); }

    .panel{
      margin-top:14px;
      padding:14px;
      border-radius:16px;
      border:1px solid rgba(255,255,255,.18);
      background: rgba(0,0,0,.18);
    }

    .tillBox{
      margin-top:10px;
      padding:14px;
      border-radius:14px;
      background: var(--green);
      text-align:center;
      font-weight:900;
      letter-spacing:1px;
    }
    .tillNum{ font-size:1.9rem; letter-spacing:3px; margin-top:6px; }
    .mini{ font-size:.92rem; opacity:.9; line-height:1.45; margin:8px 0 0; }

    .actions{ display:flex; gap:10px; flex-wrap:wrap; margin-top:12px; justify-content:center; }
    .aBtn{
      border:0; border-radius:14px; padding:12px 14px; font-weight:900; cursor:pointer;
    }
    .primary{ background: var(--gold); color:#0b3c5d; }
    .secondary{ background: rgba(255,255,255,.16); color:#fff; }
    .danger{ background: rgba(255,255,255,.08); color:#fff; border:1px solid rgba(255,255,255,.18); }

    .foot{ text-align:center; margin-top:14px; font-size:.9rem; opacity:.85; }

    @media (max-width: 700px){
      .grid{ grid-template-columns: repeat(2, minmax(0,1fr)); }
    }
  </style>
</head>

<body>
  <div class="wrap">
    <div class="top">
      <h1>RAMADAN IFTAR DRIVE | ELWAK</h1>
      <div class="sub">Choose a challenge amount</div>
      <p class="text">Feed a fasting family for the sake of Allah, and earn His blessings.</p>
    </div>

    <div class="grid" id="amtGrid">
      <button class="btn" data-amt="100">KSh 100</button>
      <button class="btn" data-amt="200">KSh 200</button>
      <button class="btn" data-amt="300">KSh 300</button>
      <button class="btn" data-amt="500">KSh 500</button>
      <button class="btn" data-amt="1000">KSh 1,000</button>
      <button class="btn" data-amt="1500">KSh 1,500</button>
      <button class="btn" data-amt="2000">KSh 2,000</button>
      <button class="btn" data-amt="custom">Any Amount</button>
    </div>

    <div class="row">
      <input id="customAmt" type="number" min="1" inputmode="numeric" placeholder="Type any amount (e.g., 750)" />
    </div>

    <div class="panel">
      <div><b>Selected Amount:</b> <span id="selAmt">None</span></div>
      <div style="margin-top:6px;"><b>Reference Code:</b> <span id="ref">—</span></div>

      <div class="tillBox">
        BUY GOODS TILL
        <div class="tillNum">4341738</div>
      </div>

      <p class="mini">
        <b>How to pay:</b> Open M-Pesa → Lipa na M-Pesa → Buy Goods → Enter Till <b>4341738</b> →
        Enter Amount → Pay. <br/>
        After paying, click <b>Confirm via WhatsApp</b> so we can track your contribution using the reference code.
      </p>

      <div class="actions">
        <button class="aBtn primary" onclick="copyTill()">Copy Till</button>
        <button class="aBtn secondary" onclick="copyRef()">Copy Reference</button>
        <button class="aBtn primary" onclick="confirmWhatsApp()">Confirm via WhatsApp</button>
        <button class="aBtn danger" onclick="resetAll()">Reset</button>
      </div>
    </div>

    <div class="foot">Ramadan • Mercy • Shared Responsibility</div>
  </div>

<script>
  const ORG_WHATSAPP_NUMBER = "254727496308"; // WhatsApp number for donation confirmations
  const TILL = "4341738";

  let selectedAmount = null;

  const selAmtEl = document.getElementById("selAmt");
  const refEl = document.getElementById("ref");
  const customAmt = document.getElementById("customAmt");
  const buttons = document.querySelectorAll(".btn");

  function genRef(){
    // short unique ref: ELW + date + random
    const d = new Date();
    const y = String(d.getFullYear()).slice(2);
    const m = String(d.getMonth()+1).padStart(2,"0");
    const day = String(d.getDate()).padStart(2,"0");
    const rnd = Math.random().toString(36).slice(2,6).toUpperCase();
    return `ELW-${y}${m}${day}-${rnd}`;
  }

  function setAmount(val){
    selectedAmount = val;
    selAmtEl.textContent = `KSh ${val.toLocaleString()}`;
    refEl.textContent = genRef();
    // Save locally (so user can refresh and not lose)
    localStorage.setItem("elw_amt", String(val));
    localStorage.setItem("elw_ref", refEl.textContent);
  }

  buttons.forEach(btn=>{
    btn.addEventListener("click", ()=>{
      buttons.forEach(b=>b.classList.remove("sel"));
      btn.classList.add("sel");
      const v = btn.dataset.amt;
      if(v === "custom"){
        selectedAmount = null;
        selAmtEl.textContent = "Custom amount";
        refEl.textContent = genRef();
        localStorage.setItem("elw_ref", refEl.textContent);
        customAmt.focus();
      } else {
        customAmt.value = "";
        setAmount(Number(v));
      }
    });
  });

  customAmt.addEventListener("input", ()=>{
    const v = Number(customAmt.value);
    if(v > 0){
      buttons.forEach(b=>b.classList.remove("sel"));
      selAmtEl.textContent = `KSh ${v.toLocaleString()}`;
      selectedAmount = v;
      if(refEl.textContent === "—") refEl.textContent = genRef();
      localStorage.setItem("elw_amt", String(v));
      localStorage.setItem("elw_ref", refEl.textContent);
    }
  });

  function copyTill(){
    navigator.clipboard.writeText(TILL).then(()=> alert("Till number copied."));
  }
  function copyRef(){
    const r = refEl.textContent;
    if(!r || r==="—") return alert("Select an amount first.");
    navigator.clipboard.writeText(r).then(()=> alert("Reference copied."));
  }

  function confirmWhatsApp(){
    const r = refEl.textContent;
    const amt = selectedAmount || Number(localStorage.getItem("elw_amt"));
    if(!amt || !r || r==="—"){
      alert("Select an amount first.");
      return;
    }
    const msg =
`RAMADAN IFTAR DRIVE | ELWAK
I have paid: KSh ${amt}
Till: ${TILL}
Reference: ${r}
May Allah accept.`;

    const url = `https://wa.me/${ORG_WHATSAPP_NUMBER}?text=${encodeURIComponent(msg)}`;
    window.open(url, "_blank");
  }

  function resetAll(){
    selectedAmount = null;
    customAmt.value = "";
    selAmtEl.textContent = "None";
    refEl.textContent = "—";
    buttons.forEach(b=>b.classList.remove("sel"));
    localStorage.removeItem("elw_amt");
    localStorage.removeItem("elw_ref");
  }

  // Restore if refreshed
  const savedAmt = Number(localStorage.getItem("elw_amt"));
  const savedRef = localStorage.getItem("elw_ref");
  if(savedRef) refEl.textContent = savedRef;
  if(savedAmt){
    selectedAmount = savedAmt;
    selAmtEl.textContent = `KSh ${savedAmt.toLocaleString()}`;
  }
</script>
</body>
</html>
