# Skyloong Bridge 0.2.1 · App mit Logo

Die App enthält ihre Laufzeiten und alle 274 freigeschalteten Modellprofile. Es werden kein Projektordner, Terminal, Python und keine Entwicklungswerkzeuge zum Starten benötigt. Logitech G Hub muss separat installiert sein.

1. `Skyloong Bridge.app` an den gewünschten Ort kopieren und öffnen.
2. **Einrichten / prüfen** wählen. Die App erzeugt lokal eine eigene Arbeitskopie aus dem vorhandenen G Hub; die installierte App wird nicht verändert.
3. Für den Betrieb **Skyloong Bridge** in der macOS-Eingabeüberwachung freigeben. Diese Berechtigung erlaubt auch den Zugriff auf Eingabeereignisse.
4. **Starten** wählen und die Beleuchtung in **G Hub öffnen** einstellen. Die Brücke läuft bis **Stoppen** oder bis zum Beenden der App. Dann wird normales G Hub wiederhergestellt. Es gibt keine 20-Sekunden-Grenze mehr.

Die Modellauswahl im Fenster ist eine Vorschau. Die reale Tastatur wird anhand ihrer Modell- und Firmwarekennung erkannt. Deine GK87-Kombination ist praktisch geprüft; die weiteren 273 Profile sind experimentell. Das gemeinsame Format umfasst 132 LED-Plätze; darüber hinausgehende Zusatzbereiche werden noch nicht übertragen. Die bisherigen SDK-Lichtproben sind keine Bestätigung realer Spieleintegration. Reale Spieleffekte sind in dieser App-Fassung noch nicht abschließend geprüft; ebenso wenig Profilwechsel auf den experimentellen Modellen.

## Kompatibilität dieser Fassung

Apple Silicon; Build-Ziel macOS 13.5 oder neuer, bisher tatsächlich geprüft auf diesem Mac mit macOS 27.0.1. Die importierte G-Hub-Komponente ist auf die hier geprüfte Installation 2026.7.1011216 begrenzt. Andere Komponentenstände werden vor dem Umschalten abgewiesen. Eine Aussage über beliebige G-Hub-Versionen wird nicht gemacht.

Die Fassung 0.2 ist für dauerhaften Betrieb umgestellt. Der Dauerbetrieb wurde auf der vorhandenen GK87 über mehr als drei Minuten beobachtet. Stoppen, erneutes Starten und vollständiges Beenden wurden mit Rückschaltung auf normales G Hub geprüft. Sie ist lokal/ad-hoc signiert, nicht von Apple notarisiert. Das ZIP ist für kontrollierte Tests vorbereitet; die Voraussetzungen einer breiten öffentlichen Veröffentlichung sind damit noch nicht abgeschlossen.

Die App bringt keinen Logitech-Agent mit. Dieser wird ausschließlich aus der eigenen vorhandenen Installation übernommen. Die Quellen der öffentlichen Tastaturgrafiken wurden durch selbst erzeugte Layoutbilder ersetzt. Lizenzen der mitgelieferten Python- und Node-Laufzeiten liegen innerhalb der App unter `Contents/Resources/licenses`.

Eigene Einstellungen, die lokale Arbeitskopie und Protokolle liegen unter `~/Library/Application Support/Skyloong Bridge`. Beim Beenden des laufenden Betriebs wartet das Fenster auf die Rückschaltung. Ein kurzlebiger Wiederherstellungsmonitor beendet bei unerwartetem Ende des Arbeiters dessen Brückendienst und öffnet normales G Hub erneut; er installiert keinen Hintergrunddienst und keinen Autostart.

## Bestätigter Test vom 8. November 2026

Die kopierbare App wurde mit aktiver Eingabeüberwachung direkt geprüft: GK87 und G502 aktiv, eigenes 87-Tasten-Layout einschließlich Fn, anschließend 20 Sekunden physische Beleuchtung. Der Nutzer bestätigte Esc grün, Fn rot/pink und die übrigen Tasten türkis. Der Sender bestätigte Modus 1 und Exit 0; normales G Hub wurde wiederhergestellt. Dieser Nachweis gilt für die vorhandene GK87-Kombination und ersetzt keine Hardwareprüfung der 273 experimentellen Modelle.

## Änderung in 0.2

Starten, Stoppen und G Hub öffnen ersetzen die zeitbegrenzten Tests. Ein Lebenszeichen des Steuerprogramms schützt vor einem hängen gebliebenen Sender; eine feste maximale Laufzeit gibt es nicht mehr. Die Farbbeobachtung oben stammt aus 0.1. In 0.2 wurden zusätzlich Dauerbetrieb, Starten, Stoppen und vollständiges Beenden am vorhandenen Gerät geprüft.

## Dieses Paket

Enthalten sind die App mit dem ausgewählten Logo sowie der überarbeitete Tastaturkatalog. Version 0.2.1 ergänzt das App-Symbol; die Brückenfunktionen stammen aus 0.2. Die bereits geöffnete Testkopie wird durch dieses Paket nicht ersetzt.

Die App zuerst aus der ZIP entpacken und zum Beispiel nach Programme kopieren. Beim ersten Öffnen kann macOS eine Prüfung anzeigen. Diese Fassung ist nicht notarisiert. Bei einer Änderung oder einem Austausch der App kann macOS die Eingabeüberwachung erneut verlangen.
