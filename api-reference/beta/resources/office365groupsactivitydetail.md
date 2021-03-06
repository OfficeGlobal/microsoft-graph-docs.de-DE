---
title: Ressourcentyp office365GroupsActivityDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b467f73ed2a4a5e48cb1243c5b1326591bcd707
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575118"
---
# <a name="office365groupsactivitydetail-resource-type"></a>Ressourcentyp office365GroupsActivityDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                          | Typ    | Beschreibung                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| reportRefreshDate                 | Date    | Das aktuelle Datum des Inhalts.          |
| groupDisplayName                  | String  | Der Anzeigename der Gruppe.           |
| isDeleted                         | Boolean | Ob dieser Benutzer gelöschte oder weiche wurde gelöscht. |
| ownerPrincipalName                | String  | Der Gruppe Besitzer principal Name.          |
| lastActivityDate                  | Date    | Datum der letzten Aktivität für die folgenden Szenarien: Postfach empfangene e-Mails; gruppieren Benutzer angezeigt, bearbeitet, freigegebene oder Dateien in SharePoint-Dokumentbibliothek synchronisiert; SharePoint-Seiten angezeigt; Benutzer gebucht, lesen oder gefallen Nachrichten in Yammer-Gruppen. |
| groupType                         | String  | Der Gruppentyp. Mögliche Werte sind: **öffentlich** oder **Privat**. |
| memberCount                       | Int64   | Die Gruppe Elementanzahl.                  |
| externalMemberCount               | Int64   | Die Gruppe externe Elementanzahl.         |
| exchangeReceivedEmailCount        | Int64   | Die Anzahl der e-Mail, die das Gruppenpostfach empfangen. |
| sharePointActiveFileCount         | Int64   | Die Anzahl der aktiven Dateien in der Website der SharePoint-Gruppe. |
| yammerPostedMessageCount          | Int64   | Die Anzahl von Nachrichten zu Yammer-Gruppen bereitgestellt werden. |
| yammerReadMessageCount            | Int64   | Lesen Sie die Anzahl der Nachrichten in Yammer-Gruppen. |
| yammerLikedMessageCount           | Int64   | Die Anzahl der Nachrichten in Yammer-Gruppen gefallen. |
| exchangeMailboxTotalItemCount     | Int64   | Die Anzahl der Elemente in der Gruppenpostfach. |
| exchangeMailboxStorageUsedInBytes | Int64   | Der Speicher des Postfachs Gruppe verwendet.   |
| sharePointTotalFileCount          | Int64   | Die Gesamtzahl der Dateien in der Website der SharePoint-Gruppe. |
| sharePointSiteStorageUsedInBytes  | Int64   | Die Speicherung von SharePoint-Gruppe der Website verwendet. |
| reportPeriod                      | String  | Die Anzahl der Tage, die der Bericht wird behandelt.    |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```
