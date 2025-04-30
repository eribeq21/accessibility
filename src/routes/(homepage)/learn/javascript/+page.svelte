<!-- Main Content -->
<main class="col-span-8 px-6">
    <div class="space-y-8 rounded-lg bg-white p-8 shadow-sm">
      <h1 class="mb-6 text-4xl font-bold text-blue-600">JavaScript & Barrierefreiheit</h1>
  
      <section class="space-y-4" id="js-accessibility">
        <h2 class="text-2xl font-bold text-gray-900">🧠 Warum ist JavaScript wichtig für Barrierefreiheit?</h2>
  
        <p class="text-gray-700">
          JavaScript macht Webseiten interaktiv – zum Beispiel mit Popups, Menüs oder Formularen. <br />
          Aber: Wenn man es falsch nutzt, wird es für manche Menschen schwieriger, die Seite zu benutzen.
        </p>
  
        <h3 class="text-xl font-semibold text-gray-800" id="was-beachten">📌 Was muss man beachten?</h3>
        <ul class="list-disc list-inside text-gray-700">
          <li>✅ Benutze <code>&lt;button&gt;</code> statt <code>&lt;div onclick&gt;</code>, damit Tastatur und Screenreader funktionieren.</li>
          <li>✅ Achte auf den <strong>Fokus</strong> – beim Öffnen von Modalen oder beim Seitenwechsel sollte der Fokus sinnvoll gesetzt werden.</li>
          <li>✅ Ändere den <strong>Seitentitel</strong>, wenn neue Inhalte geladen werden – besonders in Single-Page-Apps (SPAs).</li>
          <li>✅ Nutze <code>aria-live</code>, um Screenreadern mitzuteilen, wenn neue Inhalte erscheinen (z. B. Fehlermeldungen oder Bestätigungen).</li>
          <li>❌ Vermeide es, CSS direkt im JavaScript zu ändern – nutze lieber CSS-Klassen.</li>
          <li>✅ Mache Zustände sichtbar – z. B. mit <code>aria-expanded</code>, <code>aria-pressed</code> oder <code>aria-hidden</code>.</li>
          <li>✅ Wenn du etwas mit JavaScript sichtbar oder unsichtbar machst, achte darauf, dass der Screenreader es auch merkt.</li>
          <li>✅ Nutze Tastatur-Events wie <code>keydown</code> zusätzlich zu <code>click</code>, damit auch Nicht-Maus-Nutzer interagieren können.</li>
        </ul>
  
        <h3 class="text-xl font-semibold text-gray-800" id="bonus-tipp">⚙️ Bonus-Tipp</h3>
        <p class="text-gray-700">
          Es gibt Bibliotheken, die dir helfen können – z. B. <code>react-aria-live</code> oder <code>focus-trap</code>. <br />
          Und: Teste deine Seite mit Tastatur und Screenreader!
        </p>
  
        <h3 class="text-xl font-semibold text-gray-800" id="fazit-js">✅ Fazit</h3>
        <p class="text-gray-700">
          JavaScript ist super – aber nur, wenn es für alle funktioniert. <br />
          Denke an Tastatur-Nutzer und Menschen mit Screenreadern. <br />
          Kleine Änderungen machen einen großen Unterschied!
        </p>
      </section>
    </div>
  </main>

  <!-- Right Sidebar -->
<aside class="sticky top-24 col-span-2 h-max border-l border-gray-200 bg-gray-50 p-6">
    <div class="flex flex-col gap-2 text-sm">
      <h2 class="mb-2 text-lg font-bold text-gray-900">On this page</h2>
      <ul class="space-y-1">
        <li><a href="#js-accessibility" class="text-blue-600 hover:underline">JavaScript & Barrierefreiheit</a></li>
        <li><a href="#was-beachten" class="text-gray-700 hover:underline">Was muss man beachten?</a></li>
        <li><a href="#bonus-tipp" class="text-gray-700 hover:underline">Bonus-Tipp</a></li>
        <li><a href="#fazit-js" class="text-gray-700 hover:underline">Fazit</a></li>
      </ul>
    </div>
  </aside>
  