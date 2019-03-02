---
title: Übersicht über die Business Central-API
description: Übersicht darüber, warum Sie Ihre Lösungen mit Geschäfts zentralen APIs integrieren möchten.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0602b02592bec5210f243f77654a52ba96e6746a
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366802"
---
# <a name="dynamics-365-business-central-api-overview-preview"></a>Dynamics 365 Business Central-API (Übersicht)
Dynamics 365 Business Central ist eine All-in-One-Unternehmensverwaltungslösung, die einfach zu verwenden und anzupassen ist, damit Sie Ihr Unternehmen verbinden und bessere Entscheidungen treffen können. Es bietet eine End-to-End-Ansicht Ihres Unternehmens, sodass Sie Ihre Finanzdaten verwalten, Ihre Supply Chain automatisieren und sichern, Smarter verkaufen und den Kundenservice verbessern können, Projekte termingerecht und unter Budget halten und ihre Abläufe optimieren können.

## <a name="why-integrate-with-dynamics-365-business-central"></a>Gründe für die Integration in Dynamics 365 Business Central
Durch die Integration Ihrer Apps in Dynamics 365 Business Central können Sie Erfahrungen erstellen, die Ihre geschäftlichen Anforderungen erfüllen. Sie können Lösungen erstellen, die Ihren Benutzern das Ausführen wichtiger geschäftlicher Aufgaben und Funktionen ermöglichen. Sie können Microsoft Graph verwenden, um Ihre Finanzen zu verwalten, mit Geschäftskontakten zu arbeiten, Verkaufs-und Einkaufsdokumente zu erstellen und zu versenden und Einblicke in Finanzberichte zu gewinnen. 

### <a name="synchronize-your-business-applications"></a>Synchronisieren Ihrer Geschäftsanwendungen
Viele Unternehmen verwenden unterschiedliche, getrennte Geschäftsanwendungen, um verschiedene Funktionen des Unternehmens zu verwalten. Mit Microsoft Graph können Sie die Daten verbinden, um diese Anwendungen zusammenzubringen. So können Sie Ihre Abrechnungsanwendung problemlos mit Mitarbeiterdatensätzen verbinden, ihre Spesen Anwendung mit Kreditorendaten Sätzen verbinden und ihre Kundendatensätze auf dem neuesten Stand halten. Verbinden Sie Ihre Daten, um Ihre Anwendungen synchron zu halten.

### <a name="create-custom-apps-to-manage-your-business-processes"></a>Erstellen benutzerdefinierter Apps zur Verwaltung Ihrer Geschäftsprozesse
Jedes Unternehmen unterscheidet sich durch spezielle Geschäftsprozesse. Diese Prozesse können mit benutzerdefinierten apps optimiert werden, die auf den Prozess zugeschnitten sind. Microsoft Graph erleichtert die Integration dieser apps in Ihre Finanzdaten. Das Erstellen einer Verkaufs-oder Feld Dienst-APP, die Verkaufsdokumente erstellt, eine Spesen-APP, die Einkaufsdokumente erstellt, oder eine Lohn-und Gehaltsabrechnung-APP, die Haupt Buch Journale erstellt, wird möglich, indem alle Ihre Dokumente in Ihrem Finanzsystem bleiben.

### <a name="gain-insights-from-your-financial-data"></a>Gewinnen von Einblicken aus ihren Finanzdaten
Microsoft Graph bietet Zugriff auf Ihre Finanzberichte. Verbinden Sie BI-Tools und-Apps mit ihrer Bilanz, Kapitalflussrechnung, Kreditoren-und Forderungs Alterungs Berichten sowie Berichte zum Bilanzausgleich, um BI-Dashboards zu erstellen und sicherzustellen, dass Benutzer Zugriff auf die benötigten Informationen haben.

## <a name="authorization"></a>Authorization
Verwenden Sie den Azure AD v 2.0-Endpunkt, um Dynamics 365 Business Central-APIs zu authentifizieren. Alle APIs erfordern den `Authorization: Bearer {access-token}` Anforderungsheader. Weitere Informationen zur Autorisierung finden Sie unter [Abrufen von Zugriffstoken zum Aufrufen von Microsoft Graph](auth-overview.md).

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

Siehe [Dynamics 365 Business Central-API in Microsoft Graph Beta](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta).


## <a name="next-steps"></a>Nächste Schritte
Erfahren Sie mehr über die [Business Central-API und Anwendungsfälle](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta) , die in Microsoft Graph unterstützt werden.
