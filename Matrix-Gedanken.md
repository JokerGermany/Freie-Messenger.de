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
Es wird nur nich als Backup genutzt. Wenn der HomeServer allerdings möchte, könnte er die Daten genauso zwischenspeichern wie es bei Matrix getan wird. Somit ist die Art der Datenverarbeitung NICHT unterschiedlich. Trotzdem ist man vollständig abhängig von dem einem Hautpchat-Server. Fällt dieser aus, ist der Gruppenchat bei XMPP/Jabber verloren. Datenschutz 

# [Kein Internetstandard](https://www.freie-messenger.de/sys_matrix/gedanken/#kein-internetstandard)
Das Matrix sehr wohl ein Internetstandard ist, habe ich schon hier erläutert:
https://github.com/JokerGermany/Freie-Messenger.de#internationaler-standard

Aber in diesem Text zeigt sich, weswegen der Autor glaubt, dass nur XMPP/Jabber ein internationaler Standard ist.
> Matrix ist kein durch die IETF (extern) geprüftes, legitimiertes oder standardisiertes Protokoll. 

Ja Matrix ist kein IETF-Standard, das ist korrekt. Meinen Informationen zurfolge ist langfristig tatsächlich der Plan, Matrix nach IETF zu standardisierem. Doch solange Matrix sich so schnell entwickelt wie es derzeit der Fall ist, möchte man lieber davon absehen, da schon jetzt die Spezifizierung eines neuen Matrix Specs sehr lange dauert und mit Einbindung der IETF noch längern dauern würde.

Interessant hierbei ist, dass der Autor meint XMPP ein "Chat-Standard" voranstellen zu müssen.
Mehr dazu hier:
https://github.com/JokerGermany/Freie-Messenger.de#chat-standard-xmpp

# [Monolithisches Protokoll](https://www.freie-messenger.de/sys_matrix/gedanken/#monolithisches-protokoll)
> Der Ansatz, auf Modularität zu verzichten um keine Fragmentierung zu bekommen funktionierte zu Beginn wunderbar. Allerdings ist Stand heute (2022) schon eine gewisse Fragmentierung festzustellen:
> - Es sind Matrix-Server mit unterschiedlichsten Versionen (extern) sowie verschiedenste Clients im Einsatz.
> - Auch ein Beispiel dafür sind die sich immer wieder veränderten Spezifikationen für Räume, für die derzeit 9 verschiedene Versionen (extern), da sich Raumspezifikationen (wie erwartet) fortentwickeln.
> Der angebliche Vorteil gegenüber dem Chatstandard XMPP von damals hat sich in Luft aufgelöst.

Es gibt immer wenn es Verbesserungen oder Fehlerbehebungen gibt neue Versionen.
Wenn man bei Matrix darauf achten, dass der HomeServer darauf bedacht ist seinen Server regelmäßig aktualisiert, dann bekommt man alle Features die Matrix bietet.
Bei XMPP hingegen muss man auch auf eine neue Version achten und darauf achten, dass der Server auch alle gewünschten Erweiterungen unterstützt. Eine neue Version des Servers bedeutet bei XMPP aber leider nicht, dass alle Features unterstützt wird.
Den Ist-Zustand kann man bei XMPP hier testen:  
https://compliance.conversations.im/tests/
Ob ein gewünschtes neues XEP (So heißen die Erweiterungen bei XMPP) unterstützt wird, steht allerdings in den Sternen.
Deswegen hat man sich bei Matrix für ein Monolithisches Protokoll entschieden und dieser Vorteil hat sich defintiv NICHT in Luft aufgelöst.

# Flexibilität des Protokolls
> Für moderne IM-Anforderungen ist das Matrix-Protokoll geeignet (es wäre ja auch schlimm, wenn nicht) - für andere Dinge jedoch wie das Internet der Dinge (IoT) oder neue Entwicklungen nicht wirklich. Also braucht es dafür separate Lösungen, was schade ist.

