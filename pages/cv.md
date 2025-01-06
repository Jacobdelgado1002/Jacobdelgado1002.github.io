---
layout: page
title: CV
---

<!-- Container for the embedded CV -->
<div style="width: 100%; height: 600px; border: none; overflow: hidden;">
  <!-- Embed the PDF using an iframe -->
  <iframe 
    src="{{ site.baseurl }}/assets/CV.pdf" 
    width="100%" 
    height="100%" 
    style="border: none;">
    <!-- Fallback content if iframe is not supported -->
    Your browser does not support PDFs. Please <a href="{{ site.baseurl }}/assets/CV.pdf">download my CV here</a>.
  </iframe>
</div>

<!-- <meta http-equiv="refresh" content="0; URL=../assets/CV.pdf" /> -->