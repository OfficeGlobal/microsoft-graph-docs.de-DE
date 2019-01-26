---
title: Ressourcentyp office365ActiveUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 192629623b0a0d46453f4dd4f9bfd7f1dc48cccf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575370"
---
# <a name="office365activeuserdetail-resource-type"></a>Ressourcentyp office365ActiveUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                          | Typ              | Beschreibung                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Date              | Das aktuelle Datum des Inhalts.          |
| userPrincipalName                 | String            | Der Benutzerprinzipalname (UPN) des Benutzers. Der Benutzerprinzipalname ist ein Internet-Schreibweise Anmeldenamen für den Benutzer anhand der Internetstandard RFC 822. Standardmäßig sollte dies der Name des Benutzers e-Mail zuordnen. Das Standardformat ist alias@domain, wobei muss Domäne in den Mandanten-Auflistung der überprüften Domänen vorhanden sein. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. |
| displayName                       | Zeichenfolge            | Der Name des Benutzers, der im Adressbuch angezeigt wird. Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. |
| isDeleted                         | Boolean           | Ob dieser Benutzer gelöschte oder weiche wurde gelöscht. |
| deletedDate                       | Date              | Das Datum, wenn der Löschvorgang erfolgt. Standardwert ist "null", wenn der Benutzer nicht gelöscht wurde. |
| hasExchangeLicense                | Boolean           | Gibt an, ob der Benutzer eine Exchange-Lizenz zugewiesen wurde. |
| hasOneDriveLicense                | Boolean           | Gibt an, ob der Benutzer eine OneDrive-Lizenz zugewiesen wurde. |
| hasSharePointLicense              | Boolean           | Gibt an, ob der Benutzer eine SharePoint-Lizenz zugewiesen wurde. |
| hasSkypeForBusinessLicense        | Boolean           | Gibt an, ob der Benutzer eine Lizenz für Business Skype zugewiesen wurde. |
| hasYammerLicense                  | Boolean           | Gibt an, ob der Benutzer eine Lizenz für Yammer zugewiesen wurde. |
| hasTeamsLicense                   | Boolean           | Gibt an, ob der Benutzer eine Lizenz Teams zugewiesen wurde. |
| exchangeLastActivityDate          | Date              | Das Datum, Benutzer zuletzt lesen oder e-Mail gesendet. |
| oneDriveLastActivityDate          | Date              | Das Datum, wenn Benutzer zuletzt angezeigt oder bearbeitet Dateien, gemeinsam genutzte Dateien intern oder extern oder synchronisiert Dateien. |
| sharePointLastActivityDate        | Date              | Das Datum, Benutzer zuletzt angezeigt oder bearbeitet Dateien, gemeinsam genutzte Dateien intern oder extern, synchronisiert Dateien oder SharePoint-Seiten angezeigt. |
| skypeForBusinessLastActivityDate  | Date              | Das Datum, Benutzer zuletzt organisiert oder in Konferenzen verwendet wurde, oder Peer-zu-Peer-Sitzungen verbunden. |
| yammerLastActivityDate            | Date              | Das Datum, wenn Benutzer zuletzt gebucht, lesen oder Nachricht gefallen. |
| teamsLastActivityDate             | Date              | Das Datum, Benutzer zuletzt Nachrichten in Team-Kanälen gebucht, gesendete Nachrichten im privaten chatten oder Besprechungen oder Anrufe beteiligt. |
| exchangeLicenseAssignDate         | Date              | Das letzte Datum, wenn der Benutzer eine Exchange-Lizenz zugewiesen wurde. |
| oneDriveLicenseAssignDate         | Date              | Das letzte Datum, wenn der Benutzer eine OneDrive-Lizenz zugewiesen wurde. |
| sharePointLicenseAssignDate       | Date              | Das letzte Datum, wenn der Benutzer eine SharePoint-Lizenz zugewiesen wurde. |
| skypeForBusinessLicenseAssignDate | Date              | Das letzte Datum, wenn der Benutzer eine Lizenz für Business Skype zugewiesen wurde. |
| yammerLicenseAssignDate           | Date              | Das letzte Datum, wenn der Benutzer eine Lizenz für Yammer zugewiesen wurde. |
| teamsLicenseAssignDate            | Date              | Das letzte Datum, wenn der Benutzer eine Lizenz Teams zugewiesen wurde. |
| assignedProducts                  | Zeichenfolgenauflistung | Alle Produkte für den Benutzer zugewiesen.  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "hasExchangeLicense": true, 
  "hasOneDriveLicense": true, 
  "hasSharePointLicense": true, 
  "hasSkypeForBusinessLicense": true, 
  "hasYammerLicense": true, 
  "hasTeamsLicense": true, 
  "exchangeLastActivityDate": "Date", 
  "oneDriveLastActivityDate": "Date", 
  "sharePointLastActivityDate": "Date", 
  "skypeForBusinessLastActivityDate": "Date", 
  "yammerLastActivityDate": "Date", 
  "teamsLastActivityDate": "Date", 
  "exchangeLicenseAssignDate": "Date", 
  "oneDriveLicenseAssignDate": "Date", 
  "sharePointLicenseAssignDate": "Date", 
  "skypeForBusinessLicenseAssignDate": "Date", 
  "yammerLicenseAssignDate": "Date", 
  "teamsLicenseAssignDate": "Date", 
  "assignedProducts": ["String"]
}
```
