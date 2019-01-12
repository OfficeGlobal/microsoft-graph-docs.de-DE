---
title: Ressourcentyp office365ActivationsUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3e2b7d5fb3c42db02407a187649544b2560f898a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982855"
---
# <a name="office365activationsuserdetail-resource-type"></a>Ressourcentyp office365ActivationsUserDetail

## <a name="properties"></a>Eigenschaften

| Eigenschaft             | Typ                                     | Beschreibung                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | Datum                                     | Das aktuelle Datum des Inhalts.          |
| userPrincipalName    | Zeichenfolge                                   | Der Benutzerprinzipalname (UPN) des Benutzers. Der Benutzerprinzipalname ist ein Internet-Schreibweise Anmeldenamen für den Benutzer anhand der Internetstandard RFC 822. Standardmäßig sollte dies der Name des Benutzers e-Mail zuordnen. Das Standardformat ist alias@domain, wobei muss Domäne in den Mandanten-Auflistung der überprüften Domänen vorhanden sein. Diese Eigenschaft ist erforderlich, wenn ein Benutzer erstellt wird. |
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
