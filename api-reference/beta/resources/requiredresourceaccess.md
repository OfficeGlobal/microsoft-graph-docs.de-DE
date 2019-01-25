---
title: Ressourcentyp requiredResourceAccess
description: Gibt den Satz von OAuth 2.0 berechtigungsbereiche und app-Rollen unter der angegebenen Ressource, der eine Anwendung Zugriff auf erforderlich ist. Die angegebene OAuth 2.0 berechtigungsbereiche möglicherweise beim von Clientanwendungen (über die **RequiredResourceAccess** -Auflistung) angefordert werden eine Anwendung Resource aufrufen. Die **RequiredResourceAccess** -Eigenschaft der Anwendung Entität ist eine Auflistung von **ReqiredResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512969"
---
# <a name="requiredresourceaccess-resource-type"></a>Ressourcentyp requiredResourceAccess

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gibt den Satz von OAuth 2.0 berechtigungsbereiche und app-Rollen unter der angegebenen Ressource, der eine Anwendung Zugriff auf erforderlich ist. Die angegebene OAuth 2.0 berechtigungsbereiche möglicherweise beim von Clientanwendungen (über die **RequiredResourceAccess** -Auflistung) angefordert werden eine Anwendung Resource aufrufen. Die **RequiredResourceAccess** -Eigenschaft der [Anwendung](application.md) Entität ist eine Auflistung von **ReqiredResourceAccess**.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|resourceAccess|[ResourceAccess](resourceaccess.md) -Auflistung|Die Liste der OAuth2.0 berechtigungsbereiche und app-Rollen, die die Anwendung aus der angegebenen Ressource erforderlich sind.|
|resourceAppId|String|Der eindeutige Bezeichner für die Ressource, der Zugriff auf für die Anwendung erforderlich ist.  Dies sollte der **AppId** für die Zielanwendung für die Ressource deklarierten gleich sein.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/requiredresourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
