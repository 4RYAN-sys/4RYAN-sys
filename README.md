<div align="center">

<!-- ========== CYBERPUNK PROFILE : 4RYAN-sys ========== -->

<style>
  :root {
    --bg: #0d1117;
    --panel: rgba(13, 17, 23, 0.55);
    --text: #c9d1d9;
    --muted: #8b949e;
    --cyan: #22d3ee;
    --yellow: #facc15;
    --line: rgba(34, 211, 238, 0.22);
    --scan: rgba(34, 211, 238, 0.05);
  }
  .cyber-panel, .cyber-header, .cyber-mission { background: var(--panel); }
  .cyber-box { display: inline-block; text-align: left; }
  .cyber-mono { font-family: ui-monospace, 'JetBrains Mono', 'Cascadia Mono', 'SF Mono', Consolas, monospace; }
  .cyber-label { font-family: ui-monospace, 'JetBrains Mono', 'Cascadia Mono', monospace; letter-spacing: 0.18em; text-transform: uppercase; }
  .cyan { color: var(--cyan); }
  .yellow { color: var(--yellow); }
  .muted { color: var(--muted); }
  .grid-panel {
    border: 1px solid rgba(34, 211, 238, 0.18);
    border-radius: 8px;
    background: var(--panel);
    padding: 12px 16px;
    box-shadow: inset 0 0 0 1px rgba(34, 211, 238, 0.04), 0 0 18px rgba(34, 211, 238, 0.06);
  }
  .td-pill {
    border: 1px solid rgba(34, 211, 238, 0.25);
    border-radius: 4px;
    padding: 2px 8px;
    font-family: ui-monospace, 'JetBrains Mono', 'Cascadia Mono', monospace;
    font-size: 12px;
    display: inline-block;
    margin: 2px;
    color: var(--text);
  }
  .td-pill.y { border-color: rgba(250, 204, 21, 0.3); }
  .stat-chip {
    border: 1px solid rgba(34, 211, 238, 0.2);
    border-radius: 4px;
    padding: 3px 10px;
    font-family: ui-monospace, 'JetBrains Mono', 'Cascadia Mono', monospace;
    font-size: 12px;
  }
  @keyframes blink { 0%, 49% { opacity: 1; } 50%, 100% { opacity: 0; } }
  .cursor { animation: blink 1.1s step-end infinite; }
  @media (prefers-color-scheme: light) {
    :root {
      --bg: #ffffff;
      --panel: rgba(22, 27, 34, 0.04);
      --text: #1f2328;
      --muted: #59636e;
    }
  }
</style>

<!-- ================= HEADER ================= -->

<div class="cyber-header" style="position:relative; overflow:hidden; border:1px solid rgba(34,211,238,0.25); border-radius:10px; padding:6px; background:var(--panel); box-shadow: inset 0 0 30px rgba(34,211,238,0.05), 0 0 20px rgba(34,211,238,0.08);">

  <!-- scanlines -->
  <svg width="100%" height="100%" style="position:absolute; inset:0; pointer-events:none;" aria-hidden="true">
    <defs>
      <pattern id="scan" width="4" height="6" patternUnits="userSpaceOnUse">
        <line x1="0" y1="0" x2="0" y2="6" stroke="#22d3ee" stroke-width="0.5" opacity="0.12"/>
      </pattern>
    </defs>
    <rect width="100%" height="100%" fill="url(#scan)" opacity="0.35"/>
  </svg>

  <div style="position:relative; border:1px solid rgba(34,211,238,0.12); border-radius:6px; padding:26px 20px;">

    <!-- matrix watermark -->
    <div style="position:absolute; inset:0; opacity:0.55; pointer-events:none; overflow:hidden; border-radius:6px;">
      <img width="100%" height="100%" src="assets/matrix.svg" alt="" style="object-fit:cover;"/>
    </div>

    <div style="position:relative; text-align:left; max-width:700px; margin:0 auto;">

      <div class="cyber-mono" style="font-size:12px; color:var(--muted);">
        <span class="cyan">$</span> whoami --profile
      </div>

      <!-- radar + name -->
      <div style="display:flex; align-items:center; gap:16px; margin:14px 0 6px;">
        <svg width="40" height="40" viewBox="0 0 40 40" aria-hidden="true">
          <circle cx="20" cy="20" r="18" fill="none" stroke="#22d3ee" stroke-width="1" opacity="0.4"/>
          <circle cx="20" cy="20" r="12" fill="none" stroke="#22d3ee" stroke-width="1" opacity="0.4"/>
          <circle cx="20" cy="20" r="6" fill="#facc15" opacity="0.35"/>
          <g>
            <line x1="20" y1="20" x2="34" y2="6" stroke="#22d3ee" stroke-width="1.4"/>
            <circle cx="34" cy="6" r="2" fill="#22d3ee"/>
            <animateTransform attributeName="transform" type="rotate" from="0 20 20" to="360 20 20" dur="3s" repeatCount="indefinite"/>
          </g>
          <circle cx="20" cy="20" r="18" fill="none" stroke="#facc15" stroke-width="1" opacity="0.5"/>
          <circle cx="20" cy="20" r="12" fill="none" stroke="#facc15" stroke-width="1" opacity="0.5"/>
          <animateTransform attributeName="transform" type="rotate" from="0 20 20" to="360 20 20" dur="6s" repeatCount="indefinite"/>
        </svg>
        <div>
          <div class="cyber-mono" style="font-size:30px; line-height:1.05; color:var(--text); letter-spacing:-0.5px;">
            4RYAN<span class="yellow">-sys</span>
          </div>
          <div class="cyber-label" style="font-size:11px; color:var(--cyan); margin-top:6px;">
            // system.init() <span class="cursor cyan" style="display:inline-block; width:1px; height:12px; background:var(--cyan); vertical-align:-1px;"></span>
          </div>
        </div>
      </div>

      <pre class="cyber-mono" style="margin:16px 0 6px; color:var(--muted); font-size:12px; line-height:1.6;">
