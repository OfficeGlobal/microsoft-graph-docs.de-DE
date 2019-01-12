---
title: Ressourcentyp alertTrigger
description: Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3a2f6818bad0c5600e4b2a2a2682707643d1900c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991258"
---
# <a name="alerttrigger-resource-type"></a>Ressourcentyp alertTrigger

Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|name|Zeichenfolge|Der Name der Eigenschaft, die als eine Erkennung Trigger.|
|type|Zeichenfolge|Typ der Eigenschaft im Schlüssel / Wert-Paar für Auslegung. String, Boolean, beispielsweise usw.|
|Wert|Zeichenfolge|Der Wert der Eigenschaft, die als eine Erkennung Trigger.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a>Beispiel

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
