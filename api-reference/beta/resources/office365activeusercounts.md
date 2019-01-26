---
title: Ressourcentyp office365ActiveUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bbc51e4859b005c01b0f8d2cfb2db3ca902d60e2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572206"
---
# <a name="office365activeusercounts-resource-type"></a>Ressourcentyp office365ActiveUserCounts

## <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ   | Beschreibung                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Date   | Das aktuelle Datum des Inhalts.          |
| Office365         | Int64  | Die Anzahl von aktiven Benutzern in Office 365. Dieser Wert schließt alle aktiven Benutzer in Exchange, OneDrive, SharePoint, Skype für Unternehmen, Yammer und Microsoft-Teams. Für jedes Produkt in der entsprechenden eigenschaftsbeschreibung finden Sie die Definition der aktiven Benutzer. |
| Exchange          | Int64  | Die Anzahl von aktiven Benutzern in Exchange. Jeder Benutzer, der lesen und e-Mail senden kann, wird einen aktiven Benutzer betrachtet. |
| oneDrive          | Int64  | Die Anzahl von aktiven Benutzern in OneDrive. Jeder Benutzer, der angezeigt oder bearbeitet Dateien, freigegebenen Dateien intern oder extern oder Dateien synchronisiert wird einen aktiven Benutzer betrachtet. |
| sharePoint        | Int64  | Die Anzahl von aktiven Benutzern in SharePoint. Jeder Benutzer, der angezeigt oder bearbeitet Dateien, gemeinsam genutzte Dateien intern oder extern, synchronisiert Dateien oder SharePoint-Seiten angezeigt wird einen aktiven Benutzer betrachtet. |
| skypeForBusiness  | Int64  | Die Anzahl von aktiven Benutzern in Skype für Unternehmen. Jeder Benutzer, die organisiert oder in Konferenzen teilgenommen Peer-zu-Peer-Sitzungen verbunden wird einen aktiven Benutzer betrachtet. |
| Yammer            | Int64  | Die Anzahl von aktiven Benutzern in Yammer. Jeder Benutzer kann buchen, lesen oder like Nachrichten wird einen aktiven Benutzer betrachtet. |
| Teams             | Int64  | Die Anzahl der aktiven Benutzer in Microsoft-Teams. Jeder Benutzer, die Nachrichten im Team Kanäle gebucht, gesendete Nachrichten in privaten chatten oder Besprechungen oder Anrufe beteiligt ist einen aktiven Benutzer betrachtet. |
| reportDate        | Date   | Das Datum, an dem eine Anzahl von Benutzern aktiv waren. |
| reportPeriod      | String | Die Anzahl der Tage, die der Bericht wird behandelt.    |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
