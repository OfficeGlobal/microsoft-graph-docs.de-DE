---
title: Ressourcentyp office365ServicesUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573893"
---
# <a name="office365servicesusercounts-resource-type"></a>Ressourcentyp office365ServicesUserCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft                 | Typ   | Beschreibung                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Date   | Das aktuelle Datum des Inhalts.          |
| exchangeActive           | Int64  | Die Anzahl von aktiven Benutzern auf Exchange. Jeder Benutzer, der lesen und e-Mail senden kann, wird einen aktiven Benutzer betrachtet. |
| exchangeInactive         | Int64  | Die Anzahl der inaktive Benutzer auf Exchange. |
| oneDriveActive           | Int64  | Die Anzahl von aktiven Benutzern in OneDrive. Jeder Benutzer, der angezeigt oder bearbeitet Dateien, freigegebenen Dateien intern oder extern oder Dateien synchronisiert wird einen aktiven Benutzer betrachtet. |
| oneDriveInactive         | Int64  | Die Anzahl der inaktive Benutzer in OneDrive. |
| sharePointActive         | Int64  | Die Anzahl der aktive Benutzer in SharePoint. Jeder Benutzer, der angezeigt oder bearbeitet Dateien, gemeinsam genutzte Dateien intern oder extern, synchronisiert Dateien oder SharePoint-Seiten angezeigt wird einen aktiven Benutzer betrachtet. |
| sharePointInactive       | Int64  | Die Anzahl der inaktive Benutzer auf SharePoint. |
| skypeForBusinessActive   | Int64  | Die Anzahl von aktiven Benutzern auf Skype für Unternehmen. Jeder Benutzer, die organisiert oder in Konferenzen teilgenommen Peer-zu-Peer-Sitzungen verbunden wird einen aktiven Benutzer betrachtet. |
| skypeForBusinessInactive | Int64  | Die Anzahl der inaktive Benutzer auf Skype für Unternehmen. |
| yammerActive             | Int64  | Die Anzahl der aktive Benutzer in Yammer. Jeder Benutzer kann buchen, lesen oder like Nachrichten wird einen aktiven Benutzer betrachtet. |
| yammerInactive           | Int64  | Die Anzahl der inaktive Benutzer auf Yammer.  |
| teamsActive              | Int64  | Die Anzahl der aktive Benutzer in Microsoft-Teams. Jeder Benutzer, die Nachrichten im Team Kanäle gebucht, gesendete Nachrichten in privaten chatten oder Besprechungen oder Anrufe beteiligt ist einen aktiven Benutzer betrachtet. |
| teamsInactive            | Int64  | Die Anzahl der inaktive Benutzer in Microsoft-Teams.     |
| office365Active          | Int64  | Die Anzahl von aktiven Benutzern in Office 365.   |
| office365Inactive        | Int64  | Die Anzahl der inaktive Benutzer in Office 365.     |
| reportPeriod             | String | Die Anzahl der Tage, die der Bericht wird behandelt.    |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```