Es ist schon spannend wie unterschiedlich Einschätzungen sein können.
Hier mal ein paar Anwendungszwecke abseits der "modernen IM Anforderungen":
- [Filestorage](https://fosdem.org/2022/schedule/event/matrix_filesystem/)
- [CMS](https://github.com/medienhaus/medienhaus-cms)
- [Thirdroom](https://github.com/matrix-org/thirdroom) - Eine Konkurrenz zum Metaverse von Meta
- [MMO Browser Game](https://fosdem.org/2022/schedule/event/matrix_mmo_browser/)
- [Datei und Webseiten Kommentare](https://fosdem.org/2022/schedule/event/matrix_decentralized_annotations/)
- [Kommentare auf Webseiten](https://cactus.chat/)
- [Blog](https://evolved.systems/hosting-a-blog-on-matrix/)
- [collaborative Whiteboard](https://github.com/toger5/TheBoard)
- [social media](https://minestrix.henri2h.fr/)
- [Event-Management](https://gatho.party/)
 
# [Föderation & Interoperabilität](https://www.freie-messenger.de/sys_matrix/gedanken/#föderation-interoperabilität)
Ja es sollte viel mehr Föderation genutzt werden.
Aus meiner Beruflichen Laufbahn sind mir allerdings auch zahlreiche XMPP Server bekannt, die nicht föderieren.
Dort gab es sogar innerhalb verschiedener Standorter von ein und derselben Firma verschiedene XMPP Server die noch nicht mal innerhalb der Firma föderiert haben.
Hier wird übrigens erklärt, das XMPP auch im militärischen Einsatz eingesetzt wird und fragt sich warum dort die nicht vorhandene Föderation kein Thema ist...  
https://www.freie-messenger.de/sys_xmpp/#militärischer-einsatz-nato

# [Ressourcenbedarf](https://www.freie-messenger.de/sys_matrix/gedanken/#ressourcenbedarf)
> Die einfachste Lösung für das Ressourcenproblem, das seitens Matrix derzeit mit „conduit“ (Beta-Status) (extern) versucht wird zu verbessern, ist die Einschränkung bei der Föderation. Um im Rahmen der vorhandenen technischen Möglichkeiten zu bleiben, werden deshalb manche Matrix-Instanzen nicht öffentlich betrieben.

Conduit befindet sich nach wie vor im Beta Status. Die Information, dass Conduit keine Föderation kann, ist veraltet. Wenn man einen neuen Server entwickelt ist es teil des Entwicklungsprozesses Features nach und nach zu implementieren. Sind alle Features stabil implementiert endet auch die Beta Phase.
Es gibt übrigens auch schon verschiedene Nachfolger von Conduit in der Entwicklung, die nochmals Ressourcenschonender sind.

# [Verschlüsselung](https://www.freie-messenger.de/sys_matrix/gedanken/#verschlüsselung)
> Trotzdem wird immer behauptet, bei Matrix wäre automatisch alles verschlüsselt. 

Schade das ohne Quellen einfach etwas behauptet wird. Wo wird etwas "immer behauptet"?
Bei Matrix sind 1zu1 Räume automatisch verschlüsselt. z.B. in Element kann man dies nur sehr sehr umständlich umgehen.
Erstellt man in Element private Räume ist eine Verschlüsselung ebenfalls vorausgewählt und muss aktiv abgewählt werden.
Nur in öffentlichen Räumen muss aktiv die Verschlüsselung eingeschaltet werden, falls gewünscht.

# [Electron](https://www.freie-messenger.de/sys_matrix/gedanken/#electron)
> Es gibt keinen nativen Element-Desktopclient für Windows oder Linux.

Das ist falsch.
Für z.b. Linux kann ich [Fluffychat](https://fluffychat.im/) empfehlen.
Es gibt wohl auch einen Windows-Client, dieser wird aber offiziell nicht unterstützt.

# [Brücken](https://www.freie-messenger.de/sys_matrix/gedanken/#brücken)
## [Grundsätzliches](https://www.freie-messenger.de/sys_matrix/gedanken/#grundsätzliches)
> 1. Die Matrix-Bifröst-Brücke ist bisher noch nicht Über den Experimentalstatus (extern) hinaus gekommen („This bridge is in very active development currently and intended mainly for experimentation and evaluation purposes.“) - offensichtlich wird in anderen Brücken mehr Wertschöfpungspotential gesehen.

Ich finde es schade, dass die XMPP-Community scheinbar keinerlei Intentionen zeigt, daran zu arbeiten es zu ändern.  
¯\\\_(ツ)_/¯ Es ist einfach über etwas zu meckern, aber daran mitzuwirken, dass sich etwas ändert ist scheinbar nicht gewünscht...
Eine Brücke ist keine Einbahnstraße...

> 2. Austausch nur über Matrix
Matrix-Brücken sind lediglich Brücken von/zu Matrix - ein direkter Austausch zwischen anderen Systemen ist damit nicht möglich. Folglich sind Brücken also Teil des Interoperabilitätsproblems und nicht der Problemlöser (das Selbe gilt auch für Brücken (“Transporte”), die es bei XMPP gibt!).

Wenn ich eine Straße von Nürnberg nach Fürth baue, erwartet man dann auch, dass ich auf dieser Straße nach Hamburg fahren kann?  
Weil ich auf der Straße nicht nach Hamburg fahren kann, ist dies Teil des Problems, warum ich nicht nach Hamburg fahren kann?
