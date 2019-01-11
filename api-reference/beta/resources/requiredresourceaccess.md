---
title: Ressourcentyp requiredResourceAccess
description: Gibt den Satz von OAuth 2.0 berechtigungsbereiche und app-Rollen unter der angegebenen Ressource, der eine Anwendung Zugriff auf erforderlich ist. Die angegebene OAuth 2.0 berechtigungsbereiche möglicherweise beim von Clientanwendungen (über die **RequiredResourceAccess** -Auflistung) angefordert werden eine Anwendung Resource aufrufen. Die **RequiredResourceAccess** -Eigenschaft der Anwendung Entität ist eine Auflistung von **ReqiredResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: 473126365a7f0b3ba3ab0371322ff90bd36318e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856168"
---
# <a name="requiredresourceaccess-resource-type"></a>Ressourcentyp requiredResourceAccess

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
