# Farhad Javanmardi

Ich baue und betreibe Software für kleine Betriebe — vom ersten Entwurf bis zum
laufenden System mit echten Nutzern. Karlsruhe.

---

## Logic Style — KI-Simulation für Friseursalons

**[logicstyle.vercel.app](https://logicstyle.vercel.app)** · Quellcode privat, Einblick auf Anfrage

Der Salon fotografiert die Kundin, wählt ein Modell, und die Anwendung zeigt in
Sekunden, wie Schnitt, Farbe oder Bart aussehen würden. Aus der Beratung wird
ein Bild statt einer Beschreibung.

- Frontend ohne Framework, als PWA installierbar
- **Supabase** als Backend: PostgreSQL mit Row Level Security, **27 Edge Functions** in TypeScript
- **Google Gemini** für die Bildgenerierung, Prompt-Aufbau vollständig serverseitig
- **291 Modellbeschreibungen**: Damen- und Herrenschnitte, Fades, Bärte, Farb- und Behandlungsdienste
- Mehrmandantenfähig: Salonkonten, Kontingente je Konto, Adminbereich
- Kundenfotos werden nicht gespeichert; Verzeichnis von Verarbeitungstätigkeiten, Impressum und Einwilligung gehören zum Projekt

Zum selben System gehören eine [Akademie](https://logicstyle.vercel.app/aca) mit
über 13.400 Übersetzungszeilen in vier Sprachen, ein
[Buchhaltungs- und Kosten-Cockpit](https://logicstyle.vercel.app/buchhaltung_standalone.html)
und eine [Modell-Galerie](https://logicstyle.vercel.app/models). Die
Veröffentlichung auf Instagram und Telegram läuft über geplante Funktionen
automatisch.

## LogicStyle Deutsch — Artikel und Grammatik

**[logicstyle.vercel.app/deutsch](https://logicstyle.vercel.app/deutsch)**

Übungs-App für deutsche Artikel und Grammatik von A1 bis B2, ausgelegt auf
Berufskurs-Lernende. **403 handgeprüfte Wörter** aus dem Arbeitsalltag mit ihrem
Artikel — bewusst ein geprüfter Datensatz statt einer Abfrage gegen eine
ungeprüfte Quelle, damit das Quiz nie etwas Falsches beibringt. Läuft ohne
Verbindung.

## Gold Intelligence — Entscheidungshilfe für XAU/USD

**[kolbenarenji.com/gold](https://kolbenarenji.com/gold)** · [Quellcode](https://github.com/farhadjavanmardi-art/kolbenarenji)

Auswertung von Kursdaten zu einer nachvollziehbaren Einschätzung, mit einer
Analysefunktion im Backend. Die Rechenlogik liegt in einer eigenen Engine, damit
die Bewertung nachvollziehbar bleibt und nicht in der Oberfläche verschwindet.

## Kolbe Narenji — Buchung und Verwaltung einer Ferienunterkunft

**[kolbenarenji.com](https://kolbenarenji.com)** · [Quellcode](https://github.com/farhadjavanmardi-art/kolbenarenji)

Buchungsseite, Adminbereich, Übergabeformular und Kundenverwaltung. Persisch,
von rechts nach links gesetzt.

---

## Wie ich arbeite

Ich messe nach, statt anzunehmen.

Ein Beispiel aus dem laufenden Betrieb: Für die Bartsimulation kam eine wählbare
Fade-Höhe dazu. Ein Prüflauf über 99 Fälle zeigte, dass der erzeugte Prompt
exakt stimmte — 93 Fälle Zeichen für Zeichen unverändert, die sechs betroffenen
um immer denselben Betrag gewachsen. Trotzdem sahen die erzeugten **Bilder**
identisch aus. Die Ursache stand im Prompt selbst: zwei Anweisungen
widersprachen sich, und die einschränkende gewann. Ein korrekt gebauter Prompt
ist eben noch kein korrektes Bild.

- Prüfsummen statt Stichproben, wenn Text maschinell gebaut wird
- ein Selbsttest-Endpunkt, der den fertigen Prompt ohne Bildkosten zurückgibt
- Kommentare erklären, **warum** etwas so ist, nicht was die Zeile tut

## Technik

JavaScript · TypeScript (Deno) · PostgreSQL · Supabase · Vercel · Gemini API ·
PWA und TWA · Meta Graph API · Telegram Bot API · n8n · Git

---

*English — I build and run software for small businesses: an AI hair and beard
simulation for salons, a German grammar trainer, a decision-support tool for
gold prices, and a booking and admin system for a guesthouse. All are live and
linked above. Details in German; happy to talk in English.*
