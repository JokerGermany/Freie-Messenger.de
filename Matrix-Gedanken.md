In diesem Dokument wird die Webseite https://www.freie-messenger.de/sys_matrix/gedanken/ analysiert.

# [Vorwort](https://www.freie-messenger.de/sys_matrix/gedanken/#vorwort)
> Aber Matrix-Installationen können die dringend notwendige Interoperabilität unterstützen, wenn die vorhandene Schnittstelle zum [internationalen Standard im Bereich Chat](https://www.freie-messenger.de/sys_xmpp/) auch tatsächlich in der Praxis freigeschaltet wird und genutzt werden kann.

Der Begriff "internationaler Standard" wurde hier analysiert:  
https://github.com/JokerGermany/Freie-Messenger.de#internationaler-standard

Was mit "vorhandene Schnittstelle in der Praxis freigeschaltet wird" gemeint ist, erschließt sich leider nicht.

# [Datenschutz/Privatsphäre](https://www.freie-messenger.de/sys_matrix/gedanken/#datenschutz-privatsphäre)
> vermutlich ist das auch der Grund für [...] die Nicht-Nutzung der Schnittstelle zu standardisiertem Chat.

Eine Analyse zu "standardisiertem Chat" kann hier gefunden werden:
https://github.com/JokerGermany/Freie-Messenger.de#standardisiertem-chat

Zusammenfassend kann man sagen, dass sehr wohl eine "Schnittstelle zu standardisiertem Chat" genutzt wird.
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
Es wird nur nich als Backup genutzt. Wenn der HomeServer allerdings möchte, könnte er die Daten genauso zwischenspeichern wie es bei Matrix getan wird. Somit ist die Art der Datenverarbeitung NICHT unterschiedlich. Trotzdem ist man vollständig abhängig von dem einem Hauptchat-Server. Fällt dieser aus, ist der Gruppenchat bei XMPP/Jabber verloren. Datenschutz 

# [Kein Internetstandard](https://www.freie-messenger.de/sys_matrix/gedanken/#kein-internetstandard)
Das Matrix sehr wohl ein Internetstandard ist, habe ich schon hier erläutert:
https://github.com/JokerGermany/Freie-Messenger.de#internationaler-standard

Aber in diesem Text zeigt sich, weswegen der Autor glaubt, dass nur XMPP/Jabber ein internationaler Standard ist.
> Matrix ist kein durch die IETF (extern) geprüftes, legitimiertes oder standardisiertes Protokoll. 

Ja Matrix ist kein IETF-Standard, das ist korrekt. Meinen Informationen zurfolge ist langfristig tatsächlich der Plan, Matrix nach IETF zu standardisierem. Doch solange Matrix sich so schnell entwickelt wie es derzeit der Fall ist, möchte man lieber davon absehen, da schon jetzt die Spezifizierung eines neuen Matrix Specs sehr lange dauert und man befürchtet mit Einbindung der IETF die Spezifizierung noch längern dauern würde.

Interessant hierbei ist, dass der Autor meint XMPP ein "Chat-Standard" voranstellen zu müssen.
Mehr dazu hier:
https://github.com/JokerGermany/Freie-Messenger.de#chat-standard-xmpp

# [Monolithisches Protokoll](https://www.freie-messenger.de/sys_matrix/gedanken/#monolithisches-protokoll)
> Der Ansatz, auf Modularität zu verzichten um keine Fragmentierung zu bekommen funktionierte zu Beginn wunderbar. Allerdings ist Stand heute (2022) schon eine gewisse Fragmentierung festzustellen:
> - Es sind Matrix-Server mit unterschiedlichsten Versionen (extern) sowie verschiedenste Clients im Einsatz.
> - Auch ein Beispiel dafür sind die sich immer wieder veränderten Spezifikationen für Räume, für die derzeit 9 verschiedene Versionen (extern), da sich Raumspezifikationen (wie erwartet) fortentwickeln.
> Der angebliche Vorteil gegenüber dem Chatstandard XMPP von damals hat sich in Luft aufgelöst.

Es gibt immer, wenn es Verbesserungen oder Fehlerbehebungen gibt, neue Versionen.
Wenn man bei Matrix darauf achten, dass der HomeServer darauf bedacht ist seinen Server regelmäßig aktualisiert, dann bekommt man alle Features die Matrix bietet.
Bei XMPP hingegen muss man auch auf eine neue Server-Version achten (z.B. wegen Sicherheitsupdates) und darauf achten, dass der Server auch alle gewünschten Erweiterungen unterstützt. Eine neue Version des Servers bedeutet bei XMPP aber leider nicht, dass alle Features unterstützt wird.
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

>  [...] um für übergreifende Kommunikaition (=/= Interoperabilität) [...]

Wieso ist eine übergreifende Kommunikation keine Interoperabilität?  

Schaut man sich die Definition von Interoperabilität an:  
https://de.wiktionary.org/wiki/Interoperabilit%C3%A4t  
    1] Plural selten: Fähigkeit der Zusammenarbeit von verschiedenen Systemen, Techniken oder Organisationen; insbesondere möglichst nahtloses Zusammenarbeiten, um Informationen auf effiziente und verwertbare Art und Weise auszutauschen beziehungsweise den Benutzern zur Verfügung zu stellen  
    [2] Informatik, Plural selten: Konstellation, in der mehrere Programme dasselbe Protokoll beziehungsweise dieselben Protokolle oder Datenformate verwenden können__
    
