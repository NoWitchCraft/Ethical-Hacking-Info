# 🤝 Mitwirken an der Ethical Hacking Datenbank

Vielen Dank für Ihr Interesse, die größte deutschsprachige Ethical Hacking Datenbank mitzugestalten! Ihr Wissen ist der Schlüssel zum Erfolg dieses Projekts. Bevor Sie beginnen, lesen Sie bitte dieses Dokument und unseren Verhaltenskodex.

## 📜 1. Verhaltenskodex (Code of Conduct)

Um eine positive und konstruktive Community aufzubauen, bitten wir alle Mitwirkenden, unseren Verhaltenskodex zu respektieren.
> [Fügen Sie hier einen Link zu Ihrer **CODE_OF_CONDUCT.md** ein, sobald diese erstellt wurde.]

## 🚀 2. So tragen Sie bei – Der Workflow

Wir nutzen den standardmäßigen "Fork & Pull Request"-Workflow von GitHub.

1.  **Repository Forken:** Erstellen Sie eine Kopie (einen *Fork*) dieses Haupt-Repositories in Ihrem eigenen GitHub-Konto.
2.  **Branch erstellen:** Klonen Sie Ihren Fork lokal und erstellen Sie einen neuen Branch für Ihre Änderungen.
    * **Namenskonvention:** Nutzen Sie aussagekräftige Namen.
        * Für neue Einträge: `feat/neuer-angriff-titel`
        * Für Korrekturen: `fix/rechtschreibfehler-readme`
3.  **Änderungen vornehmen:** Fügen Sie Ihren neuen Datenbank-Eintrag hinzu oder bearbeiten Sie einen bestehenden (siehe Abschnitt 3).
4.  **Committen:** Führen Sie einen aussagekräftigen Commit durch.
    * **Guter Commit-Titel:** "Feat: Neuer Eintrag zu Subdomain Enumeration"
    * **Schlechter Commit-Titel:** "Änderungen gemacht"
5.  **Pull Request (PR) erstellen:** Senden Sie Ihren Branch als **Pull Request** vom Fork zurück an den `main`-Branch des Haupt-Repositories.
    * Beschreiben Sie Ihren Beitrag im PR so detailliert wie möglich.

## 🗂️ 3. Standard für Datenbank-Einträge

Um Konsistenz zu gewährleisten, **muss** jeder neue Datenbankeintrag das folgende Markdown-Template verwenden.

### 3.1. Template-Struktur

📝 Entwurf: Template für Konzepte & Systeme
Dieses Template sollte für erklärungsbedürftige Begriffe, Architekturen, Protokolle oder Verteidigungsstrategien verwendet werden. Speichern Sie diese Einträge in einem passenden Ordner wie z.B. concepts/ oder technologies/.
```markdown
# [Name des Konzepts/Systems]

## 📝 Kurzbeschreibung

[Maximal 2-3 Sätze, die das Konzept/System in seiner Essenz definieren und seinen Zweck im Kontext der IT-Sicherheit erklären.]

## 📖 Hintergrund & Funktionsweise

### Was ist es?
[Detaillierte Erklärung des Begriffs oder der Technologie. Beschreiben Sie die grundlegenden Mechanismen und Komponenten.]

* **Entwickelt von/Wann:** [Falls relevant: Wer hat es entwickelt und wann?]
* **Wichtige Komponenten/Phasen:** [Listen Sie die Kernelemente oder die Schritte des Prozesses auf.]

### 🔄 Einsatzszenario

[Beschreiben Sie, in welchem Kontext oder in welchen Umgebungen dieses Konzept/System typischerweise eingesetzt wird. (z.B. "Wird im Unternehmensnetzwerk zur Authentifizierung verwendet.")]

## 🛡️ IT-Sicherheitsrelevanz

[Dieser Abschnitt ist das Herzstück der Datenbank und verbindet das Konzept direkt mit der IT-Sicherheit.]

### 🚨 Schwachstellen & Risiken

[Welche potenziellen Sicherheitslücken oder Fehlkonfigurationen sind mit diesem System/Konzept verbunden?]

* **Risiko 1:** [Erklärung des Risikos, z.B. "Fehlende Protokollierung führt zu Blindspots."]
* **Risiko 2:** [Erklärung des Risikos, z.B. "Standardkonfigurationen sind anfällig für [Angriffsart]."]

### ⚔️ Angriffsvektoren (Ethical Hacking)

[Wie kann ein Ethical Hacker dieses System/Konzept ausnutzen oder testen?]

* **Vektor:** [Kurzer Titel, z.B. "Pass-the-Hash-Angriffe bei Kerberos"]
    * **Beschreibung:** [Kurze Erklärung des Vorgehens.]
    * **Relevante Tools:** [z.B. Impacket, Metasploit-Modul]

## ✅ Empfehlungen & Best Practices

[Wie kann die Sicherheit im Umgang mit diesem System/Konzept verbessert werden? (Verteidiger-Perspektive).]

1.  **Konfiguration:** [Spezifische Konfigurationshärten.]
2.  **Monitoring:** [Was sollte überwacht werden?]
3.  **Architektur:** [Design-Empfehlungen (z.B. Segmentierung, Least Privilege).]

## 🔗 Referenzen & Weiterführende Links

* [Offizielle Dokumentation (Hersteller/Standard-Gremium)]
* [Akademische oder branchenführende Analyse]
* [Deutschsprachiger Fachartikel]
```

