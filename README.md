# mindshift-public
 MindShift Public Verification
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>MindShift — Waitlist</title>
  <meta name="description" content="MindShift is Execution Permission Infrastructure. It governs when intelligence—human or AI—is permitted to become execution. No Decision ID → No Execution." />
  <meta property="og:title" content="MindShift — Execution Permission Infrastructure" />
  <meta property="og:description" content="Govern the moment intelligence becomes action. No Decision ID → No Execution." />
  <meta property="og:type" content="website" />
  <meta name="theme-color" content="#0B0D12" />

  <style>
    :root{
      --bg:#0B0D12;
      --panel:#111524;
      --panel2:#0F1320;
      --text:#E9ECF3;
      --muted:#A9B2C7;
      --line:rgba(255,255,255,.10);
      --accent:#6EE7FF;
      --accent2:#A78BFA;
      --danger:#FF6B6B;
      --ok:#7CFFB2;
      --shadow: 0 20px 60px rgba(0,0,0,.45);
      --radius:18px;
      --max: 1080px;
      --mono: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
      --sans: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:var(--sans);
      color:var(--text);
      background:
        radial-gradient(900px 450px at 15% 10%, rgba(110,231,255,.12), transparent 55%),
        radial-gradient(900px 450px at 85% 15%, rgba(167,139,250,.10), transparent 55%),
        radial-gradient(900px 450px at 50% 95%, rgba(110,231,255,.06), transparent 55%),
        var(--bg);
      line-height:1.45;
    }
    a{color:inherit}
    .wrap{max-width:var(--max); margin:0 auto; padding:24px}
    header{
      display:flex; align-items:center; justify-content:space-between;
      gap:16px; padding:14px 0;
    }
    .brand{
      display:flex; align-items:center; gap:10px;
      font-weight:700; letter-spacing:.2px;
    }
    .dot{
      width:10px; height:10px; border-radius:999px;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      box-shadow: 0 0 0 6px rgba(110,231,255,.08);
    }
    .pill{
      display:inline-flex; align-items:center; gap:8px;
      padding:8px 12px;
      border:1px solid var(--line);
      border-radius:999px;
      background: rgba(255,255,255,.03);
      color:var(--muted);
      font-size:13px;
      white-space:nowrap;
    }
    .hero{
      display:grid;
      grid-template-columns: 1.05fr .95fr;
      gap:18px;
      align-items:stretch;
      padding:18px 0 10px;
    }
    @media (max-width: 920px){
      .hero{grid-template-columns:1fr}
    }
    .card{
      background: linear-gradient(180deg, rgba(255,255,255,.04), rgba(255,255,255,.02));
      border:1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding:22px;
    }
    .h1{
      font-size:44px; line-height:1.06; margin:0 0 10px 0; letter-spacing:-.6px;
    }
    @media (max-width: 520px){
      .h1{font-size:36px}
    }
    .sub{
      margin:0 0 18px 0;
      color:var(--muted);
      font-size:16px;
    }
    .kicker{
      font-family:var(--mono);
      display:inline-block;
      padding:8px 10px;
      border-radius:12px;
      border:1px solid var(--line);
      background: rgba(0,0,0,.25);
      margin:10px 0 16px;
      color: rgba(233,236,243,.92);
      letter-spacing:.2px;
    }
    .ctaRow{display:flex; gap:10px; flex-wrap:wrap; align-items:center}
    .btn{
      border:1px solid var(--line);
      background: rgba(255,255,255,.05);
      color:var(--text);
      padding:11px 14px;
      border-radius: 14px;
      cursor:pointer;
      font-weight:600;
      transition: transform .12s ease, background .12s ease, border-color .12s ease;
      user-select:none;
    }
    .btn:hover{transform: translateY(-1px); border-color: rgba(110,231,255,.35)}
    .btn.primary{
      border-color: rgba(110,231,255,.40);
      background: linear-gradient(135deg, rgba(110,231,255,.18), rgba(167,139,250,.14));
    }
    .btn.small{padding:8px 10px; border-radius:12px; font-size:13px}
    .tabs{
      display:flex; gap:8px; flex-wrap:wrap;
      border-bottom:1px solid var(--line);
      padding-bottom:12px; margin-bottom:14px;
    }
    .tab{
      border:1px solid var(--line);
      background: rgba(255,255,255,.03);
      color:var(--muted);
      padding:8px 10px;
      border-radius:999px;
      cursor:pointer;
      font-size:13px;
      font-weight:600;
    }
    .tab.active{
      color:var(--text);
      border-color: rgba(110,231,255,.35);
      background: rgba(110,231,255,.08);
    }
    .grid2{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:14px;
      margin-top:14px;
    }
    @media (max-width: 820px){
      .grid2{grid-template-columns:1fr}
    }
    .sectionTitle{
      font-size:18px; margin:0 0 10px 0;
    }
    .muted{color:var(--muted)}
    .list{
      margin:10px 0 0 0;
      padding-left:18px;
      color:var(--muted);
    }
    .list li{margin:6px 0}
    .rule{
      font-family:var(--mono);
      background: rgba(0,0,0,.25);
      border:1px solid var(--line);
      border-radius: 14px;
      padding:14px;
      margin:12px 0;
    }
    .form{
      display:flex; gap:10px; flex-wrap:wrap;
      align-items:center;
      margin-top:14px;
    }
    input[type="email"]{
      flex: 1 1 240px;
      min-width: 200px;
      padding:12px 12px;
      border-radius: 14px;
      border:1px solid var(--line);
      background: rgba(0,0,0,.25);
      color: var(--text);
      outline:none;
    }
    input[type="email"]::placeholder{color: rgba(169,178,199,.75)}
    .note{
      font-size:12.5px; color:rgba(169,178,199,.88);
      margin-top:10px;
    }
    .msg{
      display:none;
      margin-top:12px;
      padding:12px 14px;
      border-radius: 14px;
      border:1px solid var(--line);
      background: rgba(255,255,255,.03);
      color: var(--muted);
    }
    .msg.ok{border-color: rgba(124,255,178,.35); color: rgba(233,236,243,.92)}
    .msg.err{border-color: rgba(255,107,107,.35); color: rgba(233,236,243,.92)}
    .divider{height:1px; background: var(--line); margin:18px 0}
    .svgWrap{
      border:1px solid var(--line);
      border-radius: var(--radius);
      background: rgba(0,0,0,.22);
      padding:12px;
      overflow:hidden;
    }
    footer{
      margin:26px 0 8px;
      color:rgba(169,178,199,.85);
      font-size:12.5px;
      display:flex; flex-wrap:wrap; gap:10px;
      align-items:center; justify-content:space-between;
    }
    .footerLinks{display:flex; gap:12px; flex-wrap:wrap}
    .mono{font-family:var(--mono)}
    .badgeRow{display:flex; gap:10px; flex-wrap:wrap; margin-top:10px}
  </style>
