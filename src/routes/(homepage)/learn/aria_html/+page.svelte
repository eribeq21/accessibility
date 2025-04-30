<script>
	

</script>

<!-- Main Content -->
<main class="col-span-8 px-6">
  <div class="space-y-8 rounded-lg bg-white p-8 shadow-sm">
    <h1 class="mb-6 text-4xl font-bold text-blue-600">Aria & Html</h1>

    <section class="space-y-4" id="aria-and-html">
      <h2 class="text-2xl font-bold text-gray-900">🌐 HTML & ARIA einfach erklärt</h2>

      <p class="text-gray-700">
        HTML ist die Standardsprache fürs Web. <br />
        ARIA (Accessible Rich Internet Applications) hilft Menschen mit Behinderungen, Webseiten besser zu nutzen – z. B. mit Screenreadern.
      </p>
      <p class="text-gray-700">
        ARIA ist kein eigener Code, sondern Zusatz-Infos, die man zu HTML-Elementen schreibt. <br />
        ARIA zeigt, was ein Element ist (Rolle), wie es gerade ist (Zustand) und welche Eigenschaften es hat.
      </p>

      <h3 class="text-xl font-semibold text-gray-800" id="geschichte">📅 Kurze Geschichte von ARIA</h3>
      <p class="text-gray-700">
        ARIA wurde 2008 vom W3C entwickelt. <br />
        Es hilft besonders bei dynamischen Inhalten oder komplexen UI-Elementen.
      </p>

      <h3 class="text-xl font-semibold text-gray-800" id="rollen">🧱 Die drei Hauptteile von ARIA</h3>
      <ul class="list-inside list-disc text-gray-700">
        <li><strong>Role:</strong> Was das Element ist — z. B. <code>&lt;div role="button"&gt;</code></li>
        <li><strong>Property:</strong> Welche Eigenschaften es hat — z. B. <code>aria-describedby="info"</code></li>
        <li><strong>State:</strong> Aktueller Zustand — z. B. <code>aria-pressed="false"</code></li>
      </ul>

      <h3 class="text-xl font-semibold text-gray-800" id="tree">🌲 Accessibility Tree</h3>
      <p class="text-gray-700">
        Der Accessibility Tree ist wie der normale DOM, aber für Screenreader. <br />
        ARIA hilft dabei, diesen Baum besser verständlich zu machen.
      </p>

      <h3 class="text-xl font-semibold text-gray-800" id="einsatz">🛠️ Wann (nicht) ARIA verwenden?</h3>
      <p class="text-gray-700">
        ✅ Nutze HTML, wenn möglich: <code>&lt;button&gt;</code> ist besser als <code>&lt;div role="button"&gt;</code>.
      </p>

      <h3 class="text-xl font-semibold text-gray-800" id="rules">🔁 Die 5 ARIA-Regeln</h3>
      <ul class="list-disc list-inside text-gray-700">
        <li>❌ Verwende ARIA nur, wenn nötig. → HTML reicht oft aus.</li>
        <li>❌ Füge kein unnötiges ARIA zu HTML hinzu. → Macht es nur komplizierter.</li>
        <li>✅ Elemente müssen mit der Tastatur bedienbar sein. → z. B. <code>tabindex="0"</code> für Fokus.</li>
        <li>❌ Verstecke keine fokussierbaren Elemente mit <code>aria-hidden</code>. → Sonst sieht der Screenreader sie nicht.</li>
        <li>✅ Alle interaktiven Elemente brauchen einen Namen. → z. B. <code>&lt;img alt="Red leather boots"&gt;</code></li>
      </ul>

      <h3 class="text-xl font-semibold text-gray-800" id="beispiele">🤔 Beispiele guter Praxis</h3>
      <p class="text-gray-700">GUT: <code>&lt;button&gt;Submit&lt;/button&gt;</code></p>
      <p class="text-gray-700">SCHLECHT: <code>&lt;a role="button"&gt;Submit&lt;/a&gt;</code></p>
      <p class="text-gray-700">GUT: <code>&lt;ul&gt;</code></p>
      <p class="text-gray-700">SCHLECHT: <code>&lt;ul role="list"&gt;</code></p>

      <h3 class="text-xl font-semibold text-gray-800" id="fazit">⚠️ Fazit: ARIA ist mächtig, aber kompliziert</h3>
      <p class="text-gray-700">
        Nutze es nur, wenn nötig. Teste deine Seite mit Screenreadern oder Chrome DevTools. <br />
        Denke immer an alle Nutzer, nicht nur an Sehende.
      </p>
    </section>
  </div>
</main>

<!-- Right Sidebar -->
<aside class="sticky top-24 col-span-2 h-max border-l border-gray-200 bg-gray-50 p-6">
  <div class="flex flex-col gap-2 text-sm">
    <h2 class="mb-2 text-lg font-bold text-gray-900">On this page</h2>
    <ul class="space-y-1">
      <li><a href="#aria-and-html" class="text-blue-600 hover:underline">HTML & ARIA</a></li>
      <li><a href="#geschichte" class="text-gray-700 hover:underline">Kurze Geschichte</a></li>
      <li><a href="#rollen" class="text-gray-700 hover:underline">Hauptteile</a></li>
      <li><a href="#tree" class="text-gray-700 hover:underline">Accessibility Tree</a></li>
      <li><a href="#einsatz" class="text-gray-700 hover:underline">Wann ARIA nutzen?</a></li>
      <li><a href="#rules" class="text-gray-700 hover:underline">5 Regeln</a></li>
      <li><a href="#beispiele" class="text-gray-700 hover:underline">Beispiele</a></li>
      <li><a href="#fazit" class="text-gray-700 hover:underline">Fazit</a></li>
    </ul>
  </div>
</aside>
