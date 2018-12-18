---
title: Übersicht über Microsoft Graph Data Connect (Vorschau)
description: Microsoft Graph enthält umfassende Informationen zu Mitarbeitern und ihrem Arbeitsplatz, einschließlich Informationen dazu, wie Mitarbeiter arbeiten und sie kommunizieren, zusammenarbeiten und ihre Zeit verwalten. Microsoft Graph Data Connect liefert diese Daten an Microsoft Azure, sodass Sie Zugriff auf die besten Entwicklungs- und Hostingtools erhalten, um mit diesen Daten zu arbeiten. Dadurch können Kunden von innovativen oder branchenspezifischen Anwendungen profitieren, die ihre Produktivität verbessern, während sie gleichzeitig die vollständige Kontrolle über ihre Microsoft Graph-Kundendaten behalten. Microsoft bietet die sichere Kontrolle, die Kunden erwarten.
author: ajacks-msft
ms.openlocfilehash: 4f621dc40f99ec7b827ecb5cec61d6c2916b7ada
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323373"
---
# <a name="overview-of-microsoft-graph-data-connect-preview"></a>Übersicht über Microsoft Graph Data Connect (Vorschau)
Microsoft Graph enthält umfassende Informationen zu Mitarbeitern und ihrem Arbeitsplatz, einschließlich Informationen dazu, wie Mitarbeiter arbeiten und sie kommunizieren, zusammenarbeiten und ihre Zeit verwalten. Microsoft Graph Data Connect liefert diese Daten an Microsoft Azure, sodass Sie Zugriff auf die besten Entwicklungs- und Hostingtools erhalten, um mit diesen Daten zu arbeiten. Dadurch können Kunden von innovativen oder branchenspezifischen Anwendungen profitieren, die ihre Produktivität verbessern, während sie gleichzeitig die vollständige Kontrolle über ihre Microsoft Graph-Kundendaten behalten. Microsoft bietet die sichere Kontrolle, die Kunden erwarten.

## <a name="why-use-microsoft-graph-data-connect"></a>Vorteile von Microsoft Graph Data Connect
Office 365-Administratoren müssen die Herausforderungen im Zusammenhang mit dem Verschieben und Verwalten großer Mengen von Organisationsdaten sorgfältig überdenken. Microsoft Graph Data Connect ist so konzipiert, dass Administratoren neue Steuerungsmöglichkeiten für ihre Daten erhalten; Sie können diese Daten verwenden, um Apps zu entwickeln, die datengesteuerte Einblicke liefern. 

### <a name="enable-granular-consent"></a>Aktivieren der differenzierten Zustimmung

Im Microsoft Graph-Zustimmungsmodell kann ein Administrator oder Benutzer nur die Anforderung einer Anwendung zum Zugreifen auf spezifische, vordefinierte Entitätssätze erteilen oder verweigern. Eine Anforderung für Mail.Read umfasst beispielsweise Lesezugriff auf eine feste Gruppe von Entitäten, die Outlook-Mail unterstützen, einschließlich ganzer [message](/graph/api/resources/message?view=graph-rest-1.0)-Instanzen mit all ihren Eigenschaften. Microsoft Graph Data Connect ermöglicht dagegen eine differenziertere Zustimmung, sodass Anwendungen Zugriff auf bestimmte Eigenschaften in einer Entität anfordern oder die Daten in diesen Eigenschaften filtern können. Administratoren müssen die explizite Genehmigung für den Zugriff auf Microsoft Graph-Daten erteilen, bevor der Zugriff gewährt wird. Die Anforderung muss die angeforderte Zugriffsebene angeben und die Datenrichtlinienerzwingung, den Grund für die Anforderung sowie das Schema der angeforderten Daten beschreiben. Anwendungen können daher nur die Daten verwenden, die für ihre Funktion wichtig sind; nicht relevante Inhalte werden ausgeschlossen. Eine App kann beispielsweise E-Mail-Header verwenden, aber den Textinhalt und Anlagen ausschließen. 

### <a name="provide-data-governance"></a>Bereitstellen der Datengovernance
Microsoft ermöglicht eine vielfältige und verbundene Kommunikation zwischen Microsoft Graph und Azure bezüglich des Status von Kundendaten. Beim Erstellen von Apps über Microsoft Graph Data Connect können Sie eine Reihe detaillierter Richtlinien angeben, die Sie einhalten möchten. Office 365-Administratoren können diese Richtlinien dann überprüfen und ihnen zustimmen. Durch diese Vorgehensweise wird der Aufwand der Complianceverwaltung minimiert. Wenn den Richtlinien zugestimmt wird, überwacht Microsoft die Einhaltung der Richtlinien durch die Anwendung. Wenn eine Anwendung gegen eine von der Organisation festgelegte Richtlinie verstößt (oder dies versucht), wird der Datenfluss zu dieser Anwendung von Microsoft gestoppt. 

### <a name="get-access-to-data-at-scale"></a>Skalierter Zugriff auf Daten
Umfassende Anwendungen benötigen Zugriff auf große Mengen von Daten, häufig von vielen Benutzern in der Organisation gleichzeitig. Mit dem herkömmlichen Transaktionsdatenmodell müssen Sie eine komplexe Infrastruktur erstellen und Tausende von API-Aufrufe tätigen, um diese Datenübermittlung zu koordinieren. Microsoft Graph Data Connect nutzt die Vorteile von Azure Data Factory, um Office 365-Daten aus Ihrer Organisation in einem wiederholbaren Zeitplan und mit nur wenigen einfachen Schritte an Ihre Anwendung zu liefern.

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

[Richten Sie](data-connect-get-started.md) Microsoft Graph Data Connect ein, und lesen Sie die Informationen unter [Verwenden von Azure-Analysen und Office 365-Daten zum Erstellen intelligenter Anwendungen](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki).


## <a name="next-steps"></a>Nächste Schritte
Informationen zu den ersten Schritten finden Sie unter [Erste Schritte mit Microsoft Graph Data Connect (Vorschau)](data-connect-get-started.md).
