<!-- Main Content -->
<main class="col-span-8 px-6">
    <div class="space-y-8 rounded-lg bg-white p-8 shadow-sm">
      <h1 class="mb-6 text-4xl font-bold text-blue-600">Accessible Images</h1>
  
      <section class="space-y-4" id="accessible-images">
        <h2 class="text-2xl font-bold text-gray-900">🖼️ Barrierefreie Bilder – einfach erklärt</h2>
  
        <p class="text-gray-700">
          Bilder machen Webseiten schöner – aber sie müssen auch für Menschen mit Behinderungen zugänglich sein. <br />
          Screenreader brauchen Alternativtexte („alt“), um Bilder zu beschreiben.
        </p>
  
        <h3 class="text-xl font-semibold text-gray-800" id="bildzweck">🎯 Was ist der Zweck des Bildes?</h3>
        <ul class="list-disc list-inside text-gray-700">
          <li>Ist das Bild wichtig für das Verständnis der Seite?</li>
          <li>Zeigt es eine Idee, Emotion oder Aktion?</li>
          <li>Oder ist es nur Deko?</li>
        </ul>
  
        <h3 class="text-xl font-semibold text-gray-800" id="dekorativ">🎨 Dekorative Bilder</h3>
        <p class="text-gray-700">
          Wenn ein Bild rein dekorativ ist, sollte es für Screenreader versteckt werden.
        </p>
        <ul class="list-disc list-inside text-gray-700">
          <li><code>alt=""</code> → leeres alt-Attribut</li>
          <li><code>role="presentation"</code> oder <code>role="none"</code></li>
          <li><code>aria-hidden="true"</code> → Vorsicht, kann zu viel verstecken</li>
          <li>Hintergrundbilder in CSS → werden automatisch ignoriert</li>
        </ul>
  
        <h3 class="text-xl font-semibold text-gray-800" id="informativ">📸 Informative Bilder</h3>
        <p class="text-gray-700">
          Zeigen Infos, z. B. Fotos, Icons oder Zeichnungen. <br />
          → Beschreibung im <code>alt</code>-Attribut schreiben.
        </p>
        <pre class="text-sm text-gray-600 bg-gray-100 p-2 rounded">&lt;img src="ladybugs.jpg" alt="Ein Schwarm Marienkäfer auf Rosenblättern"&gt;</pre>
        <p class="text-gray-700">
          Bei SVGs braucht man <code>role="img"</code> und ein <code>&lt;title&gt;</code> im SVG.
        </p>
  
        <h3 class="text-xl font-semibold text-gray-800" id="funktional">🔗 Funktionale Bilder</h3>
        <p class="text-gray-700">
          Bilder, die etwas machen – z. B. Buttons, Logos, Icons mit Links.
          <br />
          → Der alt-Text sollte die Aktion beschreiben, nicht das Aussehen.
        </p>
        <pre class="text-sm text-gray-600 bg-gray-100 p-2 rounded">&lt;img src="logo.png" alt="Zur Startseite navigieren"&gt;</pre>
  
        <h3 class="text-xl font-semibold text-gray-800" id="komplex">🧠 Komplexe Bilder</h3>
        <p class="text-gray-700">
          Beispiele: Infografiken, Karten, Diagramme. <br />
          → Kurzer alt-Text + längere Erklärung per Link oder extra Text.
        </p>
        <ul class="list-disc list-inside text-gray-700">
          <li><code>aria-describedby</code> → verweist auf längeren Text</li>
          <li><code>&lt;figure&gt;</code> + <code>&lt;figcaption&gt;</code> → Beschreibung im HTML</li>
          <li>Link zu weiterführenden Infos</li>
        </ul>
  
        <h3 class="text-xl font-semibold text-gray-800" id="best-practices">✅ Alt-Text: Best Practices</h3>
        <ul class="list-disc list-inside text-gray-700">
          <li>Text muss sinnvoll & kurz sein (max. ~150 Zeichen)</li>
          <li>Keine Wörter wie „Bild von...“ – das erkennt der Screenreader selbst</li>
          <li>Benutze klare Namen für Bilddateien (z. B. <code>ladybug-swarm.jpg</code>)</li>
          <li>Punktuation verwenden → besser verständlich</li>
          <li>Keine Keyword-Stuffing → schreibe natürlich!</li>
        </ul>
  
        <h3 class="text-xl font-semibold text-gray-800" id="fazit">🧾 Fazit: Bilder barrierefrei machen</h3>
        <p class="text-gray-700">
          Überlege dir immer: Was macht das Bild? Was soll vermittelt werden? <br />
          Dann wähle die passende Technik: alt-Text, aria, figcaption oder gar nichts.
        </p>
      </section>
    </div>
  </main>
  
  <!-- Right Sidebar -->
  <aside class="sticky top-24 col-span-2 h-max border-l border-gray-200 bg-gray-50 p-6">
    <div class="flex flex-col gap-2 text-sm">
      <h2 class="mb-2 text-lg font-bold text-gray-900">On this page</h2>
      <ul class="space-y-1">
        <li><a href="#accessible-images" class="text-blue-600 hover:underline">Barrierefreie Bilder</a></li>
        <li><a href="#bildzweck" class="text-gray-700 hover:underline">Bildzweck</a></li>
        <li><a href="#dekorativ" class="text-gray-700 hover:underline">Dekorativ</a></li>
        <li><a href="#informativ" class="text-gray-700 hover:underline">Informativ</a></li>
        <li><a href="#funktional" class="text-gray-700 hover:underline">Funktional</a></li>
        <li><a href="#komplex" class="text-gray-700 hover:underline">Komplex</a></li>
        <li><a href="#best-practices" class="text-gray-700 hover:underline">Alt-Text Tipps</a></li>
        <li><a href="#fazit" class="text-gray-700 hover:underline">Fazit</a></li>
      </ul>
    </div>
  </aside>
  