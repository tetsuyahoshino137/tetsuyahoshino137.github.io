---
layout: default
title: Home
---

<!-- Profile -->
<div class="profile">
  <div class="profile-info">
    <h1>{{ site.name }}</h1>
    <p>{{ site.position }}</p>
    <ul>
      <li>
        <span class="icon">@</span>
        <span>
          {{ site.email | replace: "@", "[at]" }}
          <button class="copy-btn" onclick="navigator.clipboard.writeText('{{ site.email }}')">Copy</button>
        </span>
      </li>
      <li>
        <span class="icon">📄</span>
        <a href="{{ site.cv }}">CV (December 2025)</a>
      </li>
    </ul>

    {% if site.seminars %}
    <strong>Upcoming Seminars/Conferences:</strong>
    <ul class="upcoming-list">
      {% for s in site.seminars %}
      <li>{{ s }}</li>
      {% endfor %}
    </ul>
    {% endif %}
  </div>
</div>

---

## Working Papers

* [Elections with Opinion Polls: Information Acquisition and Aggregation](GombergHoshino/GombergHoshino250408.pdf) (with Andrei Gomberg)  
  \[[Slides](GombergHoshino/GombergHoshinoSlide250503_CETC.pdf)\] \[[Replication codes](#)\]

* [Rational Inattention and Endogenous Volatility: A Large Deviation Approach](HoshinoUi/HoshinoUi20251120.pdf) (with Takashi Ui)  
  \[[Slides](HoshinoUi/StatMechRI_BRIC.pdf)\]  
  To be presented at Seoul National University (February 13)

* [Indirect Enforcement and the Transformation of Organized Crime: Evidence from the Yakuza](HoshinoKamada/YakuzaFraud20260125.pdf) (with Takuma Kamada)

* [Two-Sided Markets and Restricted Boltzmann Machines](HoshinoPancs/HoshinoPancs20250513.pdf) (with Romans Pancs)  
  \[[Slides](HoshinoPancs/HoshinoPancs_EconometricSocietyAIML.pdf)\] \[[Replication codes](#)\]  
  <span class="red">R&R at *Management Science*</span>

* Recursive Rational Inattention Is Entropic (with Henrique De Oliveira)  
  \[[Slides](#)\]

* [Rational Inattention in Games](jmp2019/ri_in_games_jmp.pdf)  
  A part of this paper is subsumed by the joint work with Takashi Ui.

---

## Publications

* [Bargaining and Information Acquisition](ChatterjeeDongHoshino/ChatterjeeDongHoshino20240904.pdf) (with Kalyan Chatterjee and Miaomiao Dong)  
  <span class="red">[*American Economic Journal: Micro*](https://www.aeaweb.org/articles?id=10.1257/mic.20240034) (2025)</span>

* [Multi-Agent Persuasion: Leveraging Strategic Uncertainty](HoshinoMultiAgent/Hoshino20210901.pdf)  
  <span class="red">[*International Economic Review*](https://onlinelibrary.wiley.com/doi/10.1111/iere.12546) (2022)</span>

* [Third-Party Policing Approaches against Organized Crime](HoshinoKamada/yakuza_20200601.pdf) (with Takuma Kamada)  
  <span class="red">[*Journal of Quantitative Criminology*](https://link.springer.com/article/10.1007/s10940-020-09466-6) (2021)</span>

* [Repeated Coordination with Private Learning](BasuChatterjeeHoshinoTamuz/BasuChatterjeeHoshinoTamuz20200731.pdf) (with Pathikrit Basu, Kalyan Chatterjee, and Omer Tamuz)  
  <span class="red">[*Journal of Economic Theory*](https://www.sciencedirect.com/science/article/abs/pii/S0022053120300995) (2020)</span>
