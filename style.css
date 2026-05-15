/* ─────────────────────────────────────────
   RESET & ROOT VARIABLES
───────────────────────────────────────── */
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

:root {
  --bg:        #0a0a14;
  --bg2:       #0f0f20;
  --bg3:       #13132a;
  --card:      rgba(255,255,255,0.04);
  --card-border: rgba(255,255,255,0.10);
  --text:      #e8e8f0;
  --muted:     #8888aa;
  --accent1:   #7c3aed;
  --accent2:   #06b6d4;
  --accent3:   #a855f7;
  --grad:      linear-gradient(135deg, #7c3aed, #06b6d4);
  --grad2:     linear-gradient(135deg, #a855f7, #3b82f6);
  --radius:    16px;
  --transition: 0.35s cubic-bezier(.4,0,.2,1);
}

html { scroll-behavior: smooth; }

body {
  font-family: 'Inter', sans-serif;
  background: var(--bg);
  color: var(--text);
  overflow-x: hidden;
  line-height: 1.65;
}

/* ─────────────────────────────────────────
   UTILITIES
───────────────────────────────────────── */
.container {
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 24px;
}

.gradient-text {
  background: var(--grad);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.card-glass {
  background: var(--card);
  border: 1px solid var(--card-border);
  backdrop-filter: blur(16px);
  -webkit-backdrop-filter: blur(16px);
  border-radius: var(--radius);
  transition: transform var(--transition), box-shadow var(--transition), border-color var(--transition);
}
.card-glass:hover {
  transform: translateY(-6px);
  box-shadow: 0 20px 60px rgba(124,58,237,0.2);
  border-color: rgba(124,58,237,0.4);
}

/* Reveal animation */
.reveal { opacity: 0; transform: translateY(30px); transition: opacity 0.7s ease, transform 0.7s ease; }
.reveal.visible { opacity: 1; transform: translateY(0); }

/* ─────────────────────────────────────────
   NAVBAR
───────────────────────────────────────── */
#navbar {
  position: fixed; top: 0; left: 0; width: 100%;
  z-index: 1000;
  transition: background var(--transition), box-shadow var(--transition);
  padding: 0 24px;
}
#navbar.scrolled {
  background: rgba(10,10,20,0.85);
  backdrop-filter: blur(20px);
  box-shadow: 0 2px 40px rgba(0,0,0,0.5);
}
.nav-inner {
  max-width: 1100px; margin: 0 auto;
  display: flex; align-items: center; justify-content: space-between;
  height: 68px;
}
.nav-logo {
  font-family: 'Outfit', sans-serif;
  font-size: 1.6rem; font-weight: 800;
  background: var(--grad);
  -webkit-background-clip: text; -webkit-text-fill-color: transparent;
  background-clip: text;
}
.dot { color: var(--accent2); -webkit-text-fill-color: var(--accent2); }
.nav-links { list-style: none; display: flex; gap: 32px; }
.nav-links a {
  color: var(--muted); text-decoration: none;
  font-size: 0.9rem; font-weight: 500;
  transition: color var(--transition);
}
.nav-links a:hover { color: var(--text); }
.nav-cta {
  background: var(--grad); color: #fff; border: none;
  padding: 10px 22px; border-radius: 50px;
  font-size: 0.85rem; font-weight: 600; cursor: pointer;
  transition: opacity var(--transition), transform var(--transition);
}
.nav-cta:hover { opacity: 0.85; transform: scale(1.04); }
.hamburger { display: none; background: none; border: none; color: var(--text); font-size: 1.5rem; cursor: pointer; }
.mobile-links { display: none; flex-direction: column; background: rgba(10,10,20,0.97); list-style: none; padding: 12px 24px 20px; gap: 12px; }
.mobile-links.open { display: flex; }
.mobile-links a { color: var(--text); text-decoration: none; font-size: 1rem; font-weight: 500; padding: 6px 0; }

/* ─────────────────────────────────────────
   HERO
───────────────────────────────────────── */
#hero {
  min-height: 100vh;
  display: flex; align-items: center;
  position: relative; overflow: hidden;
  padding-top: 68px;
}
.hero-bg {
  position: absolute; inset: 0;
  background: radial-gradient(ellipse 80% 60% at 20% 60%, rgba(124,58,237,0.18) 0%, transparent 60%),
              radial-gradient(ellipse 60% 50% at 80% 30%, rgba(6,182,212,0.14) 0%, transparent 60%),
              var(--bg);
}
.hero-content {
  position: relative; z-index: 2;
  max-width: 600px;
  padding: 80px 24px 80px 10%;
}
.badge {
  display: inline-block;
  background: rgba(124,58,237,0.15);
  border: 1px solid rgba(124,58,237,0.35);
  color: #c4b5fd;
  font-size: 0.78rem; font-weight: 600; letter-spacing: 0.08em;
  padding: 6px 16px; border-radius: 50px; margin-bottom: 20px;
  text-transform: uppercase;
}
.hero-title {
  font-family: 'Outfit', sans-serif;
  font-size: clamp(2.8rem, 6vw, 5rem);
  font-weight: 800; line-height: 1.1; margin-bottom: 20px;
}
.hero-sub {
  font-size: 1.15rem; color: var(--muted); margin-bottom: 36px; max-width: 480px;
}
.hero-actions { display: flex; gap: 16px; flex-wrap: wrap; margin-bottom: 48px; }
.btn-primary {
  background: var(--grad); color: #fff; text-decoration: none;
  padding: 14px 30px; border-radius: 50px;
  font-weight: 700; font-size: 0.95rem;
  transition: opacity var(--transition), transform var(--transition);
  box-shadow: 0 8px 32px rgba(124,58,237,0.35);
}
.btn-primary:hover { opacity: 0.85; transform: translateY(-2px); }
.btn-outline {
  border: 1.5px solid rgba(255,255,255,0.2); color: var(--text); text-decoration: none;
  padding: 14px 30px; border-radius: 50px;
  font-weight: 600; font-size: 0.95rem;
  transition: border-color var(--transition), background var(--transition);
  backdrop-filter: blur(8px);
}
.btn-outline:hover { border-color: var(--accent1); background: rgba(124,58,237,0.1); }

