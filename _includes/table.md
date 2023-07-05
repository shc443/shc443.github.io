

|:------------------------------|:-------------------:|:-------------------:|
| Xinapse.ai                  | &#x2714;            | &#x2714;            |
| XLP Capital                 | &#x2714;            | &#x2714;            |
| State Street                | &#x2714;            | &#x2714;            |
| Republic of Korea Army      |                     | &#x2714;            |
| Haver Analytics             |                     | &#x2714;            |
|===============================+=====================+=====================|
|                               | [__Download__][kit] | [__Buy PRO__][buy]{:.gumroad-button data-gumroad-single-product="true"} |
{:.stretch-table.dl-table}

[^21]: Large screens (> 1664px width) only.

[^22]: Price now permanently reduced by <strong class="discount">30%</strong>! Use the offer code <strong class="code">QR0TW8M</strong> to apply this discount later.
       {:.ppi}
       If you're upgrading from Hydejack 8, find your upgrade discount code in the latest zip download.

<script type="module">
  document.querySelectorAll('a[href="#_search-input"]').forEach(el => {
    if (!el.dataset.done) {
      el.addEventListener('click', () => document.getElementById('_search-input').focus());
      el.dataset.done = '';
    }
  });

  document.querySelectorAll('.ppi').forEach(async el => {
    if (!el.dataset.done) {
      const { name, emoji, code, discount } = await window._ppiData;
      if (!code) return;
      el.querySelectorAll('.name').forEach(el => { el.innerText = name });
      el.querySelectorAll('.emoji').forEach(el => { el.innerText = emoji; el.title = name });
      el.querySelectorAll('.code').forEach(el => { el.innerText = code.toUpperCase() });
      el.querySelectorAll('.discount').forEach(el => { el.innerText = `${discount * 100}%` });
      el.dataset.done = '';
    }
  });

  document.querySelectorAll('.price').forEach(async el => {
    if (!el.dataset.done) {
      const { name, emoji, code, discount } = await window._ppiData;
      if (!code) return;
      el.querySelectorAll('.name').forEach(el => { el.innerText = name });
      el.querySelectorAll('.emoji').forEach(el => { el.innerText = emoji; el.title = name });
      el.querySelectorAll('.code').forEach(el => { el.innerText = code.toUpperCase() });
      el.querySelectorAll('.new-price').forEach(el => { el.innerText = `$${99 - discount * 100}` });
      el.dataset.done = '';
    }
  });
</script>
