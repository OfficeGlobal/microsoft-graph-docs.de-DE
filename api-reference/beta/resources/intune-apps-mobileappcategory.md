---
title: mobileAppCategory-Ressourcentyp
description: Enthält Eigenschaften für eine einzelne Intune-App-Kategorie.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 59f840bdd3a01ca8f8614f6e14e53d9ba95005dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422264"
---
# <a name="mobileappcategory-resource-type"></a>mobileAppCategory-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Enthält Eigenschaften für eine einzelne Intune-App-Kategorie.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[mobileAppCategories auflisten](../api/intune-apps-mobileappcategory-list.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)-Objekte.|
|[mobileAppCategory abrufen](../api/intune-apps-mobileappcategory-get.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)-Objekts.|
|[mobileAppCategory erstellen](../api/intune-apps-mobileappcategory-create.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Erstellen eines neuen [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)-Objekts.|
|[MobileAppCategory löschen](../api/intune-apps-mobileappcategory-delete.md)|Keine|Löscht eine [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[mobileAppCategory aktualisieren](../api/intune-apps-mobileappcategory-update.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Aktualisieren der Eigenschaften eines [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|displayName|String|Name der App-Kategorie|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der mobileAppCategory.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