<span class="cyan">┌──</span> AVARITIA <span class="yellow">::</span> RPL UNIT <span class="cyan">──</span><span class="yellow">╼</span> <span class="cyan">▛</span> INIT <span class="cyan">▜</span>
<span class="cyan">├─</span><span class="yellow">▣</span> mode    <span class="cyan">::</span> <span class="muted">fullstack + iot</span>
<span class="cyan">├─</span><span class="yellow">▣</span> shell   <span class="cyan">::</span> <span class="muted">github-profile v2.1</span>
<span class="cyan">└─</span><span class="yellow">▣</span> status  <span class="cyan">::</span> <span class="muted">online</span> <span class="cyan">[ OK ]</span></pre>

      <div style="display:flex; flex-wrap:wrap; gap:8px; margin-top:12px;">
        <span class="stat-chip" style="color:var(--cyan);">▶ TECH-REGION: ID</span>
        <span class="stat-chip" style="color:var(--yellow);">▲ ROLE: STUDENT</span>
        <span class="stat-chip" style="color:var(--muted);">▣ RPL // VOCATIONAL</span>
      </div>

    </div>
  </div>
</div>

<!-- ================= ABOUT / SYSINFO ================= -->

<br/>

<div class="cyber-box cyber-panel" style="width:100%; max-width:760px; border:1px solid rgba(34,211,238,0.18); border-radius:8px; overflow:hidden; box-shadow: inset 0 0 0 1px rgba(34,211,238,0.04);">

  <div class="cyber-label" style="font-size:11px; padding:8px 14px; color:var(--cyan); border-bottom:1px solid rgba(34,211,238,0.15); background:rgba(34,211,238,0.04);">
    ▚ SYSINFO // PROFILE.JSON
  </div>

  <pre class="cyber-mono" style="margin:0; padding:16px 18px; font-size:13px; line-height:1.7; color:var(--muted); text-align:left; overflow-x:auto;">
<span class="cyan">$</span> cat profile.json
<span class="yellow">{</span>
  <span class="cyan">"handle"</span>: <span class="muted">"4RYAN-sys"</span>,
  <span class="cyan">"role"</span>:    <span class="muted">"RPL Student :: Fullstack & IoT"</span>,
  <span class="cyan">"focus"</span>:   <span class="muted">[ "Fullstack Web", "Embedded IoT" ]</span>,
  <span class="cyan">"drive"</span>:   <span class="muted">"ship small systems that actually work"</span>,
  <span class="cyan">"build"</span>:   <span class="muted">{ "app": "Next.js", "board": "ESP32" }</span>
<span class="yellow">}</span></pre>

</div>

<br/>

<!-- ================= TECH STACK ================= -->