#### 📝 Entwurf: Angriffe
Erstellen Sie die Datei im passenden Unterordner (z.B. `web_applications/`) und benennen Sie sie nach dem Angriff (z.B. `sql_injection_blind.md`).

```markdown
# [Titel des Eintrags/Angriffstechnik]

## 📝 Kurzbeschreibung

[Maximal 2-3 Sätze, die den Angriff/die Technik kurz zusammenfassen.]

## 🎯 Betroffene Systeme / Anwendungsfälle

* Welche Systeme sind typischerweise betroffen? (z.B. Webserver, Linux-Kernel, Mobile Apps)
* In welcher Phase des Pentests wird diese Technik angewendet? (z.B. Reconnaissance, Exploitation)

## 🛠️ Schritte zur Durchführung (PoC - Proof of Concept)

[Eine klare, schrittweise Anleitung, wie der Angriff durchgeführt werden kann.]

1.  Schritt 1: [Befehl, Tool oder Vorgehen]
2.  Schritt 2: [Befehl, Tool oder Vorgehen]

### Beispiel-Code / Tools
```bash
# Beispiel für einen Befehl, der das Vorgehen illustriert
ping -c 3 example.com

## 🛡️ Empfohlene Gegenmaßnahmen
[Wie kann dieser Angriff verhindert oder abgeschwächt werden? Konkrete Maßnahmen.]
- Maßnahme 1: [Technische Umsetzung]
- Maßnahme 2: [Organisatorische Vorkehrung]

## 🔗 Referenzen & Weiterführende Links
- [OWASP-Link oder CVE-ID]
- [Weiterführender deutschsprachiger Artikel]
- [Englischsprachige Quelle (optional)]
```
### 3.2. Wichtige Regeln für Inhalte

* **Sprache:** Alle Beiträge müssen in **hochwertigem Deutsch** verfasst sein (Fachbegriffe sind erlaubt).
* **Lesbarkeit:** Verwenden Sie Überschriften, Listen und Markdown-Formatierung, um den Text leicht lesbar zu machen.
* **Originalität/Quellen:** Verlinken Sie bitte immer die ursprünglichen Quellen oder Referenzen am Ende des Eintrags.
* **Kein illegaler Inhalt:** Das Repository dient ausschließlich der **Ethical Hacking Ausbildung** und der **Verbesserung der Sicherheit**. Alle Beiträge müssen diesem ethischen Grundsatz entsprechen.

## 🏷️ 4. Issues und Diskussionen

Wenn Sie sich nicht sicher sind, ob ein Thema relevant ist, oder wenn Sie einen Fehler gefunden haben:

1.  **Issue erstellen:** Nutzen Sie die GitHub Issues, um Bugs zu melden, neue Themen vorzuschlagen oder Fragen zu stellen.
2.  **Labels verwenden:** Wir nutzen Labels (z.B. `bug`, `feature request`, `good first issue`) zur Kategorisierung.
3.  **Keine sensiblen Daten:** Posten Sie niemals Passwörter, private Schlüssel oder andere sensible Informationen in Issues oder Pull Requests.

Wir freuen uns auf Ihre Beiträge!
