---
permalink: /
title: "Hi, there! I'm Zihao (Gavin)."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I study whether the explanations that large language models give for their answers, in particular chain-of-thought reasoning, faithfully report what drove those answers, and how to measure and train such faithfulness.
{: .lede}

I build counterfactual and interpretability-based evaluations with proper baselines, and model organisms with known hidden influences as ground truth, toward trustworthy and auditable AI, especially in high-stakes domains. I am available for internships from May 2027 to August 2027.

I am a second-year CS PhD student at [Northeastern University](https://www.northeastern.edu/), advised by Professor [Byron Wallace](https://www.byronwallace.com/). I graduated cum laude from [New York University](https://www.nyu.edu/) with a Bachelor's degree in Computer Science and Data Science. Previously, I worked in VisionX Lab as a research intern, advised by Professor [Saining Xie](https://www.sainingxie.com/). During my undergraduate program, I worked in [OLAB](https://www.nyuolab.org/) and Memo Lab, advised by Professor [Eric K. Oermann](https://nyulangone.org/doctors/1235498403/eric-k-oermann) and Professor [Shuo Chen](https://shuolab.github.io/) respectively.

I have been fortunate to be advised by Professor Xie, Professor Oermann, and Professor Chen. I am also grateful for the mentorship from [Lavender Y. Jiang](https://lavenderjiang.github.io/), [Xujin C. Liu](https://scholar.google.com/citations?user=ZY-JsPoAAAAJ&hl=en), Professor [Kyunghyun Cho](https://kyunghyuncho.me/), and Professor [Samuel R. Bowman](https://sleepinyourhat.github.io/).

Email: [yang.zih@northeastern.edu](mailto:yang.zih@northeastern.edu) or [gavin.yang@nyu.edu](mailto:gavin.yang@nyu.edu). CV: [PDF]({{ '/files/Resume_Zihao(Gavin)_Yang.pdf' | relative_url }}).

## Publications

### Peer-reviewed

{% include publications.html group="peer-reviewed" %}

### Preprints and manuscripts

{% include publications.html group="preprint" %}

## Education

+ 2025–present: Ph.D., Computer Science, Northeastern University, Boston, MA, USA
+ 2020–2024: B.A., Computer Science & Data Science, Minor in Mathematics, New York University, New York, NY, USA
{: .education}

<div class="visitor-map">
<script>
  (function () {
    var pages = {
      light: '{{ '/visitor-map/day.html' | relative_url }}',
      dark: '{{ '/visitor-map/night.html' | relative_url }}'
    };
    var root = document.documentElement;
    var box = document.currentScript.parentNode;
    var frames = {};
    function fit(frame, tries) {
      var widget = frame.contentDocument && frame.contentDocument.getElementById('mapmyvisitors-widget');
      if (widget && widget.offsetHeight) {
        frame.style.height = widget.offsetHeight + 'px';
      } else if (tries > 0) {
        setTimeout(function () { fit(frame, tries - 1); }, 200);
      }
    }
    function load(theme) {
      var frame = document.createElement('iframe');
      frame.className = 'visitor-map__frame';
      frame.title = 'Visitor map';
      frame.setAttribute('scrolling', 'no');
      frame.onload = function () { fit(frame, 50); };
      frame.src = pages[theme];
      box.appendChild(frame);
      frames[theme] = frame;
    }
    function show() {
      var theme = root.getAttribute('data-theme') === 'dark' ? 'dark' : 'light';
      if (!frames[theme]) { load(theme); }
      for (var name in frames) { frames[name].classList.toggle('is-hidden', name !== theme); }
    }
    show();
    new MutationObserver(show).observe(root, { attributes: true, attributeFilter: ['data-theme'] });
  })();
</script>
</div>
