## Footer Implementation

### Requirement
Display version, deploy date, and author information in the website footer.

### Footer Format
```
Pravin Mishra Portfolio v1.0 — Deployed on <DD Mon YYYY> — By <Your Name>
```

### How Deploy Date is Generated
The deploy date is automatically generated using JavaScript when the page loads.

### Code Snippet
```html
<footer>
  Pravin Mishra Portfolio v1.0 — Deployed on <span id="deployDate"></span> — By Michael Uche Vincent
</footer>

<script>
  const date = new Date();
  const options = { day: '2-digit', month: 'short', year: 'numeric' };
  document.getElementById('deployDate').textContent = 
    date.toLocaleDateString('en-GB', options);
</script>
```