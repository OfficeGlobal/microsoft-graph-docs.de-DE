---
title: Ressourcentyp groupPolicyPresentationValue
description: Die Basis Präsentation Wert Entität, die den Wert für eine einzelne Gruppenrichtlinie Präsentation gespeichert werden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ec299eccc29ddcb39ece0d1f6c0e063a02192909
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429935"
---
# <a name="grouppolicypresentationvalue-resource-type"></a>Ressourcentyp groupPolicyPresentationValue

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Die Basis Präsentation Wert Entität, die den Wert für eine einzelne Gruppenrichtlinie Präsentation gespeichert werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste groupPolicyPresentationValues](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Auflistung|Listeneigenschaften und Beziehungen der [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekte.|
|[Abrufen von groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Lesen Sie Eigenschaften und Beziehungen des [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekts.|
|[Erstellen von groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Erstellen eines neuen [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekts.|
|[GroupPolicyPresentationValue löschen](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|Keine|Löscht eine [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).|
|[GroupPolicyPresentationValue aktualisieren](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Das Datum und die Zeit, die das Objekt zuletzt geändert wurde.|
|createdDateTime|DateTimeOffset|Das Datum und die Zeit, die das Objekt erstellt wurde.|
|id|Zeichenfolge|Schlüssel der Entität|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Der Gruppenrichtlinie Definition zugeordnete Wert mit dem Wert der Präsentation.|
|Präsentation|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|Der Gruppenrichtlinie Präsentation Präsentation Wert zugeordnet.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)"
}
```




