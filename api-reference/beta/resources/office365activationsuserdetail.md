---
title: Ressourcentyp office365ActivationsUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: f87a5b32b08466428f0f6f0246a4b8d4c20e97be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877336"
---
# <a name="office365activationsuserdetail-resource-type"></a>Ressourcentyp office365ActivationsUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft             | Typ                                     | Beschreibung                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | Datum                                     | Das aktuelle Datum des Inhalts.          |
| userPrincipalName    | String                                   | Der Benutzerprinzipalname (UPN) des Benutzers. Der Benutzerprinzipalname ist ein Internet-Schreibweise Anmeldenamen für den Benutzer anhand der Internetstandard RFC 822. Standardmäßig sollte dies der Name des Benutzers e-Mail zuordnen. Das Standardformat ist alias@domain, wobei muss Domäne in den Mandanten-Auflistung der überprüften Domänen vorhanden sein. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. |
| displayName          | Zeichenfolge                                   | Der Name des Benutzers, der im Adressbuch angezeigt wird. Dies ist normalerweise eine Kombination aus dem Vornamen, der Initiale des weiteren Vornamens und des Nachnamens. Diese Eigenschaft ist beim Erstellen eines Benutzers erforderlich und kann nicht bei Updates deaktiviert werden. |
| userActivationCounts | [UserActivationCounts](../resources/useractivationcounts.md) -Auflistung | Neueste produktaktivierung des Benutzers wird auf allen Plattformen für alle zugewiesenen Produkttypen gezählt. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userActivationCounts": [{"@odata.type":"microsoft.graph.userActivationCounts"}]
}
```
