---
title: Verwenden Sie den Aktivitätsfeed REST-API
description: 'Der Aktivitätsfeed-API in Microsoft Graph können Sie eines Benutzers Actiity Geräte-und plattformübergreifend fortsetzen. Aktivität feed API-Anfragen werden ausgeführt, im Auftrag eines Benutzers über delegierten Berechtigungen und dem Benutzer die Berechtigung Aktivität, die mit entweder persönliche oder Arbeit und Schule Konten verwendet werden kann. '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: a229a5231894598fce0ff11f15926256987caa84
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971844"
---
# <a name="use-the-activity-feed-rest-api"></a>Verwenden Sie den Aktivitätsfeed REST-API

Der Aktivitätsfeed-API in Microsoft Graph können Sie eines Benutzers Actiity Geräte-und plattformübergreifend fortsetzen. Aktivität feed API-Anfragen werden ausgeführt, im Auftrag eines Benutzers über [Berechtigungen delegiert](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) und die [Benutzerberechtigungen für die Aktivität](/graph/permissions-reference), die mit entweder persönliche oder Arbeit und Schule Konten verwendet werden können. 

Die Benutzeraktivitäten werden von der Ressource [Aktivität](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/projectrome_activity) dargestellt und sind organisiert ein Feed zeitbasierte dargestellt durch die Auflistung mich / Aktivitäten. 
<!-- Add missing content.
Each activity represents a unique... 
-->
## <a name="what-makes-a-great-user-activity"></a>Was macht eine hervorragende Benutzeraktivität?

Die Benutzeraktivitäten nicht starten Sie apps – sie deep-Links in spezifischem Inhalt Ihrer App sind. Die Benutzeraktivitäten, die Sie erstellen können nicht nur in Ihrer eigenen app verwendet werden, aber auch im Cortana und Windows-Zeitachse angezeigt – gesteuerter Weitere app-Reengagement und erleichtert es für Ihre Benutzer weiterhin Ihre app für mehrere Geräte verwenden.  

### <a name="what-should-become-an-activity"></a>Was sollte eine Aktivität werden? 

Da jeder app unterscheidet, ist es zu verstehen, die beste Möglichkeit zum Zuordnen von Aktionen innerhalb der Anwendung auf die Benutzeraktivitäten jeder app-Entwickler. Beispielsweise Spiele möglicherweise eine Aktivität für jede Kampagne erstellen, Erstellen von apps Dokument möglicherweise eine Aktivität für jedes Dokument erstellen und Line-of-Business-apps möglicherweise eine Aktivität für jeden Workflow erstellen. 

Wenden Sie die folgenden Richtlinien, wie Sie in Ihrer app Activitites definieren:

**Aktionen aus:** Tragen Sie eine einzelne Aktivität für eine Gruppe von verwandten Benutzeraktionen. Wenn Ihre Anwendung bei einer Sequenz von verwandten Inhalten verwendet wird, ist es wahrscheinlich sinnvoll, um eine einzelne Aktivität für die gesamte Sitzung aufzuzeichnen.  

*Wiedergabeliste Szenarien:* Dies ist besonders relevant für Wiedergabelisten oder TV-Programmen – eine Aktivität einzelner Benutzer kann aktualisiert werden, um Ihren Fortschritt anzuzeigen. In diesem Fall müssen Sie eine einzelne Benutzeraktivität mit mehreren [Verlaufselemente](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/projectrome_historyitem) , die über mehrere Tage oder Wochen hinweg Zeiträume, in denen Engagements darstellt.  

**Aktionen aus:** Speichern von Benutzerdaten in die Cloud. Wenn Sie Aktivitäten Cross-Gerät unterstützen möchten, müssen Sie sicherstellen, dass der Inhalt erforderlich, um diese Aktivität reengage an einen Speicherort für die Cloud gespeichert ist. Angenommen, wenn Sie eine Aktivität eines Dokuments Bearbeitung jedes Mal veröffentlichen, sollte das Dokument in der Cloud im Gegensatz zur lokal auf dem Gerät des Benutzers gespeichert werden, um zwischen Geräten Reengagement zu aktivieren.  

**Nicht:** Erstellen Sie eine Benutzeraktivität für Aktionen, die Benutzer nicht benötigen, um zukünftig fortzusetzen. Wenn Ihre Anwendung verwendet wird, zum einfachen, einmaligen Vorgänge ausführen, die Status für Sie in der Zukunft verfolgen nicht beibehalten, müssen wahrscheinlich nicht Sie eine Benutzeraktivität zu schreiben. 

