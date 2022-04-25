Freie-Messenger.de schreibt selber:
https://www.freie-messenger.de/grundsaetzliches/ ([Archiviert am 2021-12-16](https://web.archive.org/web/20211216144331/https://www.freie-messenger.de/grundsaetzliches/))
> Auf diesen Seiten soll ein neutraler Ein- und Überblick zum Thema „Freie Messenger“ gegeben werden

Auf dieser Seite soll aufgezeigt werden, warum dies nicht der Fall ist.  
Dies ist meiner Meinung nach wichtig, da ein falscher Anschein für den Besucher erweckt wird.
Statt einen neutrale Anlaufstelle für Freie-Messenger zu bieten, ist die Webseite leider eigentlich nur eine XMPP Fanboy Seite.

Das bedeutet nicht, dass alle Argumente z.B. gegen properitären Messengern falsch sind! 
Im Gegenteil, oft sind die Argumente gut aufgearbeitet, aber die Schlussfolgerungen sind nicht mehr Neutral.

Die Mitarbeit und Kritik an diesem Repository ist gewünscht!

# Zentrale Kritikpunkte
## Internationaler Standard
Ein Argument, das immer wieder kommt sind Formulierungen wie:
> [internationalen Standard im Bereich Chat](https://www.freie-messenger.de/sys_xmpp/)

Beispiel:
https://www.freie-messenger.de/sys_matrix/gedanken/

Interessant ist in diesem Zusammenhang, dass Jabber/XMPP nicht als Wort erwähnt wird, aber verlinkt.

### Begriff
Aber was ist ein internationaler Standard überhaupt?
Schaut man sich mal die beiden Begriffe bei Wiktionary:
#### International
https://de.wiktionary.org/wiki/international  
[1] Nationen-übergreifend  
[2] mehrere Nationen betreffend, auf diese Bezug nehmend  

Nimmt man nur für sich den Begriff International bekommt man den Eindruck: Im Bezug auf Messenger ist jeder Messenger "international", der in mindestens 2 Ländern eingesetzt wird. Nicht unbedingt ein Ausschlusskriterium

#### Standard
https://de.wiktionary.org/wiki/Standard  
[1] etwas Geläufiges, Etabliertes, weithin Verbreitetes  
[2] Industrie: verbindliche Richtlinie, die sicherstellen soll, dass Produkte verschiedener Hersteller miteinander kompatibel beziehungsweise interoperabel sind.  

Hier ist es schon interessanter. Wenn man ehrlich ist, passt auf "Etablertes, weithin Verbreitetes" in den meisten Ländern leider am Besten WhatsApp. Nimmt man die "verbindliche Richtlinie" kann man eigentlich jegliches offene Protokoll oder sogar API als Standard bezeichnen.
Bei Matrix sind diese zum Beispiel hier zu finden:
https://spec.matrix.org/latest/

## standardisiertem Chat
Gern genannt wird auch "standardisiertem Chat"
Beispiel:
https://www.freie-messenger.de/sys_matrix/gedanken/#datenschutz-privatsphäre

Aber was ist das überhaupt?
### Begriff standardisiert
https://de.wiktionary.org/wiki/standardisiert
[1] durch einen Standard festgelegt

Es wird also wieder auf [Standard](#Standard) verwiesen.

Also auch in diesem Fall, eine Nebelkerze die alles heißen kann.

## Chat-Standard „XMPP“
Quelle:  
https://www.freie-messenger.de/sys_matrix/gedanken/#kein-internetstandard
Hier sei wieder auf [Standard](#Standard) verwiesen.
Warum man es für wichtig hält for XMPP "Chat Standard" zu stellen und warum man das bei den anderen Messengern nicht macht, ist wohl das Geheimnis des Autors.

## internationale Protokolle
Auch gerne wird von internationalen Protokoll gesprochen.  
Beispiel:  
https://www.freie-messenger.de/sys_matrix/gedanken/#unklare-positionierung  
[Die Definition von International wurde oben schon mal erläutert](#international)  

### Protokoll
https://de.wiktionary.org/wiki/Protokoll  
[4] Informatik, Telekommunikation: Satz von Befehlen, eine bestimmte Implementation, zur Steuerung der Kommunikation zwischen zwei Geräten, zum Beispiel zwischen zwei Computern

Also auch in diesem Fall, eine Nebelkerze die alles heißen kann.
# Kritik einzelner Seiten
Nachfolgend, getrennt in einer eigenen Datei, werden einzelne Seiten einzeln analysiert.  
[Matrix -> Gedanken](Matrix-Gedanken.md)

# DMA
Beispiele:
1. https://www.freie-messenger.de/begriffe/interoperabilitaet/dma/ ([Archiviert am 2021-12-16](https://web.archive.org/web/20211216144331/https://www.freie-messenger.de/grundsaetzliches/))
> Man kann an alle verantwortlichen Politiker also lediglich appellieren, hier ihrer öffentlichen Vorbildfunktion gerecht zu werden und über den DMA hinaus anbieterunabhängigen Chat auf der Basis von XMPP zumindest als Kontaktmöglichkeit anzubieten.

Weswegen wird ausgerechnet auf einem Seitenteil, der nichts mit XMPP selber zu tun hat, ein "Chat auf der Basis von XMPP" gefordert?
Warum nicht statt "Chat auf der Basis von XMPP" "Chat auf Basis eines freien Protokolls"?

# Kontakt
https://www.freie-messenger.de/kontakt/ ([Archiviert am 2022-04-25](https://web.archive.org/web/20220425094826/https://www.freie-messenger.de/kontakt/))
> nicht genug Vertrauen bezüglich dem Datenschutz (dezentrale Architektur der Chaträume).

Dabei funktioniert der Gruppenchat bei XMPP/Jabber ironischerweise GENAUSO wie Matrix mit dem Unterschied das nicht jeder Server ein Backup speichern MUSS.
Der Nutzer kontaktiert seinen Heimserver welcher wiederum die Daten vom Chatserver, wo der Chat gehostet wird, abholt.
Man stellt also fest, dass auch bei XMPP/Jabber die Daten quasi repliziert werden.
Es wird nur nich als Backup genutzt. Wenn der HomeServer allerdings möchte, könnte er die Daten genauso zwischenspeichern wie es bei Matrix getan wird. Somit ist die Art der Datenverarbeitung NICHT unterschiedlich. Trotzdem ist man vollständig abhängig von dem einem Hauptchat-Server. Fällt dieser aus, ist der Gruppenchat bei XMPP/Jabber verloren.  
(Kopiert von [Matrix-Gedanken.md#replizierung-von-chatr%C3%A4umen](Matrix-Gedanken.md#replizierung-von-chatr%C3%A4umen))

> Auch ist es schwieriger sicherzustellen, daß bößwillig eingestellte strafrechtliche Inhalte auf allen (ab dem Zeitpunkt der Veröffentlichung) beteiligten Servern tatsächlich gelöscht werden.

Für strafrechtliche Inhalte ist der Hoster, in diesem Fall also der Server selbst zuständig.  
Weswegen sich der Autor hier Gedanken darüber macht, was der Server mit seiner Löschanforderung macht, ist mir schleierhaft.

> Ich übernehme keine Verantwortung für geteilte Inhalte außerhalb der offiziellen Chaträume und auf von mir nicht gewählten Servern, da ich mögliche Folgen nicht abschätzen kann.

Hier würde mich interessieren welche Verantwortung der Autor den für geteilte Inhalte auf von ihm gewählten Servern übernimmt...