¯\\\_(ツ)_/¯  Arbeiten nicht verschiedene Systeme zusammen, wenn über verschiedene Messenger hinweg sich ausgetauscht werden kann?

## [Rechtmäßigkeit und Zukunftssicherheit](https://www.freie-messenger.de/sys_matrix/gedanken/#rechtmäßigkeit-und-zukunftssicherheit)
> Matrix wirbt damit, viele Brücken zu geschlossenen Messengerdiensten wie beispielsweise Discord, Facebook Messenger, Instagram, Signal, Threema, WeChat und auch WhatsApp zu haben: https://matrix.org/bridges (extern)
>
> Dabei ist jedoch nicht klar, ob es mit den jeweiligen Eigentümern von zentralen Diensten (z.B. Facebook, Microsoft, Apple oder Google - um mal die großen zu nennen) überhaupt Verträge diesbezüglich gibt oder nicht. Denn andere Clients als den eigenen zu nutzen ist nicht erwünscht. Vielleicht lohnt sich hier ein Blick in die Allgemeinen Geschäftsbedingungen der jeweiligen Anbieter …!?

Und wenn man sich mit dem Thema beschäftigt, merkt man, dass es auch von der Art der Brücke abhängt.
z.B. sind Brücken bei denen die Bots genutzt werden, z.B. bei Discord und Telegram, völlig unkritisch.

## [Datenintegrität](https://www.freie-messenger.de/sys_matrix/gedanken/#datenintegrität)
> Seit März 2022 verändert die die Matrix-Brücke (Bifröst) Inhalte und übersetzt neuerdings XMPP URIs (Adressen)

Es ist schon faszinierend wie jemand, der immer wieder XMPP/Jabber versucht als DEN Standard hervorzuheben, das Prinzip von Diensten scheinbar nicht versteht.
Genauso wie es bei freien Messengern bei Homeservern nicht DEN Anbieter gibt, gibt es auch bei Brücken nicht die "Matrix-Brücke (Bifrost)".
Das von ihm angedeutete Feature macht eine der Brücken:  
https://aria-net.org/SitePages/Portal/Bridges.aspx  

