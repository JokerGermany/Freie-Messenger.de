In diesem Dokument wird die Webseite https://www.freie-messenger.de/sys_matrix/gedanken/ analysiert.
# [Vorwort](https://www.freie-messenger.de/sys_matrix/gedanken/#vorwort)
> Aber Matrix-Installationen können die dringend notwendige Interoperabilität unterstützen, wenn die vorhandene Schnittstelle zum [internationalen Standard im Bereich Chat](https://www.freie-messenger.de/sys_xmpp/) auch tatsächlich in der Praxis freigeschaltet wird und genutzt werden kann.

Der Begriff "internationaler Standard" mehrdeutig ist, wurde hier erläutert:  
https://github.com/JokerGermany/Freie-Messenger.de#internationaler-standard

Was mit "vorhandene Schnittstelle in der Praxis freigeschaltet wird" gemeint ist, erschließt sich leider nicht.

# [Datenschutz/Privatsphäre](https://www.freie-messenger.de/sys_matrix/gedanken/#datenschutz-privatsphäre)
> vermutlich ist das auch der Grund für [...] die Nicht-Nutzung der Schnittstelle zu standardisiertem Chat.
## standardisiertem Chat
Eine Analyse zu "standardisiertem Chat" kann hier gefunden werden:
https://github.com/JokerGermany/Freie-Messenger.de#standardisiertem-chat

Zusammenfassend kann man sagen, dass sehr wohl eine "Schnittstell zu standardisiertem Chat" genutzt wird.
https://spec.matrix.org/latest/


## volle Kontrolle über ihre Kommunikation
>Es wird auch nicht damit geworben, daß Nutzer die volle Kontrolle über ihre Kommunikation behalten - statt dessen ist der Vorteil lt. Matrix:
> > There is no single point of control or failure in a Matrix conversation which spans multiple servers: the act of communication with someone elsewhere in Matrix shares ownership of the conversation equally with them.

Hier würde mich interessieren welche Chat-Messenger die "volle Kontrolle über ihre Kommunikation" gewährleisten kann...

## Datenschutzbedenken
> Merkwürdigerweise wird genau der Punkt Datenschutz als Argument aufgeführt, um geschlossene Matrix-Instanzen zu rechtfertigen und um keine Schnittstelle nach außen (=Interoperabilität) haben zu müssen. Aus einer E-Mail auf Landesebene:
> > …, was von uns aus datenschutzrechtlichen Gründen ausdrücklich nicht gewünscht ist.
> Auf die Frage nach einer Konkretisierung der angeblichen Datenschutzbedenken bekommt man jedoch trotz gezielter Nachfragen von keiner Firma und keiner Behörde eine Auskunft. Es kann nicht begründet werden.

Ohne konkret zu erklären, was mit "Schnittstelle nach außen" gemeint wird, wird hier versucht Zweifel zu schüren.
Dabei ist der Grund dafür, warum man Föderation lieber nicht erlaubt, mit Datenschutzbedenken gut erklärt.
Man hat Sorge das Mitarbeiter versentlich Daten in die Öffentlichkeit verschicken.

Was dies allerdings mit Matrix an sich zu tun hat, bleibt wohl das Geheimnis des Autors der Webseite.

## Replizierung von Chaträumen
> Das Grundkonzept von Matrix ist die Replizierung von Chaträumen (auch 1:1-Chats) auf alle am jeweiligen Chat beteiligten Server. Und genau das führt nicht nur zu höherem Ressourcenverbrauch (s.u.), sondern ist auch bei öffentlicher Föderation datenschutztechnisch problematisch. Vermutlich müsste der Auftrag zur Datenverarbeitung jeweils erweitert werden, was praktisch kaum möglich ist. Eine Lösung hier ist nur, bei der Kommunikation mit anderen Systemen auf standardisierte Schnittstellen zurückzugreifen, die keine Replizierung von Datenbanken erfordern.

Hier versucht der Autor mit standartisiertem Schnittstellen ( [Analyse zu "standardisiertem Chat"](README.md#standardisiertem-chat) ) auf XMPP/Jabber hinzuweisen.
Dabei funktioniert der Gruppenchat bei XMPP/Jabber ironischerweise GENAUSO wie Matrix mit dem Unterschied das nicht jeder Server ein Backup speichern MUSS.
Der Nutzer kontaktiert seinen Heimserver welcher wiederum die Daten vom Chatserver, wo der Chat gehostet wird, abholt.
Man stellt also fest, dass auch bei XMPP/Jabber die Daten quasi repliziert werden.
Es wird nur nich als Backup genutzt. Wenn der HomeServer allerdings möchte, könnte er die Daten genauso zwischenspeichern wie es bei Matrix getan wird. Somit ist die Art der Datenverarbeitung NICHT unterschiedlich. Trotzdem ist man vollständig abhängig von dem einem Hautpchat-Server. Fällt dieser aus, ist der Gruppenchat bei XMPP/Jabber verloren.