<div class="cyber-box" style="width:100%; max-width:760px;">

  <div class="cyber-label" style="font-size:11px; color:var(--yellow); margin-bottom:10px; text-align:left;">
    ▚ STACK // CYBER-PANEL
  </div>

  <table role="presentation" align="center" border="0" cellpadding="0" cellspacing="8">
    <tr>
      <td width="50%">
        <div class="grid-panel" style="text-align:left;">
          <div class="cyber-label" style="font-size:10px; color:var(--cyan); margin-bottom:8px;">FRONTEND</div>
          <span class="td-pill">NEXT.JS</span><span class="td-pill">TYPESCRIPT</span><span class="td-pill">TAILWIND</span><span class="td-pill">HTML</span>
        </div>
      </td>
      <td width="50%">
        <div class="grid-panel" style="text-align:left;">
          <div class="cyber-label" style="font-size:10px; color:var(--cyan); margin-bottom:8px;">BACKEND</div>
          <span class="td-pill">NODE.JS</span><span class="td-pill">PYTHON</span><span class="td-pill">JAVA</span><span class="td-pill">LARAVEL</span><span class="td-pill">SUPABASE</span>
        </div>
      </td>
    </tr>
    <tr>
      <td width="50%">
        <div class="grid-panel" style="text-align:left;">
          <div class="cyber-label" style="font-size:10px; color:var(--cyan); margin-bottom:8px;">MOBILE</div>
          <span class="td-pill">FLUTTER</span>
        </div>
      </td>
      <td width="50%">
        <div class="grid-panel" style="text-align:left;">
          <div class="cyber-label" style="font-size:10px; color:var(--yellow); margin-bottom:8px;">IOT // EMBEDDED</div>
          <span class="td-pill y">ESP32</span>
        </div>
      </td>
    </tr>
    <tr>
      <td width="50%" colspan="2">
        <div class="grid-panel" style="text-align:left;">
          <div class="cyber-label" style="font-size:10px; color:var(--muted); margin-bottom:8px;">DESIGN TOOLS</div>
          <span class="td-pill">FIGMA</span><span class="td-pill">CANVA</span>
        </div>
      </td>
    </tr>
  </table>

</div>

<br/>

<!-- ================= MISSIONS / PROJECTS ================= -->

<div class="cyber-box" style="width:100%; max-width:760px;">

  <div class="cyber-label" style="font-size:11px; color:var(--cyan); margin-bottom:10px; text-align:left;">
    ▚ DIRECTIVES // MISSION LOG
  </div>

  <div style="display:flex; flex-direction:column; gap:10px;">

    <div class="cyber-mission" style="border:1px solid rgba(34,211,238,0.2); border-left:3px solid var(--cyan); border-radius:6px; padding:10px 14px; text-align:left; box-shadow: inset 0 0 18px rgba(34,211,238,0.05);">
      <span class="cyber-mono" style="font-size:11px; color:var(--cyan);">[ACTIVE]</span> <span style="font-size:14px; color:var(--text); font-family:ui-monospace,'SF Mono',monospace;">VEDC PKL MANAGEMENT SYSTEM</span>
      <span class="cyber-mono" style="font-size:11px; color:var(--muted); display:block; margin-top:4px;">> fullstack :: web + db</span>
    </div>

    <div class="cyber-mission" style="border:1px solid rgba(34,211,238,0.2); border-left:3px solid var(--cyan); border-radius:6px; padding:10px 14px; text-align:left; box-shadow: inset 0 0 18px rgba(34,211,238,0.05);">
      <span class="cyber-mono" style="font-size:11px; color:var(--cyan);">[ACTIVE]</span> <span style="font-size:14px; color:var(--text); font-family:ui-monospace,'SF Mono',monospace;">OSIS SYSTEM DEVELOPMENT</span>
      <span class="cyber-mono" style="font-size:11px; color:var(--muted); display:block; margin-top:4px;">> web + org database</span>
    </div>

    <div class="cyber-mission" style="border:1px solid rgba(250,204,21,0.25); border-left:3px solid var(--yellow); border-radius:6px; padding:10px 14px; text-align:left; box-shadow: inset 0 0 18px rgba(250,204,21,0.05);">
      <span class="cyber-mono" style="font-size:11px; color:var(--yellow);">[QUEUED]</span> <span style="font-size:14px; color:var(--text); font-family:ui-monospace,'SF Mono',monospace;">IOT SMART LIGHT PROTOCOL</span>
      <span class="cyber-mono" style="font-size:11px; color:var(--muted); display:block; margin-top:4px;">> esp32 :: embedded</span>
    </div>

  </div>
</div>

<br/>

<!-- ================= FOOTER ================= -->

<div class="cyber-mono" align="center" style="font-size:11px; color:var(--muted);">
<span class="cyan">└─</span> SYSTEM <span class="yellow">STABLE</span> <span class="cyan">//</span> UPTIME<span class="yellow">▸</span>100% <span class="cyan">::</span> rebuild quickly, break nothing <span class="cursor cyan">_</span>
</div>

</div>
