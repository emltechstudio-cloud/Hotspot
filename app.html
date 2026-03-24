<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HotSpot</title>
    <meta name="theme-color" content="#f97316">
    <link rel="manifest" href="manifest.json">
    <link rel="apple-touch-icon" href="apple-touch-icon.png">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
    <style>
        :root {
            --orange: #f97316;
            --yellow: #eab308;
            --bg: #ffffff;
            --surface: #f9fafb;
            --border: #e5e7eb;
            --text: #111827;
            --muted: #6b7280;
            --shadow: 0 1px 6px rgba(0,0,0,.08);
            --shadow-lg: 0 4px 20px rgba(0,0,0,.12);
            --radius: 14px;
        }
        [data-theme="dark"] {
            --bg: #0f0f0f;
            --surface: #1a1a1a;
            --border: #2a2a2a;
            --text: #f3f4f6;
            --muted: #9ca3af;
            --shadow: 0 1px 6px rgba(0,0,0,.4);
            --shadow-lg: 0 4px 20px rgba(0,0,0,.5);
        }
        * { margin:0; padding:0; box-sizing:border-box; -webkit-tap-highlight-color:transparent; }
        body { font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif; background:var(--bg); color:var(--text); min-height:100vh; display:flex; flex-direction:column; transition:background .3s,color .3s; }
        @media(display-mode:standalone){ header { padding-top: max(16px, env(safe-area-inset-top)); } footer { padding-bottom: max(10px, env(safe-area-inset-bottom)); } }

        /* ── Header ── */
        header { padding:16px 20px 12px; border-bottom:1px solid var(--border); background:var(--bg); position:sticky; top:0; z-index:100; display:flex; align-items:center; justify-content:space-between; transition:background .3s,border-color .3s; }
        .logo { display:flex; align-items:center; gap:9px; cursor:pointer; user-select:none; }
        .logo-icon { width:32px; height:32px; background:#111; border-radius:8px; display:flex; align-items:center; justify-content:center; flex-shrink:0; }
        .logo-icon svg { width:22px; height:22px; }
        .logo-text { font-size:20px; font-weight:700; letter-spacing:-.4px; background:linear-gradient(90deg,var(--orange),var(--yellow)); -webkit-background-clip:text; -webkit-text-fill-color:transparent; background-clip:text; }
        .header-right { display:flex; align-items:center; gap:8px; }
        .icon-btn { width:36px; height:36px; border-radius:50%; border:1px solid var(--border); background:var(--surface); color:var(--muted); cursor:pointer; display:flex; align-items:center; justify-content:center; font-size:14px; transition:all .2s; }
        .icon-btn:hover { color:var(--text); border-color:var(--orange); }
        .logout-btn { font-size:13px; font-weight:500; color:var(--muted); background:none; border:none; cursor:pointer; padding:6px 10px; border-radius:8px; transition:all .2s; }
        .logout-btn:hover { color:var(--text); background:var(--surface); }

        /* ── Main ── */
        main { flex:1; overflow-y:auto; }

        /* ── Auth screen ── */
        .auth-screen { display:flex; flex-direction:column; align-items:center; justify-content:center; min-height:85vh; padding:32px 20px; }
        .auth-logo { display:flex; align-items:center; gap:10px; margin-bottom:8px; }
        .auth-logo-icon { width:52px; height:52px; background:#111; border-radius:14px; display:flex; align-items:center; justify-content:center; }
        .auth-logo-icon svg { width:36px; height:36px; }
        .auth-logo-text { font-size:32px; font-weight:800; letter-spacing:-.5px; background:linear-gradient(90deg,var(--orange),var(--yellow)); -webkit-background-clip:text; -webkit-text-fill-color:transparent; background-clip:text; }
        .auth-tagline { color:var(--muted); font-size:14px; margin-bottom:32px; }
        .auth-card { width:100%; max-width:380px; background:var(--surface); border:1px solid var(--border); border-radius:20px; padding:28px; box-shadow:var(--shadow); }
        .auth-tabs { display:flex; margin-bottom:24px; background:var(--bg); border-radius:10px; padding:3px; border:1px solid var(--border); }
        .auth-tab { flex:1; padding:8px; text-align:center; font-size:13px; font-weight:600; color:var(--muted); cursor:pointer; border-radius:8px; transition:all .2s; user-select:none; }
        .auth-tab.active { background:var(--orange); color:white; }
        .auth-form { display:none; }
        .auth-form.active { display:block; }
        .field { margin-bottom:14px; }
        .field label { display:block; font-size:11px; font-weight:700; color:var(--muted); text-transform:uppercase; letter-spacing:.08em; margin-bottom:5px; }
        .field input, .field select { width:100%; background:var(--bg); border:1px solid var(--border); border-radius:10px; padding:11px 13px; font-size:14px; color:var(--text); outline:none; font-family:inherit; transition:border-color .2s,background .3s; }
        .field input:focus, .field select:focus { border-color:var(--orange); }
        .field select option { background:var(--surface); }
        .submit-btn { width:100%; padding:12px; background:var(--orange); color:white; border:none; border-radius:10px; font-size:15px; font-weight:700; cursor:pointer; font-family:inherit; transition:opacity .2s; margin-top:4px; }
        .submit-btn:hover { opacity:.88; }
        .submit-btn:disabled { opacity:.45; cursor:not-allowed; }
        .auth-switch { text-align:center; margin-top:14px; font-size:13px; color:var(--muted); }
        .auth-switch a { color:var(--orange); cursor:pointer; font-weight:500; text-decoration:none; }
        .auth-error { background:rgba(239,68,68,.08); border:1px solid rgba(239,68,68,.2); border-radius:8px; padding:10px 13px; font-size:13px; color:#ef4444; margin-bottom:14px; display:none; }

        /* ── Dashboard ── */
        .dashboard { padding:20px 20px 90px; max-width:640px; margin:0 auto; }
        .dash-greeting { font-size:17px; font-weight:600; margin-bottom:4px; }
        .dash-sub { font-size:13px; color:var(--muted); margin-bottom:24px; }
        .slots-label { font-size:11px; font-weight:700; text-transform:uppercase; letter-spacing:.1em; color:var(--muted); margin-bottom:12px; display:flex; align-items:center; justify-content:space-between; }
        .slots-label span { color:var(--orange); font-size:13px; text-transform:none; letter-spacing:0; font-weight:600; }

        /* ── Site slot ── */
        .slot { border:1px solid var(--border); border-radius:var(--radius); margin-bottom:12px; transition:border-color .2s; }
        .slot.empty { border-style:dashed; background:var(--surface); }
        .slot.empty:hover { border-color:var(--orange); }
        .slot-empty-inner { display:flex; flex-direction:column; align-items:center; justify-content:center; padding:28px; cursor:pointer; gap:8px; }
        .slot-empty-inner i { font-size:22px; color:var(--border); transition:color .2s; }
        .slot.empty:hover .slot-empty-inner i { color:var(--orange); }
        .slot-empty-inner span { font-size:13px; color:var(--muted); font-weight:500; }

        .slot.filled { background:var(--bg); }
        .slot-filled-inner { padding:16px 18px; }
        .slot-top { display:flex; align-items:flex-start; justify-content:space-between; gap:10px; margin-bottom:10px; }
        .slot-name { font-size:16px; font-weight:700; }
        .slot-live { display:inline-flex; align-items:center; gap:5px; font-size:11px; font-weight:600; color:var(--orange); background:rgba(249,115,22,.08); padding:3px 9px; border-radius:20px; }
        .slot-live .dot { width:5px; height:5px; background:var(--orange); border-radius:50%; animation:blink 2s infinite; }
        @keyframes blink { 0%,100%{opacity:1} 50%{opacity:.3} }
        .slot-url { font-size:12px; color:var(--muted); word-break:break-all; margin-bottom:12px; }
        .slot-timer { font-size:12px; color:var(--muted); margin-bottom:14px; display:flex; align-items:center; gap:5px; }
        .slot-timer i { color:var(--yellow); }
        .slot-actions { display:flex; gap:8px; }
        .slot-btn { flex:1; padding:9px; border-radius:8px; font-size:13px; font-weight:600; cursor:pointer; border:1px solid var(--border); background:var(--surface); color:var(--text); font-family:inherit; display:flex; align-items:center; justify-content:center; gap:6px; transition:all .2s; }
        .slot-btn:hover { border-color:var(--orange); color:var(--orange); }
        .slot-btn.danger:hover { border-color:#ef4444; color:#ef4444; }
        .slot-btn.copied { color:var(--orange); border-color:var(--orange); }

        /* ── Upload panel ── */
        .upload-panel { display:none; position:fixed; inset:0; background:rgba(0,0,0,.5); z-index:500; align-items:flex-end; justify-content:center; }
        .upload-panel.open { display:flex; animation:slideUp .3s ease; }
        @keyframes slideUp { from{opacity:0;transform:translateY(30px)} to{opacity:1;transform:translateY(0)} }
        .upload-sheet { background:var(--bg); border-radius:20px 20px 0 0; padding:24px 22px 40px; width:100%; max-width:480px; border-top:1px solid var(--border); }
        .sheet-handle { width:36px; height:4px; background:var(--border); border-radius:2px; margin:0 auto 20px; }
        .upload-sheet h3 { font-size:17px; font-weight:700; margin-bottom:20px; }
        .name-row { display:flex; align-items:center; gap:0; }
        .name-prefix { background:var(--surface); border:1px solid var(--border); border-right:none; border-radius:10px 0 0 10px; padding:11px 10px; font-size:12px; color:var(--muted); white-space:nowrap; line-height:1.4; }
        .name-input { border-radius:0 10px 10px 0!important; flex:1; }
        .name-check { font-size:12px; margin-top:5px; min-height:16px; }
        .name-check.ok { color:var(--orange); }
        .name-check.err { color:#ef4444; }
        .drop-zone { border:2px dashed var(--border); border-radius:12px; padding:28px; text-align:center; cursor:pointer; transition:border-color .2s,background .2s; margin-bottom:14px; }
        .drop-zone:hover, .drop-zone.dragover { border-color:var(--orange); background:rgba(249,115,22,.04); }
        .drop-zone i { font-size:28px; color:var(--border); margin-bottom:8px; display:block; transition:color .2s; }
        .drop-zone:hover i, .drop-zone.dragover i { color:var(--orange); }
        .drop-zone p { font-size:13px; color:var(--muted); }
        .drop-zone .file-name { font-size:13px; font-weight:600; color:var(--orange); margin-top:4px; }
        .duration-pills { display:flex; gap:8px; margin-bottom:16px; }
        .dur-pill { flex:1; padding:10px; border:1px solid var(--border); border-radius:10px; text-align:center; cursor:pointer; font-size:13px; font-weight:600; color:var(--muted); transition:all .2s; user-select:none; }
        .dur-pill.active { border-color:var(--orange); background:rgba(249,115,22,.07); color:var(--orange); }
        .upload-btn { width:100%; padding:13px; background:var(--orange); color:white; border:none; border-radius:10px; font-size:15px; font-weight:700; cursor:pointer; font-family:inherit; transition:opacity .2s; display:flex; align-items:center; justify-content:center; gap:8px; }
        .upload-btn:hover { opacity:.88; }
        .upload-btn:disabled { opacity:.45; cursor:not-allowed; }
        .cancel-btn { width:100%; padding:11px; background:transparent; border:1px solid var(--border); border-radius:10px; font-size:14px; font-weight:500; cursor:pointer; font-family:inherit; color:var(--muted); margin-top:8px; transition:all .2s; }
        .cancel-btn:hover { border-color:var(--text); color:var(--text); }

        /* ── Footer ── */
        footer { display:flex; justify-content:space-around; padding:10px 0; border-top:1px solid var(--border); background:var(--bg); position:sticky; bottom:0; z-index:99; transition:background .3s,border-color .3s; }
        .footer-btn { color:var(--muted); background:none; border:none; padding:7px 20px; cursor:pointer; font-size:11px; display:flex; flex-direction:column; align-items:center; gap:3px; border-radius:8px; transition:color .2s; }
        .footer-btn i { font-size:20px; }
        .footer-btn:hover, .footer-btn.active { color:var(--orange); }

        /* ── Toast ── */
        .toast { position:fixed; bottom:74px; left:50%; transform:translateX(-50%); background:var(--text); color:var(--bg); padding:10px 18px; border-radius:8px; font-size:13px; z-index:4000; white-space:nowrap; pointer-events:none; box-shadow:0 4px 16px rgba(0,0,0,.2); animation:fadeIn .2s ease; }
        @keyframes fadeIn { from{opacity:0} to{opacity:1} }

        /* ── Loading spinner ── */
        .spinner { width:18px; height:18px; border:2px solid rgba(255,255,255,.35); border-top-color:white; border-radius:50%; animation:spin 1s linear infinite; }
        @keyframes spin { to{transform:rotate(360deg)} }

        @media(max-width:480px){ .auth-card{padding:22px 18px} .upload-sheet{padding:20px 18px 36px} }
    </style>
</head>
<body>

<!-- Header -->
<header id="appHeader" style="display:none">
    <div class="logo" id="logoBtn">
        <div class="logo-icon">
            <svg viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect x="1" y="11" width="16" height="14" rx="7" fill="none" stroke="#f97316" stroke-width="3"/>
                <rect x="19" y="11" width="16" height="14" rx="7" fill="none" stroke="#eab308" stroke-width="3"/>
                <rect x="16" y="13" width="4" height="10" fill="#111"/>
                <circle cx="18" cy="18" r="2" fill="#f97316"/>
            </svg>
        </div>
        <span class="logo-text">HotSpot</span>
    </div>
    <div class="header-right">
        <button class="icon-btn" id="themeBtn" title="Toggle theme"><i class="fas fa-moon" id="themeIcon"></i></button>
        <button class="logout-btn" id="logoutBtn"><i class="fas fa-sign-out-alt"></i></button>
    </div>
</header>

<!-- Main -->
<main>

    <!-- Auth Screen -->
    <div id="authScreen" class="auth-screen">
        <div class="auth-logo">
            <div class="auth-logo-icon">
                <svg viewBox="0 0 36 36" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect x="1" y="11" width="16" height="14" rx="7" fill="none" stroke="#f97316" stroke-width="3"/>
                    <rect x="19" y="11" width="16" height="14" rx="7" fill="none" stroke="#eab308" stroke-width="3"/>
                    <rect x="16" y="13" width="4" height="10" fill="#111"/>
                    <circle cx="18" cy="18" r="2" fill="#f97316"/>
                </svg>
            </div>
            <span class="auth-logo-text">HotSpot</span>
        </div>
        <p class="auth-tagline">Deploy instantly. Share the link. Done.</p>

        <div class="auth-card">
            <div class="auth-tabs">
                <div class="auth-tab active" id="tabLogin" onclick="showAuthTab('login')">Sign In</div>
                <div class="auth-tab" id="tabRegister" onclick="showAuthTab('register')">Sign Up</div>
                <div class="auth-tab" id="tabRecover" onclick="showAuthTab('recover')" style="display:none">Recover</div>
            </div>

            <!-- Login -->
            <div class="auth-form active" id="formLogin">
                <div class="auth-error" id="loginError"></div>
                <div class="field"><label>Email</label><input type="email" id="loginEmail" placeholder="you@example.com" autocomplete="email"></div>
                <div class="field"><label>Password</label><input type="password" id="loginPassword" placeholder="Your password" autocomplete="current-password"></div>
                <button class="submit-btn" id="loginBtn">Sign In</button>
                <div class="auth-switch">Forgot password? <a onclick="showAuthTab('recover')">Recover account</a></div>
            </div>

            <!-- Register -->
            <div class="auth-form" id="formRegister">
                <div class="auth-error" id="registerError"></div>
                <div class="field"><label>Email</label><input type="email" id="regEmail" placeholder="you@example.com" autocomplete="email"></div>
                <div class="field"><label>Password</label><input type="password" id="regPassword" placeholder="At least 6 characters" autocomplete="new-password"></div>
                <div class="field"><label>Security Question</label>
                    <select id="regQuestion">
                        <option value="">Choose a question...</option>
                        <option>What city were you born in?</option>
                        <option>What is your mother's maiden name?</option>
                        <option>What was the name of your first pet?</option>
                        <option>What was the name of your primary school?</option>
                        <option>What is your favourite food?</option>
                        <option>What street did you grow up on?</option>
                    </select>
                </div>
                <div class="field"><label>Answer</label><input type="text" id="regAnswer" placeholder="Your answer (remember this)"></div>
                <button class="submit-btn" id="registerBtn">Create Account</button>
                <div class="auth-switch">Already have an account? <a onclick="showAuthTab('login')">Sign in</a></div>
            </div>

            <!-- Recover -->
            <div class="auth-form" id="formRecover">
                <div class="auth-error" id="recoverError"></div>
                <div class="field"><label>Email</label><input type="email" id="recEmail" placeholder="you@example.com"></div>
                <div id="recQuestionWrap" style="display:none">
                    <div class="field"><label>Security Question</label><p id="recQuestion" style="font-size:14px;padding:10px 0;color:var(--text)"></p></div>
                    <div class="field"><label>Your Answer</label><input type="text" id="recAnswer" placeholder="Your answer"></div>
                    <div class="field"><label>New Password</label><input type="password" id="recPassword" placeholder="New password"></div>
                </div>
                <button class="submit-btn" id="recoverBtn">Continue</button>
                <div class="auth-switch"><a onclick="showAuthTab('login')">← Back to sign in</a></div>
            </div>
        </div>
    </div>

    <!-- Dashboard -->
    <div id="dashboard" class="dashboard" style="display:none">
        <p class="dash-greeting" id="dashGreeting">Your sites</p>
        <p class="dash-sub">Up to 3 active sites on the free plan</p>
        <div class="slots-label">
            Active Sites <span id="slotsCount">0 / 3</span>
        </div>
        <div id="siteSlots"></div>
    </div>

</main>

<!-- Upload Panel -->
<div class="upload-panel" id="uploadPanel">
    <div class="upload-sheet">
        <div class="sheet-handle"></div>
        <h3>Deploy a New Site</h3>

        <div class="field">
            <label>Site Name</label>
            <div class="name-row">
                <span class="name-prefix">hotspot.afric.site/s/</span>
                <input type="text" class="field input name-input" id="siteNameInput" placeholder="my-project" autocomplete="off" spellcheck="false">
            </div>
            <div class="name-check" id="nameCheck"></div>
        </div>

        <div class="field">
            <label>Duration</label>
            <div class="duration-pills">
                <div class="dur-pill active" data-h="24">24h</div>
                <div class="dur-pill" data-h="48">48h</div>
                <div class="dur-pill" data-h="72">72h</div>
            </div>
        </div>

        <div class="field">
            <label>HTML File</label>
            <div class="drop-zone" id="dropZone">
                <i class="fas fa-cloud-upload-alt"></i>
                <p>Tap to choose or drop your HTML file</p>
                <div class="file-name" id="fileName"></div>
            </div>
            <input type="file" id="fileInput" accept=".html" style="display:none">
        </div>

        <button class="upload-btn" id="deployBtn" disabled>
            <i class="fas fa-bolt"></i> Deploy Site
        </button>
        <button class="cancel-btn" id="cancelUpload">Cancel</button>
    </div>
</div>

<!-- Footer -->
<footer id="appFooter" style="display:none">
    <button class="footer-btn active" id="homeFooterBtn"><i class="fas fa-home"></i><span>Home</span></button>
    <button class="footer-btn" id="addSiteBtn"><i class="fas fa-plus-circle"></i><span>Deploy</span></button>
    <button class="footer-btn" id="installFooterBtn"><i class="fas fa-download"></i><span>Install</span></button>
</footer>

<script>
'use strict';

const API = 'https://emltechstudio-hotspot.hf.space';

// ── Service Worker ───────────────────────────────────────────────────
if ('serviceWorker' in navigator) {
    navigator.serviceWorker.register('./sw.js').catch(() => {});
}

// ── State ────────────────────────────────────────────────────────────
let token = localStorage.getItem('hs-token') || '';
let email = localStorage.getItem('hs-email') || '';
let sites = [];
let selectedDuration = 24;
let selectedFile = null;
let nameCheckTimer = null;
let recoverStep = 1;

// ── DOM ──────────────────────────────────────────────────────────────
const el = id => document.getElementById(id);
const D = {
    authScreen: el('authScreen'),
    dashboard: el('dashboard'),
    appHeader: el('appHeader'),
    appFooter: el('appFooter'),
    themeBtn: el('themeBtn'),
    themeIcon: el('themeIcon'),
    logoutBtn: el('logoutBtn'),
    logoBtn: el('logoBtn'),
    dashGreeting: el('dashGreeting'),
    slotsCount: el('slotsCount'),
    siteSlots: el('siteSlots'),
    uploadPanel: el('uploadPanel'),
    siteNameInput: el('siteNameInput'),
    nameCheck: el('nameCheck'),
    dropZone: el('dropZone'),
    fileInput: el('fileInput'),
    fileName: el('fileName'),
    deployBtn: el('deployBtn'),
    cancelUpload: el('cancelUpload'),
    addSiteBtn: el('addSiteBtn'),
    installFooterBtn: el('installFooterBtn'),
    loginEmail: el('loginEmail'),
    loginPassword: el('loginPassword'),
    loginBtn: el('loginBtn'),
    loginError: el('loginError'),
    regEmail: el('regEmail'),
    regPassword: el('regPassword'),
    regQuestion: el('regQuestion'),
    regAnswer: el('regAnswer'),
    registerBtn: el('registerBtn'),
    registerError: el('registerError'),
    recEmail: el('recEmail'),
    recAnswer: el('recAnswer'),
    recPassword: el('recPassword'),
    recoverBtn: el('recoverBtn'),
    recoverError: el('recoverError'),
    recQuestion: el('recQuestion'),
    recQuestionWrap: el('recQuestionWrap')
};

// ── Boot ─────────────────────────────────────────────────────────────
document.addEventListener('DOMContentLoaded', () => {
    applyTheme(localStorage.getItem('hs-theme') === 'dark');
    if (token && email) {
        showDashboard();
        loadSites();
    } else {
        showAuth();
    }
    bindEvents();
});

function bindEvents() {
    D.themeBtn.addEventListener('click', () => applyTheme(document.body.getAttribute('data-theme') !== 'dark'));
    D.logoutBtn.addEventListener('click', logout);
    D.logoBtn.addEventListener('click', () => { if (token) loadSites(); });
    D.loginBtn.addEventListener('click', doLogin);
    D.registerBtn.addEventListener('click', doRegister);
    D.recoverBtn.addEventListener('click', doRecover);
    D.addSiteBtn.addEventListener('click', openUpload);
    D.cancelUpload.addEventListener('click', closeUpload);
    D.deployBtn.addEventListener('click', doDeploy);
    D.installFooterBtn.addEventListener('click', () => location.href = 'install.html');

    // Enter key on auth inputs
    [D.loginEmail, D.loginPassword].forEach(i => i.addEventListener('keydown', e => { if (e.key==='Enter') doLogin(); }));
    [D.regEmail, D.regPassword, D.regAnswer].forEach(i => i.addEventListener('keydown', e => { if (e.key==='Enter') doRegister(); }));

    // Site name check
    D.siteNameInput.addEventListener('input', () => {
        clearTimeout(nameCheckTimer);
        const v = D.siteNameInput.value.trim();
        D.nameCheck.textContent = '';
        D.nameCheck.className = 'name-check';
        validateDeploy();
        if (v.length >= 3) {
            nameCheckTimer = setTimeout(() => checkName(v), 600);
        }
    });

    // Duration pills
    document.querySelectorAll('.dur-pill').forEach(p => {
        p.addEventListener('click', () => {
            document.querySelectorAll('.dur-pill').forEach(x => x.classList.remove('active'));
            p.classList.add('active');
            selectedDuration = +p.dataset.h;
        });
    });

    // File drop zone
    D.dropZone.addEventListener('click', () => D.fileInput.click());
    D.fileInput.addEventListener('change', e => {
        const f = e.target.files[0];
        if (f) handleFile(f);
    });
    D.dropZone.addEventListener('dragover', e => { e.preventDefault(); D.dropZone.classList.add('dragover'); });
    D.dropZone.addEventListener('dragleave', () => D.dropZone.classList.remove('dragover'));
    D.dropZone.addEventListener('drop', e => {
        e.preventDefault();
        D.dropZone.classList.remove('dragover');
        const f = e.dataTransfer.files[0];
        if (f) handleFile(f);
    });

    // Close upload on backdrop click
    D.uploadPanel.addEventListener('click', e => {
        if (e.target === D.uploadPanel) closeUpload();
    });
}

// ── Theme ────────────────────────────────────────────────────────────
function applyTheme(dark) {
    if (dark) {
        document.body.setAttribute('data-theme','dark');
        D.themeIcon.className = 'fas fa-sun';
    } else {
        document.body.removeAttribute('data-theme');
        D.themeIcon.className = 'fas fa-moon';
    }
    localStorage.setItem('hs-theme', dark ? 'dark' : 'light');
}

// ── Auth views ────────────────────────────────────────────────────────
function showAuth() {
    D.authScreen.style.display = 'flex';
    D.dashboard.style.display = 'none';
    D.appHeader.style.display = 'none';
    D.appFooter.style.display = 'none';
}

function showDashboard() {
    D.authScreen.style.display = 'none';
    D.dashboard.style.display = 'block';
    D.appHeader.style.display = 'flex';
    D.appFooter.style.display = 'flex';
    const name = email.split('@')[0];
    D.dashGreeting.textContent = `Hey, ${name} 👋`;
}

function showAuthTab(tab) {
    ['login','register','recover'].forEach(t => {
        el('tab' + t.charAt(0).toUpperCase() + t.slice(1)).classList.toggle('active', t === tab);
        el('form' + t.charAt(0).toUpperCase() + t.slice(1)).classList.toggle('active', t === tab);
    });
    el('tabRecover').style.display = tab === 'recover' ? 'flex' : 'none';
    recoverStep = 1;
    D.recQuestionWrap.style.display = 'none';
    D.recoverBtn.textContent = 'Continue';
}

// ── Auth actions ──────────────────────────────────────────────────────
async function doLogin() {
    const em = D.loginEmail.value.trim();
    const pw = D.loginPassword.value;
    if (!em || !pw) { showErr('loginError','Please fill all fields'); return; }
    setLoading(D.loginBtn, true);
    try {
        const r = await api('POST', '/api/login', { email: em, password: pw });
        saveSession(r.token, r.email);
        showDashboard();
        loadSites();
    } catch(e) {
        showErr('loginError', e.message);
    } finally {
        setLoading(D.loginBtn, false);
    }
}

async function doRegister() {
    const em = D.regEmail.value.trim();
    const pw = D.regPassword.value;
    const q = D.regQuestion.value;
    const a = D.regAnswer.value.trim();
    if (!em || !pw || !q || !a) { showErr('registerError','Please fill all fields'); return; }
    setLoading(D.registerBtn, true);
    try {
        const r = await api('POST', '/api/register', {
            email: em, password: pw,
            security_question: q, security_answer: a
        });
        saveSession(r.token, r.email);
        showDashboard();
        loadSites();
    } catch(e) {
        showErr('registerError', e.message);
    } finally {
        setLoading(D.registerBtn, false);
    }
}

async function doRecover() {
    if (recoverStep === 1) {
        const em = D.recEmail.value.trim();
        if (!em) { showErr('recoverError','Enter your email'); return; }
        setLoading(D.recoverBtn, true);
        try {
            const r = await api('GET', `/api/security-question?email=${encodeURIComponent(em)}`);
            D.recQuestion.textContent = r.question;
            D.recQuestionWrap.style.display = 'block';
            D.recoverBtn.textContent = 'Reset Password';
            recoverStep = 2;
            hideErr('recoverError');
        } catch(e) {
            showErr('recoverError', e.message);
        } finally {
            setLoading(D.recoverBtn, false);
        }
    } else {
        const em = D.recEmail.value.trim();
        const ans = D.recAnswer.value.trim();
        const pw = D.recPassword.value;
        if (!ans || !pw) { showErr('recoverError','Fill all fields'); return; }
        setLoading(D.recoverBtn, true);
        try {
            const r = await api('POST', '/api/recover', {
                email: em, security_answer: ans, new_password: pw
            });
            saveSession(r.token, r.email);
            showDashboard();
            loadSites();
        } catch(e) {
            showErr('recoverError', e.message);
        } finally {
            setLoading(D.recoverBtn, false);
        }
    }
}

function saveSession(t, em) {
    token = t;
    email = em;
    localStorage.setItem('hs-token', t);
    localStorage.setItem('hs-email', em);
}

function logout() {
    token = ''; email = ''; sites = [];
    localStorage.removeItem('hs-token');
    localStorage.removeItem('hs-email');
    showAuth();
}

// ── Dashboard ─────────────────────────────────────────────────────────
async function loadSites() {
    try {
        const r = await api('GET', '/api/sites');
        sites = r.sites || [];
        renderSlots();
    } catch(e) {
        toast('Failed to load sites');
    }
}

function renderSlots() {
    const MAX = 3;
    D.slotsCount.textContent = `${sites.length} / ${MAX}`;
    D.siteSlots.innerHTML = '';

    // Filled slots
    sites.forEach(site => {
        const div = document.createElement('div');
        div.className = 'slot filled';
        const expiresAt = new Date(site.expires_at);
        div.innerHTML = `
            <div class="slot-filled-inner">
                <div class="slot-top">
                    <span class="slot-name">${escHtml(site.sitename)}</span>
                    <span class="slot-live"><span class="dot"></span> LIVE</span>
                </div>
                <div class="slot-url">${escHtml(site.url)}</div>
                <div class="slot-timer" id="timer-${site.sitename}">
                    <i class="fas fa-clock"></i>
                    <span>Calculating...</span>
                </div>
                <div class="slot-actions">
                    <button class="slot-btn" onclick="copyLink('${escHtml(site.url)}', this)">
                        <i class="fas fa-copy"></i> Copy Link
                    </button>
                    <button class="slot-btn danger" onclick="deleteSite('${escHtml(site.sitename)}')">
                        <i class="fas fa-trash"></i> Delete
                    </button>
                </div>
            </div>
        `;
        D.siteSlots.appendChild(div);
        startTimer(site.sitename, expiresAt);
    });

    // Empty slots
    const empty = MAX - sites.length;
    for (let i = 0; i < empty; i++) {
        const div = document.createElement('div');
        div.className = 'slot empty';
        div.innerHTML = `
            <div class="slot-empty-inner" onclick="openUpload()">
                <i class="fas fa-plus"></i>
                <span>Deploy a site</span>
            </div>
        `;
        D.siteSlots.appendChild(div);
    }
}

function startTimer(sitename, expiresAt) {
    function update() {
        const el = document.getElementById(`timer-${sitename}`);
        if (!el) return;
        const diff = expiresAt - new Date();
        if (diff <= 0) {
            el.innerHTML = '<i class="fas fa-clock"></i><span>Expired — refresh</span>';
            loadSites();
            return;
        }
        const h = Math.floor(diff / 3600000);
        const m = Math.floor((diff % 3600000) / 60000);
        const s = Math.floor((diff % 60000) / 1000);
        el.innerHTML = `<i class="fas fa-clock"></i><span>${h}h ${m}m ${s}s remaining</span>`;
        setTimeout(update, 1000);
    }
    update();
}

function copyLink(url, btn) {
    navigator.clipboard.writeText(url).then(() => {
        btn.classList.add('copied');
        btn.innerHTML = '<i class="fas fa-check"></i> Copied!';
        setTimeout(() => {
            btn.classList.remove('copied');
            btn.innerHTML = '<i class="fas fa-copy"></i> Copy Link';
        }, 2000);
    });
}

async function deleteSite(sitename) {
    if (!confirm(`Delete "${sitename}"? This cannot be undone.`)) return;
    try {
        await api('DELETE', `/api/site/${sitename}`);
        toast('Site deleted');
        loadSites();
    } catch(e) {
        toast(e.message);
    }
}

// ── Upload ────────────────────────────────────────────────────────────
function openUpload() {
    if (sites.length >= 3) { toast('Free tier limit: 3 active sites. Delete one first.'); return; }
    D.uploadPanel.classList.add('open');
    D.siteNameInput.value = '';
    D.nameCheck.textContent = '';
    D.fileName.textContent = '';
    selectedFile = null;
    D.deployBtn.disabled = true;
    document.querySelectorAll('.dur-pill').forEach((p,i) => p.classList.toggle('active', i===0));
    selectedDuration = 24;
}

function closeUpload() {
    D.uploadPanel.classList.remove('open');
}

function handleFile(f) {
    if (!f.name.endsWith('.html')) { toast('Only .html files allowed'); return; }
    if (f.size > 5 * 1024 * 1024) { toast('File too large (max 5MB)'); return; }
    selectedFile = f;
    D.fileName.textContent = f.name;
    validateDeploy();
}

async function checkName(name) {
    try {
        const r = await api('GET', `/api/check/${encodeURIComponent(name)}`);
        D.nameCheck.textContent = r.available ? '✓ Available' : `✗ ${r.reason}`;
        D.nameCheck.className = 'name-check ' + (r.available ? 'ok' : 'err');
        validateDeploy();
    } catch {}
}

function validateDeploy() {
    const name = D.siteNameInput.value.trim();
    const nameOk = D.nameCheck.classList.contains('ok');
    D.deployBtn.disabled = !(name.length >= 3 && nameOk && selectedFile);
}

async function doDeploy() {
    const name = D.siteNameInput.value.trim();
    if (!name || !selectedFile) return;
    D.deployBtn.disabled = true;
    D.deployBtn.innerHTML = '<div class="spinner"></div> Deploying...';
    try {
        const form = new FormData();
        form.append('file', selectedFile);
        form.append('sitename', name);
        form.append('duration', selectedDuration);
        const r = await apiForm('/api/upload', form);
        closeUpload();
        toast('🔥 Site is live!');
        loadSites();
    } catch(e) {
        toast(e.message);
        D.deployBtn.disabled = false;
        D.deployBtn.innerHTML = '<i class="fas fa-bolt"></i> Deploy Site';
    }
}

// ── API helpers ───────────────────────────────────────────────────────
async function api(method, path, body) {
    const opts = {
        method,
        headers: { 'Content-Type': 'application/json' }
    };
    if (token) opts.headers['Authorization'] = `Bearer ${token}`;
    if (body && method !== 'GET') opts.body = JSON.stringify(body);
    const r = await fetch(API + path, opts);
    const data = await r.json();
    if (!r.ok) throw new Error(data.detail || 'Something went wrong');
    return data;
}

async function apiForm(path, form) {
    const r = await fetch(API + path, {
        method: 'POST',
        headers: { 'Authorization': `Bearer ${token}` },
        body: form
    });
    const data = await r.json();
    if (!r.ok) throw new Error(data.detail || 'Something went wrong');
    return data;
}

// ── Utilities ─────────────────────────────────────────────────────────
function showErr(id, msg) {
    const el = document.getElementById(id);
    el.textContent = msg;
    el.style.display = 'block';
}
function hideErr(id) { document.getElementById(id).style.display = 'none'; }
function setLoading(btn, loading) {
    btn.disabled = loading;
    if (loading) { btn._txt = btn.textContent; btn.innerHTML = '<div class="spinner"></div>'; }
    else { btn.disabled = false; btn.innerHTML = btn._txt || btn.textContent; }
}
function toast(msg) {
    document.querySelectorAll('.toast').forEach(t => t.remove());
    const t = document.createElement('div');
    t.className = 'toast';
    t.textContent = msg;
    document.body.appendChild(t);
    setTimeout(() => { t.style.opacity='0'; t.style.transition='opacity .3s'; setTimeout(() => t.remove(), 300); }, 2800);
}
function escHtml(s) {
    return String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/"/g,'&quot;');
}
</script>
</body>
</html>
