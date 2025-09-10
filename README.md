README.md
# Mini Finance

This is a simple web application deployed on AWS EC2.

## Footer Versioning

The footer automatically displays the version, deployment date, and author:


### Dynamic Date Implementation

In `index.html`, the footer contains a placeholder:

```html
<footer class="site-footer">
  <p class="copyright-text">
    Mini Finance v1.0 — Deployed on <span id="deploy-date"></span> — By Thelma
  </p>
</footer>
<script>
  const options = { day: '2-digit', month: 'short', year: 'numeric' };
  document.getElementById("deploy-date").textContent =
    new Date().toLocaleDateString("en-GB", options);
</script>
