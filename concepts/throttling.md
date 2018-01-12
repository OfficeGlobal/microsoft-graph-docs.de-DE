# <a name="microsoft-graph-throttling-guidance"></a>Leitfaden zu Einschränkungen in Microsoft Graph


Durch Einschränkungen wird die Anzahl der gleichzeitigen Aufrufe an einen Dienst begrenzt, um eine Überlastung von Ressourcen zu verhindern. Microsoft Graph ist für die Verarbeitung einer großen Menge von Anforderungen konzipiert. Wenn die Anzahl der Anforderungen jedoch zu hoch ist und zu einer Überlastung führen könnte, können Einschränkungen dazu beitragen, die optimale Leistung und Zuverlässigkeit des Microsoft Graph-Diensts aufrechtzuerhalten.

Einschränkungsgrenzwerte variieren je nach Szenario. Wenn Sie beispielsweise eine große Anzahl von Schreibvorgängen ausführen, ist eine Einschränkung wahrscheinlicher, als wenn nur Lesevorgänge ausgeführt werden.

## <a name="what-happens-when-throttling-occurs"></a>Was passiert im Fall einer Einschränkung?

Wenn ein Einschränkungsschwellenwert überschritten wird, begrenzt Microsoft Graph alle weiteren Anforderungen von diesem Client für einen bestimmten Zeitraum. Im Fall einer Einschränkung gibt Microsoft Graph den HTTP-Statuscode 429 (zu viele Anforderungen) zurück, und bei den Anforderungen tritt ein Fehler auf. Eine vorgeschlagene Wartezeit wird im Antwortheader der nicht ausgeführten Anforderung zurückgegeben. Das Einschränkungsverhalten kann vom Typ und der Anzahl der Anforderungen abhängen. Wenn z. B. eine große Menge von Anforderungen vorliegt, werden alle Anforderungstypen eingeschränkt. Die Schwellenwerte variieren je nach Anforderungstyp. Daher kann der Fall eintreten, dass Schreibvorgänge eingeschränkt werden, Lesevorgänge jedoch weiterhin zulässig sind. 

## <a name="common-throttling-scenarios"></a>Allgemeine Einschränkungsszenarien

Zu den häufigsten Ursachen für die Einschränkung von Clients zählen folgende:

* Eine große Anzahl von Anforderungen in allen Anwendungen in einem Mandanten.
* Eine große Anzahl von Anforderungen von einer bestimmten Anwendung in allen Mandanten.

## <a name="best-practices-to-handle-throttling"></a>Bewährte Methoden zum Behandeln der Einschränkungen

Im Folgenden finden Sie bewährte Methoden für den Umgang mit Einschränkungen:

* Verringern Sie die Anzahl der Vorgänge pro Anforderung.
* Verringern Sie die Häufigkeit von Aufrufen.
* Vermeiden Sie sofortige Wiederholungsversuche, da alle Anforderungen auf Ihre Nutzungsgrenzwerte angerechnet werden.

Wenn Sie Fehlerbehandlung implementieren, verwenden Sie den HTTP-Fehlercode 429 zur Erkennung von Einschränkungen. Im Antwortheader der Fehlerantwort ist das Feld *Retry-After* enthalten. Das Zurückhalten von Anforderungen unter Anwendung der *Retry-After*-Verzögerung ist die schnellste Methode der Wiederherstellung nach Auftreten einer Einschränkung, da Microsoft Graph den Ressourceneinsatz weiterhin protokolliert, während ein Client eingeschränkt ist.

1. Warten Sie die im Feld *Retry-After* angegebene Anzahl von Sekunden.
2. Wiederholen Sie die Anforderung.
3. Wenn die Anforderung erneut nicht ausgeführt und der Fehlercode 429 zurückgegeben wird, unterliegen Sie weiterhin einer Einschränkung. Wiederholen Sie die Anforderung unter Anwendung der empfohlenen Retry-After-Verzögerung so lange, bis die Anforderung erfolgreich ist.

Folgende Ressourcen bieten derzeit einen Retry-After-Header:
- [Benutzer](../api-reference/v1.0/resources/user.md)
- [Foto](../api-reference/v1.0/resources/profilephoto.md)
- [E-Mail](../api-reference/v1.0/resources/message.md)
- [Kalender (Benutzer und Gruppen)](../api-reference/v1.0/resources/event.md)
- [Kontakt](../api-reference/v1.0/resources/contact.md)
- [Anlage](../api-reference/v1.0/resources/attachment.md)
- [Gruppenunterhaltungen](../api-reference/v1.0/resources/conversation.md)
- [Personen und soziale Netzwerke](../api-reference/beta/resources/social_overview.md)
- [Drive (OneDrive)](../api-reference/v1.0/resources/drive.md)

Eine ausführlichere Erläuterung zum Thema Einschränkung in der Microsoft Cloud finden Sie unter [Throttling]((https://msdn.microsoft.com/de-DE/library/office/dn589798.aspx)).
