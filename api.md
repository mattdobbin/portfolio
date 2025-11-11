<section>
  <h2>GET /api/users</h2>
  <pre><code>fetch('/api/users').then(res => res.json())</code></pre>
  <button id="run">Run Example</button>
  <pre id="output"></pre>

  <script>
    document.getElementById('run').onclick = async () => {
      const res = await fetch('/api/users');
      document.getElementById('output').textContent = JSON.stringify(await res.json(), null, 2);
    };
  </script>
</section>