.hero-scroll { display: flex; justify-content: flex-start; }
.hero-scroll span {
  display: block; width: 2px; height: 48px;
  background: linear-gradient(to bottom, rgba(255,255,255,0.3), transparent);
  border-radius: 2px; animation: scrollPulse 2s ease-in-out infinite;
}
@keyframes scrollPulse { 0%,100%{opacity:1;transform:scaleY(1)} 50%{opacity:0.4;transform:scaleY(0.6)} }

/* Floating orbs */
.hero-visual { position: absolute; right: 0; top: 0; width: 50%; height: 100%; pointer-events: none; }
.orb {
  position: absolute; border-radius: 50%;
  filter: blur(60px); opacity: 0.35; animation: float 6s ease-in-out infinite;
}
.orb1 { width: 350px; height: 350px; background: var(--accent1); top: 15%; right: 5%; animation-delay: 0s; }
.orb2 { width: 250px; height: 250px; background: var(--accent2); bottom: 20%; right: 25%; animation-delay: 2s; }
.orb3 { width: 180px; height: 180px; background: var(--accent3); top: 55%; right: 8%; animation-delay: 4s; }
@keyframes float { 0%,100%{transform:translateY(0)} 50%{transform:translateY(-20px)} }

.floating-card {
  position: absolute; background: rgba(255,255,255,0.07);
  border: 1px solid rgba(255,255,255,0.12);
  backdrop-filter: blur(12px); border-radius: 12px;
  padding: 10px 18px; display: flex; align-items: center; gap: 8px;
  font-size: 0.85rem; font-weight: 600; color: var(--text);
  animation: float 5s ease-in-out infinite;
  box-shadow: 0 8px 32px rgba(0,0,0,0.3);
}
.card-icon { font-size: 1.1rem; }
.card1 { top: 25%; right: 15%; animation-delay: 0.5s; }
.card2 { top: 48%; right: 35%; animation-delay: 2s; }
.card3 { top: 65%; right: 12%; animation-delay: 3.5s; }

/* Hero animations */
@keyframes fadeIn { from{opacity:0} to{opacity:1} }
@keyframes slideUp { from{opacity:0;transform:translateY(30px)} to{opacity:1;transform:translateY(0)} }
.animate-fade { animation: fadeIn 0.8s ease forwards; }
.animate-slide { animation: slideUp 0.8s ease forwards; }
.delay-1 { animation-delay: 0.2s; }
.delay-2 { animation-delay: 0.4s; }
.delay-3 { animation-delay: 0.6s; }

