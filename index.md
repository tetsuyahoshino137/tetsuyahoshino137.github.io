---
layout: default
title: Home
---

<link href="https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,400;0,600;0,700;1,400&family=M+PLUS+Rounded+1c:wght@400;500;700&display=swap" rel="stylesheet">
<style>
.hoshino-page *, .hoshino-page *::before, .hoshino-page *::after { box-sizing: border-box; margin: 0; padding: 0; }
.hoshino-page {
  font-family: 'Nunito', 'M PLUS Rounded 1c', sans-serif;
  font-size: 16.5px; line-height: 1.6; color: #2a2a2a;
  max-width: 700px; margin: 0 auto;
}

/* ヘッダー */
.hoshino-page .page-header { display: block; margin-bottom: 2rem; padding: 0; border: none; }
.hoshino-page .page-header h1 { font-size: 1.9rem; font-weight: 700; color: #1a1a1a; letter-spacing: 0.005em; margin-bottom: 0.1rem; }
.hoshino-page .position { font-size: 1rem; color: #666; margin-bottom: 1rem; }
.hoshino-page .meta-row { display: flex; flex-direction: column; gap: 0.3rem; font-size: 1rem; }
.hoshino-page .meta-row a { color: #2a6496; text-decoration: none; font-weight: 700; }
.hoshino-page .meta-row a:hover { text-decoration: underline; }
.hoshino-page .meta-row .lbl { color: #999; font-weight: 600; }
.hoshino-page .meta-row code { font-size: 1rem; color: #444; }
.hoshino-page .copy-btn { font-family: inherit; font-size: 0.7rem; font-weight: 700; letter-spacing: 0.03em; padding: 0.08rem 0.45rem; border: 1px solid #ccc; border-radius: 3px; background: transparent; color: #888; cursor: pointer; }
.hoshino-page .copy-btn:hover { background: #2a6496; color: #fff; border-color: #2a6496; }

/* Upcoming */
.hoshino-page .upcoming { margin-bottom: 0.5rem; }
.hoshino-page .upcoming-title { font-size: 0.72rem; font-weight: 700; letter-spacing: 0.13em; text-transform: uppercase; color: #bbb; margin-bottom: 0.5rem; }
.hoshino-page .upcoming-list { list-style: none; }
.hoshino-page .upcoming-list li { font-size: 0.85rem; color: #888; line-height: 1.7; }
.hoshino-page .upcoming-list li .date { color: #aaa; }

/* セクション見出し */
.hoshino-page .section { margin-top: 2.8rem; }
.hoshino-page .section h2 {
  font-size: 1rem; font-weight: 700; letter-spacing: 0.16em; text-transform: uppercase;
  color: #2a6496; padding-bottom: 0.5rem; margin-bottom: 1.3rem;
  border-bottom: 1px solid #e6e4dd;
}

/* 論文リスト: 余白主体、罫線なし */
.hoshino-page .paper-list { list-style: none; }
.hoshino-page .paper-list > li { margin-bottom: 1.35rem; }
.hoshino-page .paper-list > li:last-child { margin-bottom: 0; }
.hoshino-page .paper-title { font-weight: 700; color: #1a1a1a; line-height: 1.45; margin-bottom: 0.1rem; }
.hoshino-page .paper-title a { color: #2a6496; text-decoration: none; background-image: linear-gradient(#2a6496,#2a6496); background-size: 0% 1.5px; background-repeat: no-repeat; background-position: 0 100%; transition: background-size 0.2s; padding-bottom: 1px; }
.hoshino-page .paper-title a:hover { color: #2a6496; background-size: 100% 1.5px; }
.hoshino-page .paper-sub { font-size: 1rem; color: #555; }
.hoshino-page .paper-pub { font-size: 1rem; margin-top: 0.05rem; }
.hoshino-page .paper-sub a { color: #2a6496; text-decoration: none; }
.hoshino-page .paper-sub a:hover { text-decoration: underline; }
.hoshino-page .badge { color:#c0392b; font-weight: 600; }
.hoshino-page .badge a { color:#c0392b; }
.hoshino-page .dot { color: #ccc; margin: 0 0.4rem; }
.hoshino-page a { color: #2a6496; }

/* ===== レスポンシブ ===== */
@media (max-width: 600px) {
  .hoshino-page { font-size: 16px; }
  .hoshino-page .page-header h1 { font-size: 1.6rem; }
  .hoshino-page .section h2 { font-size: 0.95rem; letter-spacing: 0.1em; }
  .hoshino-page .paper-sub, .hoshino-page .paper-pub { font-size: 0.95rem; }
  .hoshino-page .meta-row { font-size: 0.95rem; }
  .hoshino-page .meta-row code { word-break: break-all; }
}
</style>

<div class="hoshino-page">

  <div class="page-header">
    <h1>{{ site.name }}</h1>
    <p class="position">{{ site.position }}</p>
    <div class="meta-row">
      <a href="TetsuyaHoshinoCV260510.pdf">CV (26-05-10)</a>
      <span><span class="lbl">Email:</span> <code>{{ site.email | replace: "@", "[at]" }}</code> <button class="copy-btn" onclick="navigator.clipboard.writeText('{{ site.email }}')">Copy</button></span>
    </div>
  </div>

  <div class="upcoming">
    <div class="upcoming-title">Upcoming Seminars and Conferences</div>
    <ul class="upcoming-list">
      <li>Chung-Ang U. Conference @ Chung-Ang U. <span class="date">(26-05-28)</span></li>
      <li>KISDI <span class="date">(26-06-18)</span></li>
      <li>Waseda U. <span class="date">(26-06-23)</span></li>
      <li>Keio U. <span class="date">(26-06-26)</span></li>
      <li>Contract Theory Workshop @ Doshisha U. <span class="date">(26-07-18)</span></li>
      <li>Workshop on Search and Platform @ Kyoto U. <span class="date">(26-07-23)</span></li>
    </ul>
  </div>

  <div class="section">
    <h2>Working Papers</h2>
    <ul class="paper-list">
      <li>
        <div class="paper-title"><a href="papers/GombergHoshino250408.pdf">Elections with Opinion Polls: Information Acquisition and Aggregation</a></div>
        <div class="paper-sub">with Andrei Gomberg<span class="dot">·</span><a href="slides/GombergHoshino_CETC.pdf">Slides</a><span class="dot">·</span><a href="https://colab.research.google.com/drive/1Udqhdzlq0Cck9HbkMKYVyT4HPwApEFsW?usp=sharing">Codes</a></div>
      </li>
      <li>
        <div class="paper-title">Rational Inattention and Endogenous Volatility: A Large Deviation Approach</div>
        <div class="paper-sub">with Takashi Ui<span class="dot">·</span><a href="slides/HoshinoUi_BRIC.pdf">Slides</a></div>
      </li>
      <li>
        <div class="paper-title"><a href="papers/HoshinoKamada260125.pdf">Indirect Enforcement and the Transformation of Organized Crime: Evidence from the Yakuza</a></div>
        <div class="paper-sub">with Takuma Kamada</div>
        <div class="paper-pub"><span class="badge">R&amp;R at <em>Journal of Comparative Economics</em></span></div>
      </li>
      <li>
        <div class="paper-title"><a href="papers/HoshinoPancs260406.pdf">Estimating Pair-Specific Network Effects in Binary-Action Games: Two-Sided Markets via Restricted Boltzmann Machines</a></div>
        <div class="paper-sub">with Romans Pancs<span class="dot">·</span><a href="slides/HoshinoPancs_EconometricSocietyAIML.pdf">Slides</a><span class="dot">·</span><a href="https://colab.research.google.com/drive/1zIY4-pjJv4uWzs7OlHq-XOe5-MAmSGNU?usp=sharing">Codes</a></div>
        <div class="paper-pub"><span class="badge">R&amp;R at <em>Management Science</em></span></div>
      </li>
      <li>
        <div class="paper-title">Recursive Rational Inattention Is Entropic</div>
        <div class="paper-sub">with Henrique De Oliveira<span class="dot">·</span><a href="slides/DeoliveiraHoshino_EconometricSociety.pdf">Slides</a></div>
      </li>
      <li>
        <div class="paper-title"><a href="papers/HoshinoJMP.pdf">Rational Inattention in Games</a></div>
        <div class="paper-sub">Partially subsumed by joint work with Takashi Ui.</div>
      </li>
    </ul>
  </div>

  <div class="section">
    <h2>Publications</h2>
    <ul class="paper-list">
      <li>
        <div class="paper-title"><a href="papers/ChatterjeeDongHoshinoAEJ240904.pdf">Bargaining and Information Acquisition</a></div>
        <div class="paper-sub">with Kalyan Chatterjee and Miaomiao Dong</div>
        <div class="paper-pub"><span class="badge"><a href="https://www.aeaweb.org/articles?id=10.1257/mic.20240034"><em>American Economic Journal: Micro</em></a> (2025)</span></div>
      </li>
      <li>
        <div class="paper-title"><a href="papers/HoshinoIER210901.pdf">Multi-Agent Persuasion: Leveraging Strategic Uncertainty</a></div>
        <div class="paper-pub"><span class="badge"><a href="https://onlinelibrary.wiley.com/doi/10.1111/iere.12546"><em>International Economic Review</em></a> (2022)</span></div>
      </li>
      <li>
        <div class="paper-title"><a href="papers/HoshinoKamadaJQC200601.pdf">Third-Party Policing Approaches against Organized Crime</a></div>
        <div class="paper-sub">with Takuma Kamada</div>
        <div class="paper-pub"><span class="badge"><a href="https://link.springer.com/article/10.1007/s10940-020-09466-6"><em>Journal of Quantitative Criminology</em></a> (2021)</span></div>
      </li>
      <li>
        <div class="paper-title"><a href="papers/BasuChatterjeeHoshinoTamuzJET200731.pdf">Repeated Coordination with Private Learning</a></div>
        <div class="paper-sub">with Pathikrit Basu, Kalyan Chatterjee, and Omer Tamuz</div>
        <div class="paper-pub"><span class="badge"><a href="https://www.sciencedirect.com/science/article/abs/pii/S0022053120300995"><em>Journal of Economic Theory</em></a> (2020)</span></div>
      </li>
    </ul>
  </div>

</div>
