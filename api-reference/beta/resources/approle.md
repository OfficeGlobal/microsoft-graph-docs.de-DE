---
title: AppRole Ressourcentyp
description: Stellt eine Anwendungsrolle, die von einer Clientanwendung aus einer anderen Anwendung aufrufen angefordert werden kann oder, die verwendet werden kann, eine Anwendung Benutzern oder Gruppen in einer angegebenen Anwendungsrolle zugewiesen. Die **AppRoles** -Eigenschaft der Entität ServicePrincipal und der Anwendung Entität ist eine Auflistung von **AppRole**.
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640413"
---
# <a name="approle-resource-type"></a>AppRole Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Anwendungsrolle, die von einer Clientanwendung aus einer anderen Anwendung aufrufen angefordert werden kann oder, die verwendet werden kann, eine Anwendung Benutzern oder Gruppen in einer angegebenen Anwendungsrolle zugewiesen. Die **AppRoles** -Eigenschaft der Entität [ServicePrincipal](serviceprincipal.md) und der [Anwendung](application.md) Entität ist eine Auflistung von **AppRole**.

> Wichtig: Diese Funktion ist in der aktuellen Version deaktiviert.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowedMemberTypes|String-Sammlung|Gibt an, ob diese app Rollendefinition zugewiesen werden kann, Benutzer und Gruppen mit der Einstellung auf "Benutzer" oder in andere Anwendungen (, die diese Anwendung in Filterdaemon Service Szenarien zugreifen) mit der Einstellung auf "Application" oder beide.|
|description|String|Berechtigung Hilfetext, die in die Zuordnung der Admin-app angezeigt wird und die Erfahrungen stimmen.|
|displayName|String|Der Anzeigename für die Berechtigung, die in der Admin Zustimmung und app-Zuordnung Erfahrungen angezeigt wird.|
|id|Guid|Eindeutiger Rollenbezeichner innerhalb der **AppRoles** -Auflistung.|
|isEnabled|Boolescher Wert|Beim Erstellen oder Aktualisieren einer Rollendefinition, muss dies auf **true** festgelegt werden (die Standardeinstellung ist). Um eine Rolle zu löschen, muss dieser zunächst auf **false**festgelegt werden.  An dieser Stelle kann diese Rolle im Gespräch nachfolgende entfernt werden.|
|Wert|Zeichenfolge|Gibt den Wert des Anspruchs Rollen, die die Anwendung erwarten in die Authentifizierung und Zugriffsteuerung Token an.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