/* ─────────────────────────────────────────
   SECTION COMMONS
───────────────────────────────────────── */
section { padding: 100px 0; }
section:nth-child(even) { background: var(--bg2); }

.section-header {
  text-align: center; margin-bottom: 60px;
}
.section-tag {
  display: inline-block;
  font-size: 0.72rem; font-weight: 700; letter-spacing: 0.12em;
  text-transform: uppercase; color: var(--accent2);
  background: rgba(6,182,212,0.1); border: 1px solid rgba(6,182,212,0.25);
  padding: 4px 14px; border-radius: 50px; margin-bottom: 14px;
}
.section-header h2 {
  font-family: 'Outfit', sans-serif;
  font-size: clamp(1.8rem, 4vw, 2.8rem); font-weight: 800;
  background: var(--grad2); -webkit-background-clip: text;
  -webkit-text-fill-color: transparent; background-clip: text;
}
.section-desc { color: var(--muted); margin-top: 10px; font-size: 1rem; }

/* ─────────────────────────────────────────
   SOBRE
───────────────────────────────────────── */
.sobre-grid {
  display: grid; grid-template-columns: 220px 1fr; gap: 60px; align-items: center;
}
.sobre-avatar { display: flex; flex-direction: column; align-items: center; gap: 16px; }
.avatar-ring {
  width: 180px; height: 180px; border-radius: 50%;
  background: var(--grad); padding: 3px;
  animation: float 6s ease-in-out infinite;
}
.avatar-photo {
  width: 100%; height: 100%; border-radius: 50%;
  object-fit: cover; object-position: center top;
  display: block;
}
.avatar-badge {
  background: rgba(6,182,212,0.1); border: 1px solid rgba(6,182,212,0.3);
  color: var(--accent2); padding: 6px 18px; border-radius: 50px;
  font-size: 0.82rem; font-weight: 600;
}
.sobre-texto h3 { font-size: 1.6rem; font-weight: 700; margin-bottom: 16px; }
.sobre-texto p { color: var(--muted); margin-bottom: 14px; line-height: 1.75; }
.sobre-links { display: flex; flex-wrap: wrap; gap: 12px; margin-top: 20px; }
.chip {
  display: inline-flex; align-items: center; gap: 6px;
  background: rgba(255,255,255,0.06); border: 1px solid rgba(255,255,255,0.12);
  color: var(--text); text-decoration: none;
  padding: 8px 18px; border-radius: 50px; font-size: 0.85rem; font-weight: 500;
  transition: background var(--transition), border-color var(--transition);
}
.chip:hover { background: rgba(124,58,237,0.15); border-color: var(--accent1); }

