---
title: Ressourcentyp office365ActiveUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 95912e736459894a69f8e2e1a18c2aaf672a19a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060843"
---
# <a name="office365activeuserdetail-resource-type"></a>Ressourcentyp office365ActiveUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft                          | Typ              | Beschreibung                              |
| :-------------------------------- | :---------------- | ---------------------------------------- |
| reportRefreshDate                 | Datum              | Das aktuelle Datum des Inhalts.          |
| userPrincipalName                 | String            | Der Benutzerprinzipalname (UPN) des Benutzers. Der Benutzerprinzipalname ist ein Internet-Schreibweise Anmeldenamen für den Benutzer anhand der Internetstandard RFC 822. Standardmäßig sollte dies der Name des Benutzers e-Mail zuordnen. Das Standardformat ist alias@domain, wobei muss Domäne in den Mandanten-Auflistung der überprüften Domänen vorhanden sein. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. |
| displayName                       | Zeichenfolge            | Der Name des Benutzers, der im Adressbuch angezeigt wird. Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. |
| isDeleted                         | Boolesch           | Ob dieser Benutzer gelöschte oder weiche wurde gelöscht. |
| deletedDate                       | Datum              | Das Datum, wenn der Löschvorgang erfolgt. Standardwert ist "null", wenn der Benutzer nicht gelöscht wurde. |
| hasExchangeLicense                | Boolesch           | Gibt an, ob der Benutzer eine Exchange-Lizenz zugewiesen wurde. |
| hasOneDriveLicense                | Boolesch           | Gibt an, ob der Benutzer eine OneDrive-Lizenz zugewiesen wurde. |
| hasSharePointLicense              | Boolesch           | Gibt an, ob der Benutzer eine SharePoint-Lizenz zugewiesen wurde. |
| hasSkypeForBusinessLicense        | Boolesch           | Gibt an, ob der Benutzer eine Lizenz für Business Skype zugewiesen wurde. |
| hasYammerLicense                  | Boolesch           | Gibt an, ob der Benutzer eine Lizenz für Yammer zugewiesen wurde. |
| hasTeamsLicense                   | Boolesch           | Gibt an, ob der Benutzer eine Lizenz Teams zugewiesen wurde. |
| exchangeLastActivityDate          | Datum              | Das Datum, Benutzer zuletzt lesen oder e-Mail gesendet. |
| oneDriveLastActivityDate          | Datum              | Das Datum, wenn Benutzer zuletzt angezeigt oder bearbeitet Dateien, gemeinsam genutzte Dateien intern oder extern oder synchronisiert Dateien. |
| sharePointLastActivityDate        | Datum              | Das Datum, Benutzer zuletzt angezeigt oder bearbeitet Dateien, gemeinsam genutzte Dateien intern oder extern, synchronisiert Dateien oder SharePoint-Seiten angezeigt. |
| skypeForBusinessLastActivityDate  | Datum              | Das Datum, Benutzer zuletzt organisiert oder in Konferenzen verwendet wurde, oder Peer-zu-Peer-Sitzungen verbunden. |
| yammerLastActivityDate            | Datum              | Das Datum, wenn Benutzer zuletzt gebucht, lesen oder Nachricht gefallen. |
| teamsLastActivityDate             | Datum              | Das Datum, Benutzer zuletzt Nachrichten in Team-Kanälen gebucht, gesendete Nachrichten im privaten chatten oder Besprechungen oder Anrufe beteiligt. |
| exchangeLicenseAssignDate         | Datum              | Das letzte Datum, wenn der Benutzer eine Exchange-Lizenz zugewiesen wurde. |
| oneDriveLicenseAssignDate         | Datum              | Das letzte Datum, wenn der Benutzer eine OneDrive-Lizenz zugewiesen wurde. |
| sharePointLicenseAssignDate       | Datum              | Das letzte Datum, wenn der Benutzer eine SharePoint-Lizenz zugewiesen wurde. |
| skypeForBusinessLicenseAssignDate | Datum              | Das letzte Datum, wenn der Benutzer eine Lizenz für Business Skype zugewiesen wurde. |
| yammerLicenseAssignDate           | Datum              | Das letzte Datum, wenn der Benutzer eine Lizenz für Yammer zugewiesen wurde. |
| teamsLicenseAssignDate            | Datum              | Das letzte Datum, wenn der Benutzer eine Lizenz Teams zugewiesen wurde. |
| assignedProducts                  | Collection von Objekten des Typs „String“ | Alle Produkte für den Benutzer zugewiesen.  |

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
