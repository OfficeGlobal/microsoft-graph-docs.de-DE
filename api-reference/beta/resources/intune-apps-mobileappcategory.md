---
title: mobileAppCategory-Ressourcentyp
description: Enthält Eigenschaften für eine einzelne Intune-App-Kategorie.
author: tfitzmac
ms.openlocfilehash: f40e9a24269d276c89d770acb0d772a7bdf94c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340761"
---
# <a name="mobileappcategory-resource-type"></a>mobileAppCategory-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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





