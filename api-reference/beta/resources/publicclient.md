---
title: Ressourcentyp publicClient
description: Gibt die Einstellungen für nicht Web App oder Web-Api. (Mobile oder anderen öffentlichen Client wie eine installierte Anwendung, die auf einem Desktopgerät ausgeführt)
localization_priority: Normal
ms.openlocfilehash: c466c91f90ac8adc2bf3806fa212e0b01e6d2507
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864197"
---
# <a name="publicclient-resource-type"></a>Ressourcentyp publicClient

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Gibt die Einstellungen für nicht Web App oder Web-Api. (Mobile oder anderen öffentlichen Client wie eine installierte Anwendung, die auf einem Desktopgerät ausgeführt)

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|redirectUris|Collection von Objekten des Typs „String“| Gibt die URLs der Benutzertoken für die Anmeldung an gesendet werden, oder die Umleitung, URIs, dass OAuth 2.0 Autorisierungscodes und Zugriffstoken gesendet werden. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
