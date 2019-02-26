---
title: managedDeviceMobileAppConfigurationUserSummary-Ressourcentyp
description: Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für eine Zusammenfassung des Benutzerstatus von MDM-Konfigurationen mobiler Apps.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 96ec2f44864e29f374ab9ccf3f63a65a91692087
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253442"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a>managedDeviceMobileAppConfigurationUserSummary-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für eine Zusammenfassung des Benutzerstatus von MDM-Konfigurationen mobiler Apps.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDeviceMobileAppConfigurationUserSummary abrufen](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)-Objekts.|
|[managedDeviceMobileAppConfigurationUserSummary aktualisieren](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|Aktualisieren der Eigenschaften eines [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|pendingCount|Int32|Anzahl der ausstehenden Benutzer|
|notApplicableCount|Int32|Anzahl der nicht anwendbaren Benutzer|
|successCount|Int32|Anzahl der erfolgreichen Benutzer|
|errorCount|Int32|Anzahl der Benutzer mit Fehlern|
|failedCount|Int32|Anzahl der fehlgeschlagenen Benutzer|
|lastUpdateDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Aktualisierung|
|configurationVersion|Int32|Version der Richtlinie für diese Übersicht|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



