---
title: Übersicht über Informationen aus sozialen Netzwerken und deren Analyse in Microsoft Graph
description: 'Die mehreren hundert Millionen Benutzer von Microsoft 365-Clouddiensten sind Teil des Herzstücks von Microsoft Graph. Die Daten der Benutzer werden sorgfältig verwaltet, geschützt und mit der entsprechenden Berechtigung durch die Dienste von Microsoft Graph zur Verfügung gestellt, um die Produktivität und Kreativität in Unternehmen zu fördern. Benutzerdaten sind in Microsoft Graph zahlreich vorhanden, aber die Daten, die sich aus den sozialen Interaktionen des Benutzers ableiten, sind besonders interessant. Sie bieten intelligente Einblicke, die Antworten auf Fragen wie die folgenden bieten:'
ms.openlocfilehash: 518d7cb773ae32199c38f2eb8459d785b2750f18
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092276"
---
# <a name="overview-of-social-intelligence-and-analytics-in-microsoft-graph"></a>Übersicht über Informationen aus sozialen Netzwerken und deren Analyse in Microsoft Graph

Die mehreren hundert Millionen Benutzer von Microsoft 365-Clouddiensten sind Teil des Herzstücks von Microsoft Graph. Die Daten der Benutzer werden sorgfältig verwaltet, geschützt und mit der entsprechenden Berechtigung durch die Dienste von Microsoft Graph zur Verfügung gestellt, um die Produktivität und Kreativität in Unternehmen zu fördern. Benutzerdaten sind in Microsoft Graph zahlreich vorhanden, aber die Daten, die sich aus den sozialen Interaktionen des Benutzers ableiten, sind besonders interessant. Sie bieten intelligente Einblicke, die Antworten auf Fragen wie die folgenden bieten:

- „An wen sollte sich der Benutzer wenden, um Informationen zu diesem Thema zu erhalten?“
- „Welche Dokumente sind für diese Person am interessantesten?“

Sie können die Personen-API und die Einblicke API in Microsoft Graph nutzen, um intelligentere Apps zu erstellen, die auf die für einen Benutzer relevanten Personen bzw. Dokumente zugreifen.

Die Personen-API gibt Personen geordnet nach Relevanz für einen Benutzer zurück, basierend auf den Kontakten, sozialen Netzwerken, dem Organisationsverzeichnis und den letzten Kommunikationen per E-Mail und Skype des Benutzers. Dies ist besonders nützlich, wenn Personen ausgewählt werde müssen.

Die Einblicke-API verwendet erweiterte Analysemethoden und maschinelles Lernen, um dem Benutzer die relevantesten Dateien bereitzustellen, die er für seine tägliche Arbeit benötigt. Die API unterstützt die bekannten Office 365-Oberflächen, einschließlich Office Delve, die SharePoint-Startseite, die Discover-Ansicht in OneDrive for Business und Outlook im Web.

![Die Personen- und Einblicke-API geben für einen Benutzer relevante Personen und Dokumente zurück](images/social-intel-concept-overview-data.png)

## <a name="why-integrate-with-people-data"></a>Vorteile der Integration mit Personendaten

Die Personen-API gibt Daten einer einzelnen Entität zurück: [person](/graph/api/resources/person?view=graph-rest-1.0). Diese enthält die für die heute Geschäftsumgebung typischen Daten einer Einzelperson. Diese **Personendaten** werden aufgrund ihrer _Relevanz_ in Bezug auf einen Microsoft Graph-Benutzer erst besonders nützlich. Die Relevanz wird durch eine Relevanzbewertung für jede Person ausgedrückt. Diese wird auf Grundlage der Kommunikations- und Zusammenarbeitsmuster sowie der Geschäftsbeziehungen des Benutzers berechnet. Für diese _Relevanzdaten_ gibt es drei wichtige Arten der Anwendung.

### <a name="browse-people-by-relevance"></a>Suchen von Personen nach Relevanz

