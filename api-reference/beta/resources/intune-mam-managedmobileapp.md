---
title: managedMobileApp-Ressourcentyp
description: Der Bezeichner für die Bereitstellung einer App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 842987c0ed12322d77e0f28fc71d197950452dfe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148636"
---
# <a name="managedmobileapp-resource-type"></a>managedMobileApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|string|Schlüssel der Entität|
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




