---
title: Ressourcentyp appIdentity
description: Gibt die Identität der Anwendung, die die Aktion ausgeführt oder wurde geändert. Enthält Anwendungs-Id, Name, Dienstprinzipalnamen-ID und Name. Diese Ressource wird von der DirectoryAudit API aufgerufen.
ms.openlocfilehash: 6fcbe8dbb1e17139111c5f1fa9e8681cd1b996a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061962"
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