/* ─────────────────────────────────────────
   IDIOMAS
───────────────────────────────────────── */
.idiomas-grid {
  display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 24px;
}
.idioma-card { padding: 36px 28px; text-align: center; }
.flag { font-size: 3rem; margin-bottom: 14px; }
.idioma-card h3 { font-size: 1.2rem; font-weight: 700; margin-bottom: 8px; }
.nivel-badge {
  display: inline-block; padding: 4px 14px; border-radius: 50px;
  font-size: 0.75rem; font-weight: 700; letter-spacing: 0.06em;
  background: rgba(124,58,237,0.2); color: #c4b5fd;
  border: 1px solid rgba(124,58,237,0.3); margin-bottom: 12px;
}
.nivel-b1 { background: rgba(6,182,212,0.15); color: var(--accent2); border-color: rgba(6,182,212,0.3); }
.nivel-cert { background: rgba(234,179,8,0.15); color: #fbbf24; border-color: rgba(234,179,8,0.3); }
.idioma-card p, .idioma-card ul { color: var(--muted); font-size: 0.9rem; }
.cert-card ul { list-style: none; display: flex; flex-direction: column; gap: 4px; }

/* ─────────────────────────────────────────
   SKILLS
───────────────────────────────────────── */
.skills-wrapper {
  display: grid; grid-template-columns: 1fr 1px 1fr; gap: 48px; align-items: start;
}
.skills-divider { background: rgba(255,255,255,0.08); }
.skills-subtitle {
  font-family: 'Outfit', sans-serif; font-size: 1.15rem; font-weight: 700;
  margin-bottom: 28px; color: var(--text);
}
.skill-item {
  display: flex; gap: 16px; margin-bottom: 24px;
  padding: 18px; border-radius: 12px;
  background: var(--card); border: 1px solid var(--card-border);
  transition: transform var(--transition), border-color var(--transition);
}
.skill-item:hover { transform: translateX(6px); border-color: rgba(124,58,237,0.4); }
.skill-icon {
  font-size: 1.6rem; width: 48px; height: 48px; flex-shrink: 0;
  display: flex; align-items: center; justify-content: center;
  background: rgba(124,58,237,0.12); border-radius: 10px;
}
.skill-item strong { display: block; margin-bottom: 4px; font-size: 0.95rem; }
.skill-item p { color: var(--muted); font-size: 0.85rem; margin: 0; }

.hard-skill { margin-bottom: 28px; }
.hard-skill-header { display: flex; align-items: center; gap: 10px; margin-bottom: 8px; }
.hs-icon { font-size: 1.1rem; }
.hs-name { font-weight: 600; font-size: 0.95rem; min-width: 100px; }
.hs-bar-wrap {
  flex: 1; height: 6px; background: rgba(255,255,255,0.08);
  border-radius: 3px; overflow: hidden;
}
.hs-bar {
  height: 100%; width: 0;
  background: var(--grad); border-radius: 3px;
}
.hard-skill p { color: var(--muted); font-size: 0.85rem; margin: 0; }

/* ─────────────────────────────────────────
   PROJETOS
───────────────────────────────────────── */
.projetos-grid {
  display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 24px;
}
.projeto-card { padding: 28px; display: flex; flex-direction: column; gap: 12px; }
.projeto-card.featured { border-color: rgba(124,58,237,0.4); background: rgba(124,58,237,0.06); }
.projeto-header { display: flex; justify-content: space-between; align-items: center; }
.repo-icon { font-size: 1.3rem; }
.repo-badge {
  font-size: 0.7rem; font-weight: 700; letter-spacing: 0.06em;
  background: rgba(16,185,129,0.15); color: #34d399; border: 1px solid rgba(16,185,129,0.3);
  padding: 3px 10px; border-radius: 50px;
}
.badge-featured { background: rgba(124,58,237,0.2); color: #c4b5fd; border-color: rgba(124,58,237,0.4); }
.projeto-card h3 { font-size: 1.05rem; font-weight: 700; }
.projeto-card p { color: var(--muted); font-size: 0.875rem; flex: 1; }
.projeto-list { list-style: none; display: flex; flex-direction: column; gap: 4px; }
.projeto-list li { font-size: 0.82rem; color: var(--muted); }
.projeto-footer { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 8px; margin-top: 4px; }
.lang-badge { font-size: 0.75rem; color: var(--accent2); }
.btn-repo {
  font-size: 0.82rem; font-weight: 700; color: var(--accent1);
  text-decoration: none; transition: color var(--transition);
}
.btn-repo:hover { color: var(--accent3); }

.github-cta { text-align: center; margin-top: 48px; }
.btn-github {
  display: inline-flex; align-items: center; gap: 10px;
  background: rgba(255,255,255,0.06); border: 1.5px solid rgba(255,255,255,0.15);
  color: var(--text); text-decoration: none;
  padding: 14px 32px; border-radius: 50px; font-weight: 600;
  transition: background var(--transition), border-color var(--transition), transform var(--transition);
}
.btn-github:hover { background: rgba(124,58,237,0.15); border-color: var(--accent1); transform: translateY(-2px); }

/* ─────────────────────────────────────────
   TESTEMUNHOS
───────────────────────────────────────── */
.testemunhos-grid {
  display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 28px;
}
.testemunho-card { padding: 36px; position: relative; }
.quote-icon {
  font-size: 4rem; line-height: 1; color: var(--accent1); opacity: 0.4;
  font-family: Georgia, serif; position: absolute; top: 16px; left: 28px;
}
.testemunho-texto { font-size: 1rem; line-height: 1.75; color: var(--text); margin: 28px 0 24px; font-style: italic; }
.testemunho-author { display: flex; align-items: center; gap: 14px; }
.author-avatar {
  width: 44px; height: 44px; border-radius: 50%; flex-shrink: 0;
  background: var(--grad); display: flex; align-items: center; justify-content: center;
  font-weight: 700; font-size: 0.85rem;
}
.testemunho-author strong { display: block; font-size: 0.95rem; }
.testemunho-author span { font-size: 0.78rem; color: var(--muted); }

/* ─────────────────────────────────────────
   CONTATO
───────────────────────────────────────── */
.contato-grid {
  display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 20px;
}
.contato-card {
  display: flex; flex-direction: column; align-items: center; text-align: center;
  padding: 32px 20px; gap: 8px; text-decoration: none; color: var(--text);
}
.contato-icon { font-size: 2rem; margin-bottom: 6px; }
.contato-card strong { font-size: 1rem; font-weight: 700; }
.contato-card span { font-size: 0.82rem; color: var(--muted); word-break: break-all; }

/* ─────────────────────────────────────────
   FOOTER
───────────────────────────────────────── */
footer {
  background: var(--bg); border-top: 1px solid rgba(255,255,255,0.06);
  padding: 48px 24px;
}
.footer-inner {
  max-width: 1100px; margin: 0 auto;
  display: flex; flex-direction: column; align-items: center; gap: 10px; text-align: center;
}
.footer-inner p { color: var(--muted); font-size: 0.9rem; }
.footer-copy { font-size: 0.78rem; color: rgba(136,136,170,0.6); }

/* ─────────────────────────────────────────
   CERTIFICADOS
───────────────────────────────────────── */
.certs-grid {
  display: flex; flex-direction: column; gap: 24px;
}
.cert-item {
  display: flex; gap: 24px; padding: 28px; align-items: flex-start;
}
.cert-logo {
  font-size: 2.4rem; flex-shrink: 0;
  width: 64px; height: 64px;
  display: flex; align-items: center; justify-content: center;
  background: rgba(124,58,237,0.12); border-radius: 14px;
}
.cert-body { flex: 1; }
.cert-type {
  display: inline-block; font-size: 0.72rem; font-weight: 700;
  letter-spacing: 0.1em; text-transform: uppercase;
  color: var(--accent2); margin-bottom: 6px;
}
.cert-body h3 {
  font-size: 1.1rem; font-weight: 700; margin-bottom: 8px;
}
.cert-body p { color: var(--muted); font-size: 0.88rem; margin-bottom: 12px; }
.cert-topics {
  list-style: none; display: flex; flex-wrap: wrap; gap: 6px; margin-bottom: 16px;
}
.cert-topics li {
  font-size: 0.75rem; color: var(--muted);
  background: rgba(255,255,255,0.05); border: 1px solid rgba(255,255,255,0.1);
  padding: 3px 10px; border-radius: 50px;
}
.cert-footer {
  display: flex; justify-content: space-between; align-items: center;
  flex-wrap: wrap; gap: 10px;
}
.cert-date { font-size: 0.78rem; color: var(--muted); }
.btn-cert {
  font-size: 0.82rem; font-weight: 700; color: var(--accent1);
  text-decoration: none; padding: 7px 18px;
  border: 1.5px solid rgba(124,58,237,0.4); border-radius: 50px;
  transition: background var(--transition), color var(--transition);
}
.btn-cert:hover { background: var(--accent1); color: #fff; }

@media (max-width: 600px) {
  .cert-item { flex-direction: column; }
  .cert-footer { flex-direction: column; align-items: flex-start; }
}

/* ─────────────────────────────────────────
   RESPONSIVE
───────────────────────────────────────── */
@media (max-width: 768px) {
  .nav-links, .nav-cta { display: none; }
  .hamburger { display: block; }
  .hero-content { padding: 80px 24px; }
  .hero-visual { display: none; }
  .sobre-grid { grid-template-columns: 1fr; text-align: center; }
  .sobre-avatar { align-items: center; }
  .skills-wrapper { grid-template-columns: 1fr; }
  .skills-divider { display: none; }
  section { padding: 72px 0; }
}

@media (max-width: 480px) {
  .hero-title { font-size: 2.4rem; }
  .hero-actions { flex-direction: column; }
  .btn-primary, .btn-outline { text-align: center; }
}
