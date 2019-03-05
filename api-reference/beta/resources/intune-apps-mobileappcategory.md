---
title: mobileAppCategory-Ressourcentyp
description: Enthält Eigenschaften für eine einzelne Intune-App-Kategorie.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 190fc435cbcfb1ad262e93f86bec84de989f9194
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140565"
---
# <a name="mobileappcategory-resource-type"></a>mobileAppCategory-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|Zeichenfolge|Schlüssel der Entität|
|displayName|Zeichenfolge|Name der App-Kategorie|
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




