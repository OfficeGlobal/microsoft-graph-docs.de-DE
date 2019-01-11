---
title: Ressourcentyp appIdentity
description: Gibt die Identität der Anwendung, die die Aktion ausgeführt oder wurde geändert. Enthält Anwendungs-Id, Name, Dienstprinzipalnamen-ID und Name. Diese Ressource wird von der DirectoryAudit API aufgerufen.
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855783"
---
# <a name="appidentity-resource-type"></a>Ressourcentyp appIdentity
Gibt die Identität der Anwendung, die die Aktion ausgeführt oder wurde geändert. Enthält Anwendungs-Id, Name, Dienstprinzipalnamen-ID und Name. Diese Ressource wird von der [DirectoryAudit](../api/directoryaudit-get.md) API aufgerufen.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|appId|Zeichenfolge|Bezieht sich auf die eindeutige GUID, die Id der Anwendung in Azure Active Directory darstellt.|
|displayName|String|Bezieht sich auf den Namen der Anwendung in der Azure-Verwaltungsportal angezeigt.|
|servicePrincipalId|String|Bezieht sich auf die eindeutige GUID, die für die entsprechenden App Service Principal-Id in Azure Active Directory angibt.|
|servicePrincipalName|Zeichenfolge|Bezieht sich auf der Service Principal Name ist der Name der Anwendung im Mandanten. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