Wer das nicht möchte kann z.B. auch die [Brücke von matrix.org](https://github.com/matrix-org/matrix-bifrost/wiki/Address-syntax) nutzen oder selber die Brücke hosten.

> Ganz abgesehen davon, daß Nachrichten von einer Brücke nicht inhaltlich geändert werden sollten: Warum erfolgt die Änderung der Links in Nachrichten ausschließlich in Richtung der Matrix-Syntax und in der anderen Richtung wird keine Matrix-Adresse „übersetzt“ - warum?

¯\\\_(ツ)_/¯ Vielleicht liegt es daran, weil die XMPP Community bisher kein Interesse hatte das Feature beizutragen?!?

> Hier werden Aufgeben, die ein Client übernehmen sollte (optionale Anpassung in der Anzeige von Inhalten) von der Brücke übernommen. Verknüpfungen (Links) beinhalten bewußt das zu berücksichtigende Protokoll, was viele Gründe haben kann - unter anderem Sicherheit.

Wer bestimmt eigentlich, wer welche Aufgabe hat?  
Vielleicht nutzt ein Matrix-Nutzer auch die aria-net.org Brücke WEGEN des Features.  
Es soll einige Nutzer geben, die dieses Feature haben wollen.

> Ein Entwickler der Bifröst-Bridge merkt dazu treffenderweise an, daß das lediglich meine Meinung ist:
Ich nehme an, das ist Ihre Meinung im Gegensatz zu anderen, die vielleicht tatsächlich XMPP benutzen und dafür entwickeln, z.B. https://github.com/matrix-org/matrix-bifrost/issues/308 (extern)

Ähm dort wird gar nichts angemerkt?!?

## [Unklare Positionierung](https://www.freie-messenger.de/sys_matrix/gedanken/#unklare-positionierung)
>Auf der einen Seite wird mit Brücken zwischen den Protokollen Matrix und XMPP geworben - auf der anderen Seite wird XMPP überhaupt nicht bei den Matrix-Brücken (extern) aufgeführt bzw. mit keinem Wort erwähnt. Zumindest nicht auf dieser wichtigen Seite.
>
>Um „XMPP“ zu finden, muß man unter „libpurple“ schauen, wo widerum auf „matrix-bifrost“ verwisen und der Hinweis “General purpose puppeting bridges using libpurple and other backends. This bridge is in very active development currently and intended mainly for experimentation and evaluation purposes.” gegeben wird. Erst auf der dort verlinkten Github-Seite steht bzw. findet man dann „XMPP“.

Vielleicht sollte man erst einmal an der richtigen Stelle einen Verbesserungsvorschlag anbringen und wenn dann nichts passiert es anmeckern...  
[Ich habe das mal gemacht](https://github.com/matrix-org/matrix.org/issues/1311)  
Aber vielleicht will man auch gar nicht, dass sich etwas verbessert...

> Es wird also teilweise mit Brücken zu XMPP geworben - aber Interoperabilität auf der Basis von internationalen Protokollen wird nicht aktiv verfolgt.

Ich gehe mal davon aus, dass statt XMPP dort eigentlich Matrix rein sollte.
Doch es wird die Interoperablität zu vielen internationalen Protokollen verfolgt.
Was Internationale Protokolle sind, wurde hier analysiert:
https://github.com/JokerGermany/Freie-Messenger.de#internationalen-protokolle
Nämlich jeglichen der gebridgen Messenger kann man als interantionales Protokoll bezeichnen.

> Standard XMPP

Schon wieder meint der Autor XMPP ein "Standard" voranstellen zu müssen...

>internationalen Standard XMPP

Jetzt ist es sogar schon ein internationaler Standard. WoW!


# [Gründe für Matrix](https://www.freie-messenger.de/sys_matrix/gedanken/#gründe-für-matrix)
> Und: Die damals bemängelte Fragmentierung findet nun auch schon bei Matrixstatt, so wie das beidezentralen Systemen ganz natürlich ist.

Es ist ein Unterschied, ob die Fragmentierung nur auf Versionsbasis, oder auf Versions UND Featurebasis existiert.
Aber das wurde ja schon bei [#Monolithisches Protokoll](#monolithisches-protokoll) erläutert.

# [Zusammenfassung / Fazit](https://www.freie-messenger.de/sys_matrix/gedanken/#zusammenfassung-fazit)
> Das Standardprotokoll, das WhatsApp tatsächlich mittelfristig in der Breite ersetzen kann, ist aus heutiger Sicht und mit diesem Hintergrundwissen nicht das Protokoll Matrix sondern anbieterunabhängier Chat (auf der Basis des Standards XMPP).

Hier wird es jetzt ganz wild. Anbieterunabhängiger Chat, was soll das sein? Ist Matrix nicht anbieterunabhäng?
Welches Hintergrundwissen ist gemeint?

> Standard XMPP

Schon wieder meint der Autor XMPP ein "Standard" voranstellen zu müssen...

> Nicht durch eine öffentliche Föderation von Matrix-Servern sondern durch Aktivierung und Nutzung der wichtigen Brücke zu standarsisiertem Chat - also durch das Einhalten von internationalen Standards - wird tatsächliche Interoperabilität unterstützt und ermöglicht.

Eine Analyse zu "standardisiertem Chat" kann hier gefunden werden:
https://github.com/JokerGermany/Freie-Messenger.de#standardisiertem-chat
Eine Analyse zu "standardisiertem Chat" kann hier gefunden werden:
https://github.com/JokerGermany/Freie-Messenger.de#internationaler-standard

Wer entscheidet eigentliche welche Brücke wichtig und welche unwichtig ist?  
¯\\\_(ツ)_/¯  Also Matrix hat Brücken zu vielen standardisierten Chats und internationalen Standards.


