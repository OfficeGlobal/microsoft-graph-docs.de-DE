# <a name="microsoft-graph-security-data-flow"></a>Microsoft Graph Security-Datenfluss

Die Microsoft Graph Security-API bindet Anforderungen an alle Anbieter im Microsoft Graph Security-Ökosystem ein. Dies basiert auf der Zustimmung des Sicherheitsanbieters, die von der Anwendung bereitgestellt wird, wie in der folgenden Abbildung dargestellt. Der Zustimmungsworkflow gilt nur für Nicht-Microsoft-Anbieter.

![security_dataflow_1.PNG](./images/security_dataflow_1.png)

Es folgt eine Beschreibung für den Ablauf:

1. Der Anwendungsbenutzer meldet sich bei der Anbieteranwendung an, um das Einverständnisformular des Anbieters anzuzeigen. Dieses Einverständnisformular oder UI ist Eigentum des Anbieters und gilt für Nicht-Microsoft-Anbieter, nur um ausdrückliche Zustimmung von ihren Kunden zu erhalten, um Anforderungen an Microsoft Graph Security API zu senden.
2. Die Client Zustimmung wird auf der Anbieterseite gespeichert.
3. Der Anbieterzustimmungsdienst ruft die Microsoft Graph-Sicherheits-API auf, um die Zustimmungsgenehmigung für den jeweiligen Kunden zu informieren.
4. Die Anwendung sendet eine Anforderung an die Microsoft Graph-Sicherheits- API.
5. Die Microsoft Graph-Sicherheits-API sucht nach den Einwilligungsinformationen für diesen Kunden, die verschiedenen Anbietern zugeordnet sind.
6. Die Microsoft Graph-Sicherheits-API ruft alle Anbieter auf, bei denen der Kunde die ausdrückliche Zustimmung über die Zustimmung des Providers gegeben hat.
7. Die Antwort wird von allen zugelassenen Anbietern für diesen Client zurückgegeben.
8. Die Resultset-Antwort wird an die Anwendung zurückgegeben.
9. Wenn der Kunde einem Anbieter nicht zugestimmt hat, werden keine Ergebnisse von diesen Anbietern in die Antwort aufgenommen.
