---
title: managedMobileApp-Ressourcentyp
description: Der Bezeichner für die Bereitstellung einer App
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b8de88976937a967f60a0842eeb9f24b465e50f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419254"
---
# <a name="managedmobileapp-resource-type"></a>managedMobileApp-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Der Bezeichner für die Bereitstellung einer App

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedMobileApps auflisten](../api/intune-mam-managedmobileapp-list.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekte.|
|[managedMobileApp abrufen](../api/intune-mam-managedmobileapp-get.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Lesen von Eigenschaften und Beziehungen des [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekts.|
|[managedMobileApp erstellen](../api/intune-mam-managedmobileapp-create.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Erstellen eines neuen [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekts.|
|[managedMobileApp löschen](../api/intune-mam-managedmobileapp-delete.md)|Keine|Löscht ein [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekt.|
|[managedMobileApp aktualisieren](../api/intune-mam-managedmobileapp-update.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Aktualisieren der Eigenschaften eines [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Bezeichner der App mit dem zugehörigen Betriebssystemtyp|
|id|Zeichenfolge|Schlüssel der Entität|
|Version|Zeichenfolge|Version der Entität|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