Um klar, obwohl die Benutzeraktivitäten in Windows Zeitachse angezeigt werden, Dies dient nicht als Tool Versioning – auswählen eine Aktivität dokumentbasierten sollte immer die neueste Version des Dokuments (einschließlich Änderungen, die von einem anderen Benutzer vorgenommen wurden.) anzeigen

**Nicht:** Erstellen Sie eine Benutzeraktivität für Aktionen, die von *anderen Benutzern*abgeschlossen. Wenn Ihnen jemand eine Nachricht oder @mentions der Benutzer in der app dem Benutzer sendet, sollte eine neue Aktivität nicht geschrieben werden. Diese Interaktionen sind besser versorgt, indem persönliche angezeigt werden Benachrichtigungen.  

*Szenarien der Zusammenarbeit:* Wenn mehrere Personen für die gleiche Aktivität (beispielsweise ein Word-Dokument) arbeiten, ist es, Fällen, wenn ein anderer Benutzer Änderungen an das Dokument vorgenommen hat, nachdem Sie zuletzt bearbeitet. In diesem Fall sollten app-Entwickler aktualisieren die visuellen Elemente in der Aktivität entsprechend dem Dokument geändert. Zu diesem Zweck möglicherweise die app die vorhandene Aktivität aktualisieren, ohne ein neues Historienelement erstellen. 

>**Hinweis:** Wenn Sie Aktivitäten für eine Webanwendung zu veröffentlichen, es ist wichtig, die beide enthalten eine `activationURL` und eine `fallbackURL` für jede Ihrer Aktivitäten. Die Aktivitäten werden den Benutzer wieder in Ihrer app gestartet erwartungsgemäß aus Microsoft Erfahrungen wie Windows Zeitachse. 

## <a name="app-interaction-patterns-and-user-activities"></a>App-Interaktionsmuster und die Benutzeraktivitäten 
Die Benutzeraktivitäten, die Sie erstellen variiert basierend auf der Interaktionsmuster Ihrer App. Während jeder app unterscheidet, werden die meisten in eine der folgenden Interaktionsmuster gehören: 

* **Dokumentbasierter apps** – Erstellen einer Aktivität pro Dokument mit mindestens einen Verlaufsdatensätze spiegeln Zeiträume, in denen verwenden. Es ist wichtig, die Aktivität Karte aktualisieren, wie das Dokument geändert wird. 
* **Media Wiedergabe apps** – Erstellen einer Aktivität pro logische Gruppierung von Inhalt wie eine Wiedergabeliste, Programm oder eigenständigen Inhalte. 
* **Spiele** – erstellen Sie eine Aktivität für jeden gespeicherte Spiel oder der Praxis. Wenn das Spiel nur eine einzelne Sequenz von Ebenen unterstützt, können Sie die gleiche Aktivität im Laufe der Zeit schreiben, obwohl sollten Sie die Visitenkarte zum Anzeigen Ihrer aktuellen Status oder Erfolge zu aktualisieren. 
* **Dienstprogramm apps** – liegt nothing innerhalb Ihrer app, die Benutzer fortsetzen möchten, sollten Sie Aktivitäten nicht veröffentlichen. Ein gutes Beispiel ist eine einfache einfachen Zweck erfüllende app wie Rechner. 
* **Branchen apps** – viele apps zum Verwalten von Workflows oder einfache Aufgaben vorhanden. Erstellen Sie eine Aktivität für jeden separate Workflow auf die Sie über Ihre app. Beispielsweise wäre jede Spesenabrechnung eine separate-Aktivität, da Sie möglicherweise klicken Sie auf diese Aktivität, um festzustellen, ob sie genehmigt wurde.

*Einige komplexe apps enthalten mehrere Interaktionsmuster. Möglicherweise möchten Sie führen die anderen Benutzer Aktivität Erstellung Mustern für die verschiedenen Szenarien, die von Ihrer app behandelt.*

<!-- Add content or remove H2.
## Common use cases 
-->

## <a name="next-steps"></a>Nächste Schritte

- Finden Sie unter die [Aktivität Ressource](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/projectrome_activity) , und definieren Sie Ihre app Aktivitäten, mit denen Benutzer wichtige Aufgaben fortsetzen.
- Machen Sie sich die [adaptive Karte Beispiele](https://adaptivecards.io/samples/) Beispiele für Ideen, um Ihre Aktivitäten **pop**stellen.  
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.

**Weitere Ideen suchen?** 

- Finden Sie unter [wie Microsoft guter Aktivitäten verwenden](https://channel9.msdn.com/events/Build/2017/B8108).
- Informationen Sie über [die Aktivität feed API und wählen Sie aus, wo unterbrochen](https://channel9.msdn.com/Events/Windows/Windows-Developer-Day-Fall-Creators-Update/WinDev011).
