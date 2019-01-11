---
title: Ressourcentyp attributeMapping
description: Definiert, wie die Werte für das angegebene Ziel-Attribut während der Synchronisation übertragen werden soll.
localization_priority: Normal
ms.openlocfilehash: 6c7a6367684b3e11013355b6d4726afe3346dab9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825277"
---
# <a name="attributemapping-resource-type"></a>Ressourcentyp attributeMapping

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Definiert, wie die Werte für das angegebene Ziel-Attribut während der Synchronisation übertragen werden soll.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                  | Typ                      | Beschreibung    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | Zeichenfolge                    |Standardwert verwendet werden, für den Fall, dass die **Source** -Eigenschaft auf ausgewertet wurde `null`. Optional.|
|exportMissingReferences    |Zeichenfolge                     |Nur für internen Gebrauch.|
|flowBehavior               |attributeFlowBehavior      |Definiert, wenn dieses Attribut in das Zielverzeichnis exportiert werden sollen. Mögliche Werte sind: `FlowWhenChanged` und `FlowAlways`. Der Standardwert lautet `FlowWhenChanged`. |
|Wechselkurs des Flusstyps                   |attributeFlowType          |Definiert, wenn dieses Attribut in das Zielverzeichnis aktualisiert werden soll. Mögliche Werte sind: `Always` (Standard), `ObjectAddOnly` (nur wenn neues Objekt erstellt wird), `MultiValueAddOnly` (nur wenn die Änderung neue Werte ein Attribut mit mehreren Werten hinzugefügt werden). |
|matchingPriority           |Int32                      |Wenn größer als 0, wird dieses Attribut zum Ausführen einer anfänglichen Übereinstimmung zwischen Quell- und Ziel-Verzeichnissen-Objekte verwendet werden. Das Synchronisierungsmodul versucht, das mithilfe des Attributs mit dem niedrigsten Wert von übereinstimmenden Priorität zuerst übereinstimmende Objekt zu suchen. Wenn nicht gefunden, wird das Attribut mit der nächsten übereinstimmenden Priorität verwendet werden und so weiter ein bis Übereinstimmung gefunden wurde oder keine weiteren übereinstimmenden Attribute bleiben. Als übereinstimmende Attribute sollte nur Attribute, die erwartet werden, damit eindeutige Werte wie e-Mails, die verwendet werden.|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | Definiert, wie ein Wert sein sollte extrahiert haben (oder transformiert), aus dem Quellobjekt. |
|targetAttributeName        |Zeichenfolge                     |Name des Attributs im Zielobjekt. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