Sie können Personen durchsuchen, die mit dem angemeldeten Benutzer oder einem anderem Benutzer im Unternehmen des angemeldeten Benutzers in Beziehung stehen, vorausgesetzt, Sie verfügen über die entsprechende [Autorisierung](people-example.md#authorization). Sie erhalten eine Sammlung von **person**-Objekten, die nach Relevanz geordnet ist. Sie können die Sammlung der **person**-Objekte, die in der Antwort zurückgegeben wird, indem Sie die Abfrageparameter `top`, `skip`, `orderby`, `select` und `filter` angeben, noch weiter [anpassen](people-example.md#browse-people).

### <a name="fuzzy-searches-based-on-people-criteria"></a>Fuzzysuche basierend auf Personenkriterien

Mit der Personen-API können Sie nach Personen suchen, die für den angemeldeten Benutzer relevant sind, vorausgesetzt, dass Ihre App die Berechtigung durch diesen Benutzer erhalten hat. (Erfahren Sie mehr über [Personenberechtigungen](permissions-reference.md#people-permissions).)

Fuzzysuchen geben Ergebnisse basierend auf einer genauen Übereinstimmung sowie auf Ableitungen zur Absicht der Suche zurück. Zur Veranschaulichung gibt das folgende Beispiel **person**-Objekte zurück, die für den angemeldeten Benutzer relevant sind, dessen Name _oder E-Mail-Adresse_ ein Wort enthält, das mit „j“ beginnt.

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search=j
```

### <a name="fuzzy-searches-based-on-topic-criteria"></a>Fuzzysuche basierend auf Themenkriterien

Mit der Personen-API können Sie Suchvorgänge nach Personen durchführen, die für den angemeldeten Benutzer relevant sind und Interesse an der Kommunikation mit dem Benutzer über bestimmte „Themen“ gezeigt haben. „Themen“ in diesem Sinne sind einfach Wörter, die in der E-Mail-Kommunikation von den Benutzern am häufigsten verwendet wurden. Microsoft extrahiert diese Wörter und erstellt ohne deren Kontext einen Index für diese Daten, um die Fuzzysuche zu erleichtern.

Das folgende Beispiel veranschaulicht die Rückschlüsse über den Zweck der Suche zum englischen Begriff „Beetle“:

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search="topic:beetle" 
```

Eine Fuzzysuche im Index der Themendaten gibt Instanzen zurück, die sich auf das Insekt beziehen (zu Deutsch „Käfer“), auf den Volkswagen-Käfer (englisch „Beetle“), auf die Musikgruppe „Beatles“ und andere Definitionen.


## <a name="why-integrate-with-document-based-insights-preview"></a>Vorteile von dokumentbasierten Einblicken (Vorschau)

### <a name="use-intelligence-to-improve-collaboration"></a>Nutzen von Informationen zur Verbesserung der Zusammenarbeit

An einem typischen Arbeitstag verwenden Benutzer häufig große Mengen an Informationen, die in verschiedenen Dokumenten gespeichert sind, und arbeiten auf verschiedene Weise mit anderen Personen zusammen. Es ist wichtig, dass die Benutzer immer die richtigen Informationen zum richtigen Zeitpunkt finden können.

Sie können die Einblicke-API verwenden, die APIs für [trending](/graph/api/resources/insights-trending?view=graph-rest-beta), [shared](/graph/api/resources/insights-shared?view=graph-rest-beta) und [used](/graph/api/resources/insights-used?view=graph-rest-beta) beinhaltet. Hiermit können Sie Dateien aus Office 365 basierend auf dem aktuellen Kontext und den Anforderungen der Benutzer abrufen, sodass die Produktivität der Benutzer gesteigert und die Zusammenarbeit im Unternehmen gefördert wird.

Sie können die Ergebnisse der Einblicke-API auf einfache Weise in der App darstellen. Jedes Ergebnis bietet eine Reihe von allgemeinen Visualisierungseigenschaften, wie z. B. eine Vorschaubild-URL oder Vorschautext.

### <a name="make-relevant-content-visible"></a>Sichtbarmachen relevanter Inhalte

In Office 365 verwendet Delve den _trending_-Einblick, um Benutzer dabei zu unterstützen, die Dokumente zu finden, die für sie gerade von besonderem Interesse sind. Siehe Abbildung 1.

Sie können die [trending](/graph/api/resources/insights-trending?view=graph-rest-beta)-Entität programmgesteuert in der Einblicke-API verwenden, um den Kunden Ihrer App eine ähnliche Oberfläche bereitzustellen. Verwenden Sie die **trending**-Entität, um eine Verbindung zu Dokumenten herzustellen, die für den Benutzer einen Trend darstellen und relevant sind. Beim [Auflisten von Trenddokumenten](/graph/api/insights-list-trending?view=graph-rest-beta) werden die Dateien zurückgegeben, die in OneDrive oder auf SharePoint-Teamwebsites gespeichert sind, und zwar sortiert nach Relevanz mit den wichtigsten am Anfang. 

**Abbildung 1: Delve in Office 365 zeigt häufig verwendete Dokumente für einen Benutzer an**

![Screenshot von Delve in Office 365 mit häufig verwendeten Dokumenten für einen Benutzer](images/delve-concept.png)

### <a name="allow-users-to-collaborate-and-get-back-to-work"></a>Bessere Zusammenarbeit der Benutzer und Erledigung der eigentlichen Arbeit

Die neuen Personenkarten in Office 365 nutzen die _Verwendet_- und _Freigegeben_-Einblicke, um Personen und Wissen miteinander zu verbinden. Die Personenkarte identifiziert relevante Dokumente zu einer Person und zeigt sie anzeigt. Benutzer können Personenkarten überall in der Produktsuite sehen, wie z. B. in Outlook im Web. Siehe Abbildung 2.

Die Einblicke-API bietet mit den Entitäten [used](/graph/api/resources/insights-used?view=graph-rest-beta) und [shared](/graph/api/resources/insights-shared?view=graph-rest-beta) ähnliche Funktionen. Sie geben zurück, was sich ein Benutzer angesehen oder woran er gearbeitet hat, oder was Kollegen mit dem Benutzer zuletzt in Office 365 geteilt haben.

**Abbildung 2: Outlook im Web mit einer Personenkarte fpr einen Benutzer**

![Screenshot einer Personenkarte für einen Benutzer in Outlook im Web mit den zuletzt verwendeten Dateien](images/peoplecard-concept.png)

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

- [Personen-API in Microsoft Graph v1.0](/graph/api/resources/social-overview?view=graph-rest-1.0)
- [API für Informationen aus sozialen Netzwerken und deren Analyse in Microsoft Graph Beta](/graph/api/resources/social-overview?view=graph-rest-beta)

## <a name="next-steps"></a>Nächste Schritte

* Verwenden Sie den [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer), um den Personen- und Einblicke APIs mit Ihren eigenen Dateien zu testen. Melden Sie sich an und wählen Sie in der linken Spalte **Mehr Beispiele anzeigen**. Aktivieren Sie mithilfe des Menüs **Personen** und **Einblicke (Beta)**.
* Weitere Informationen zur [Personen-API](people-example.md) und zur [person](/graph/api/resources/person?view=graph-rest-1.0)-Entität.
* Erste Schritte mit der Einblicke-API finden Sie unter [Verwenden der Einblicke-API](/graph/api/resources/insights?view=graph-rest-beta).