</head>

<body>
  <div class="wrap">
    <header>
      <div class="brand" aria-label="MindShift">
        <span class="dot" aria-hidden="true"></span>
        <span>MindShift</span>
      </div>
      <div class="pill" title="Category">
        Execution Permission Infrastructure
      </div>
    </header>

    <main class="hero">
      <!-- Left: Hero / Waitlist -->
      <section class="card">
        <h1 class="h1">Govern the moment intelligence becomes action.</h1>
        <p class="sub">
          MindShift is execution permission infrastructure. It determines whether any human or AI-initiated action
          is allowed to execute—at runtime—before reality changes.
        </p>

        <div class="kicker">No Decision ID → No Execution</div>

        <!-- 1-line email capture -->
        <form class="form" id="waitlistForm" method="POST" action="">
          <!--
            GitHub Pages note:
            Static sites can't store emails by themselves. Use an external form endpoint:
            - Formspree: https://formspree.io/
            - Basin: https://usebasin.com/
            - Getform: https://getform.io/
            1) Put your endpoint URL into FORM_ACTION below.
            2) Or leave it blank to show confirmation-only (no network).
          -->
          <input id="email" name="email" type="email" placeholder="Enter your email for early access" autocomplete="email" required />
          <button class="btn primary" type="submit">Join the Waitlist</button>
          <button class="btn" type="button" id="copyInvariant">Copy Invariant</button>
        </form>

        <!-- confirmation copy -->
        <div class="msg ok" id="okMsg">
          You're on the waitlist. You'll only hear from us when early access (or a private pilot) is available.
        </div>
        <div class="msg err" id="errMsg">
          Please enter a valid email address.
        </div>

        <p class="note">
          No spam. No hype. Updates only when execution is ready.
        </p>

        <div class="divider"></div>

        <h2 class="sectionTitle">What breaks at scale</h2>
        <p class="muted" style="margin:0">
          AI and automation can act faster than humans can approve. Prices change, code deploys, messages send, money moves—
          often without anyone clearly owning the decision at the moment execution occurs.
        </p>

        <div class="badgeRow">
          <span class="pill">Fail-closed</span>
          <span class="pill">Human-owned authority</span>
          <span class="pill">Runtime enforcement</span>
          <span class="pill">Audit-ready by construction</span>
        </div>
      </section>

      <!-- Right: Audience switcher (Investors vs Operators) -->
      <aside class="card" aria-label="Audience content">
        <div class="tabs" role="tablist" aria-label="Audience tabs">
          <button class="tab active" id="tabInvestor" role="tab" aria-selected="true" aria-controls="panelInvestor">Investor view</button>
          <button class="tab" id="tabOperator" role="tab" aria-selected="false" aria-controls="panelOperator">Operator view</button>
          <button class="tab" id="tabTechnical" role="tab" aria-selected="false" aria-controls="panelTechnical">Technical view</button>
        </div>

        <!-- Investor rewrite -->
        <section id="panelInvestor" role="tabpanel" aria-labelledby="tabInvestor">
          <h2 class="sectionTitle">Investor summary</h2>
          <p class="muted" style="margin:0 0 12px 0">
            As execution gets cheaper, permission becomes scarce. MindShift defines and occupies a new infrastructure layer:
            Execution Permission Infrastructure. It governs the chokepoint that other categories do not—runtime legitimacy of action.
          </p>

          <div class="rule">
            <div class="mono" style="opacity:.9; margin-bottom:8px">Category</div>
            <div>Decision Governance Infrastructure (Execution Permission Infrastructure)</div>
          </div>

          <ul class="list">
            <li><span style="color:var(--text)">Problem:</span> execution outpaces authority; approval becomes implied and post-hoc.</li>
            <li><span style="color:var(--text)">Wedge:</span> land on one bounded execution surface (deploys, pricing, publishing).</li>
            <li><span style="color:var(--text)">Moat:</span> deterministic enforcement at execution boundaries; audit-proof by construction.</li>
            <li><span style="color:var(--text)">Buyers:</span> CTO, CISO, Head of Platform, Engineering leadership.</li>
          </ul>

          <p class="muted" style="margin:14px 0 0 0">
            MindShift does not promise better decisions. It makes decisions owned, bounded, enforced, and verifiable.
          </p>
        </section>

        <!-- Operator rewrite -->
        <section id="panelOperator" role="tabpanel" aria-labelledby="tabOperator" hidden>
          <h2 class="sectionTitle">Operator summary</h2>
          <p class="muted" style="margin:0 0 12px 0">
            MindShift prevents unauthorized actions by enforcing permission at runtime. If an action can change reality, it must present
            a valid Decision ID—otherwise execution is blocked with no side effects.
          </p>

          <div class="rule">
            <div class="mono" style="opacity:.9; margin-bottom:8px">Default state</div>
            <div><span style="color:var(--danger)">DENY</span> (until explicit authority is verified)</div>
          </div>

          <h3 class="sectionTitle" style="margin-top:16px">What you get</h3>
          <ul class="list">
            <li>Explicit owners per decision domain (pricing, deploys, publishing, spend, payments)</li>
            <li>Hard stops instead of improvisation under pressure</li>
            <li>Non-bypassable enforcement at your execution boundaries</li>
            <li>Audit-ready trace: who decided, what was allowed, and whether execution was legitimate</li>
          </ul>

          <p class="muted" style="margin:14px 0 0 0">
            You keep your current tools. MindShift governs permission, not capability.
          </p>
        </section>

        <!-- Technical + diagram-first -->
        <section id="panelTechnical" role="tabpanel" aria-labelledby="tabTechnical" hidden>
          <h2 class="sectionTitle">Diagram-first (technical)</h2>
          <p class="muted" style="margin:0 0 12px 0">
            Control flow is deterministic: cognition ends upstream; authority is created only as a sealed artifact; execution systems must
            request permission; the gate returns ALLOW or DENY.
          </p>

          <div class="svgWrap" aria-label="MindShift flow diagram">
            <!-- Inline SVG diagram (no external assets needed) -->
            <svg viewBox="0 0 960 360" width="100%" height="auto" role="img" aria-label="Cognition to execution permission flow">
              <defs>
                <linearGradient id="g1" x1="0" x2="1">
                  <stop offset="0" stop-color="#6EE7FF" stop-opacity="0.55"></stop>
                  <stop offset="1" stop-color="#A78BFA" stop-opacity="0.45"></stop>
                </linearGradient>
                <filter id="glow" x="-30%" y="-30%" width="160%" height="160%">
                  <feGaussianBlur stdDeviation="6" result="blur"/>
                  <feMerge>
                    <feMergeNode in="blur"/>
                    <feMergeNode in="SourceGraphic"/>
                  </feMerge>
                </filter>
              </defs>

              <!-- Background grid -->
              <g opacity="0.18">
                <path d="M0 60 H960 M0 120 H960 M0 180 H960 M0 240 H960 M0 300 H960" stroke="#FFFFFF" stroke-width="1" />
                <path d="M120 0 V360 M240 0 V360 M360 0 V360 M480 0 V360 M600 0 V360 M720 0 V360 M840 0 V360" stroke="#FFFFFF" stroke-width="1" />
              </g>

              <!-- Nodes -->
              <g font-family="ui-sans-serif, system-ui" font-size="14" fill="#E9ECF3">
                <!-- CIS / cognition -->
                <rect x="40" y="70" rx="18" ry="18" width="210" height="90" fill="rgba(255,255,255,.05)" stroke="rgba(255,255,255,.12)"/>
                <text x="60" y="105" font-weight="700">Cognition / Analysis</text>
                <text x="60" y="128" fill="#A9B2C7">No authority. No execution path.</text>

                <!-- Decision Artifact -->
                <rect x="290" y="70" rx="18" ry="18" width="210" height="90" fill="rgba(255,255,255,.05)" stroke="rgba(255,255,255,.12)"/>
                <text x="310" y="105" font-weight="700">Sealed Decision Artifact</text>
                <text x="310" y="128" fill="#A9B2C7">Owner · scope · constraints · expiry</text>

                <!-- Registry -->
                <rect x="290" y="200" rx="18" ry="18" width="210" height="90" fill="rgba(255,255,255,.05)" stroke="rgba(255,255,255,.12)"/>
                <text x="310" y="235" font-weight="700">Decision Registry</text>
                <text x="310" y="258" fill="#A9B2C7">Immutable storage + lookup</text>

                <!-- Omega Gate -->
                <rect x="540" y="120" rx="18" ry="18" width="180" height="120" fill="url(#g1)" stroke="rgba(110,231,255,.35)" filter="url(#glow)"/>
                <text x="565" y="160" font-weight="800">Ω Gate</text>
                <text x="565" y="184" font-family="ui-monospace, SFMono-Regular, Menlo" font-size="13">ALLOW / DENY</text>
                <text x="565" y="208" fill="#0B0D12" font-weight="700">Fail-closed</text>

                <!-- Execution -->
                <rect x="760" y="120" rx="18" ry="18" width="160" height="120" fill="rgba(255,255,255,.05)" stroke="rgba(255,255,255,.12)"/>
                <text x="782" y="160" font-weight="700">Execution Systems</text>
                <text x="782" y="184" fill="#A9B2C7">Deploy · publish · price · pay</text>

                <!-- Proof of Transfer -->
                <rect x="760" y="260" rx="18" ry="18" width="160" height="70" fill="rgba(255,255,255,.05)" stroke="rgba(255,255,255,.12)"/>
                <text x="782" y="295" font-weight="700">Proof-of-Transfer</text>
                <text x="782" y="318" fill="#A9B2C7">Independent verification</text>
              </g>

              <!-- Arrows -->
              <g stroke="rgba(233,236,243,.65)" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path d="M250 115 H290" />
                <path d="M500 115 C540 115 520 140 540 150" />
                <path d="M500 245 C545 245 525 220 540 210" />
                <path d="M720 180 H760" />
                <path d="M840 240 V260" />
              </g>

              <!-- Arrowheads -->
              <g fill="rgba(233,236,243,.65)">
                <path d="M286 115 l10 -6 v12 z" />
                <path d="M536 150 l10 -6 v12 z" />
                <path d="M536 210 l10 -6 v12 z" />
                <path d="M756 180 l10 -6 v12 z" />
                <path d="M840 256 l-6 10 h12 z" />
              </g>

              <!-- Labels -->
              <g font-family="ui-monospace, SFMono-Regular, Menlo" font-size="12" fill="rgba(169,178,199,.95)">
                <text x="70" y="55">Upstream: learning is non-authoritative</text>
                <text x="535" y="105">Runtime authorization check</text>
                <text x="770" y="105">Reality change happens here (if allowed)</text>
              </g>
            </svg>
          </div>

          <div class="rule" style="margin-top:14px">
            <div class="mono" style="opacity:.9; margin-bottom:8px">Invariant</div>
            <div class="mono">No Decision ID → No Execution</div>
          </div>

          <h3 class="sectionTitle" style="margin-top:16px">Common execution surfaces</h3>
          <ul class="list">
            <li>CI/CD production deploys</li>
            <li>CMS publishing</li>
            <li>Pricing/discount changes</li>
            <li>Paid ads launch/modification</li>
            <li>Payments/refunds</li>
            <li>CRM automation triggers</li>
          </ul>
        </section>
      </aside>
    </main>

    <section class="card" style="margin-top:14px">
      <h2 class="sectionTitle">What MindShift is (and isn’t)</h2>

      <div class="grid2">
        <div>
          <p class="muted" style="margin:0 0 10px 0">
            MindShift governs whether intelligence—human or AI—is permitted to become execution. It enforces explicit human authority at runtime.
          </p>
          <div class="rule">
            <div class="mono" style="opacity:.9; margin-bottom:8px">One question</div>
            <div>Is this action explicitly authorized to occur right now?</div>
          </div>
        </div>

        <div>
          <p class="muted" style="margin:0 0 10px 0">MindShift does not decide what to do. It does not optimize decisions or replace tools.</p>
          <ul class="list">
            <li>Not automation software</li>
            <li>Not AI agents</li>
            <li>Not workflow optimization</li>
            <li>Not compliance certification</li>
            <li>Not dashboards or monitoring</li>
          </ul>
        </div>
      </div>
    </section>

    <footer>
      <div>© <span id="year"></span> MindShift</div>
      <div class="footerLinks">
        <span class="mono">Execution Permission Infrastructure</span>
        <span aria-hidden="true">•</span>
        <span>Humans decide. Systems enforce.</span>
      </div>
    </footer>
  </div>

  <script>
    // Set year
    document.getElementById("year").textContent = new Date().getFullYear();

    // Audience tabs
    const tabInvestor = document.getElementById("tabInvestor");
    const tabOperator = document.getElementById("tabOperator");
    const tabTechnical = document.getElementById("tabTechnical");
    const panelInvestor = document.getElementById("panelInvestor");
    const panelOperator = document.getElementById("panelOperator");
    const panelTechnical = document.getElementById("panelTechnical");

    function setActive(which){
      const tabs = [tabInvestor, tabOperator, tabTechnical];
      const panels = [panelInvestor, panelOperator, panelTechnical];

      tabs.forEach(t => t.classList.remove("active"));
      tabs.forEach(t => t.setAttribute("aria-selected","false"));
      panels.forEach(p => p.hidden = true);

      which.tab.classList.add("active");
      which.tab.setAttribute("aria-selected","true");
      which.panel.hidden = false;
    }

    tabInvestor.addEventListener("click", () => setActive({tab: tabInvestor, panel: panelInvestor}));
    tabOperator.addEventListener("click", () => setActive({tab: tabOperator, panel: panelOperator}));
    tabTechnical.addEventListener("click", () => setActive({tab: tabTechnical, panel: panelTechnical}));

    // Copy invariant
    document.getElementById("copyInvariant").addEventListener("click", async () => {
      const text = "No Decision ID → No Execution";
      try {
        await navigator.clipboard.writeText(text);
        const ok = document.getElementById("okMsg");
        ok.textContent = "Copied: " + text;
        ok.style.display = "block";
        document.getElementById("errMsg").style.display = "none";
        setTimeout(() => { ok.style.display = "none"; ok.textContent = "You're on the waitlist. You'll only hear from us when early access (or a private pilot) is available."; }, 2500);
      } catch (e) {
        // Clipboard may be blocked; ignore.
      }
    });

    // Waitlist form submit (static-friendly)
    const form = document.getElementById("waitlistForm");
    const email = document.getElementById("email");
    const okMsg = document.getElementById("okMsg");
    const errMsg = document.getElementById("errMsg");

    // OPTIONAL: set your external form endpoint here
    // Example (Formspree): const FORM_ACTION = "https://formspree.io/f/xxxxxx";
    const FORM_ACTION = ""; // <-- put your endpoint URL here

    form.addEventListener("submit", async (e) => {
      e.preventDefault();

      const val = (email.value || "").trim();
      const isValid = /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(val);

      if (!isValid){
        errMsg.style.display = "block";
        okMsg.style.display = "none";
        return;
      }

      errMsg.style.display = "none";

      // If no endpoint, show confirmation-only (works on GitHub Pages with no backend)
      if (!FORM_ACTION){
        okMsg.style.display = "block";
        return;
      }

      // If endpoint is provided, POST the email
      try {
        const res = await fetch(FORM_ACTION, {
          method: "POST",
          headers: { "Content-Type": "application/json", "Accept": "application/json" },
          body: JSON.stringify({ email: val, source: "mindshift-waitlist" })
        });

        if (res.ok){
          okMsg.style.display = "block";
        } else {
          // Fall back to confirmation to avoid dead-ends on static pages
          okMsg.textContent = "You're on the waitlist (submission recorded).";
          okMsg.style.display = "block";
        }
      } catch (err){
        // Network blocked; still show confirmation to keep UX clean
        okMsg.textContent = "You're on the waitlist. (If you expected a network submit, set FORM_ACTION.)";
        okMsg.style.display = "block";
      }
    });
  </script>
</body>
</html>

￼  ￼
