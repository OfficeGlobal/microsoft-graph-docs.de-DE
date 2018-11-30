---
title: androidForWorkAppConfigurationSchema-Ressourcentyp
description: Schema, das die benutzerdefinierten Konfigurationen für eine Android for Work-Anwendung beschreibt.
ms.openlocfilehash: f555c7e1b9c62024531f4c4fc57a3fd3df3336fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058774"
---
# <a name="androidforworkappconfigurationschema-resource-type"></a>androidForWorkAppConfigurationSchema-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Schema, das die benutzerdefinierten Konfigurationen für eine Android for Work-Anwendung beschreibt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[androidForWorkAppConfigurationSchemas auflisten](../api/intune-androidforwork-androidforworkappconfigurationschema-list.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)-Sammlung|Listet die Eigenschaften und Beziehungen [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)-Objekten auf.|
|[androidForWorkAppConfigurationSchema abrufen](../api/intune-androidforwork-androidforworkappconfigurationschema-get.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Listet die Eigenschaften und Beziehungen des [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)-Objekts auf.|
|[androidForWorkAppConfigurationSchema erstellen](../api/intune-androidforwork-androidforworkappconfigurationschema-create.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Erstellen eines neuen [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)-Objekts.|
|[androidForWorkAppConfigurationSchema löschen](../api/intune-androidforwork-androidforworkappconfigurationschema-delete.md)|Keine|Löschen eines [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).|
|[androidForWorkAppConfigurationSchema aktualisieren](../api/intune-androidforwork-androidforworkappconfigurationschema-update.md)|[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)|Aktualisieren der Eigenschaften eines [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität (Name des Android-Pakets der Anwendung), der das Schema entspricht|
|exampleJson|Binär|UTF8-codiertes Bytearray mit der diesem Schema entsprechenden JSON-Beispielzeichenfolge, das veranschaulicht, wie die Konfiguration für diese App festgelegt werden soll|
|schemaItems|Collection von Objekten des Typs [androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md)|Sammlung von Elementen, von denen jedes eine benannte Konfigurationsoption im Schema darstellt.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "String",
      "displayName": "String",
      "description": "String",
      "defaultBoolValue": true,
      "defaultIntValue": 1024,
      "defaultStringValue": "String",
      "defaultStringArrayValue": [
        "String"
      ],
      "dataType": "String",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "String",
          "value": "String"
        }
      ]
    }
  ]
}
```





