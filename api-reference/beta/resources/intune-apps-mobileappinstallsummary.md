---
title: mobileAppInstallSummary-Ressourcentyp
description: Enthält Eigenschaften für die Installationszusammenfassung einer mobilen App.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9747d53c56f9e505b61e1fa38bf5abdc27d14e42
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150764"
---
# <a name="mobileappinstallsummary-resource-type"></a>mobileAppInstallSummary-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für die Installationszusammenfassung einer mobilen App.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MobileAppInstallSummary abrufen](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.|
|[MobileAppInstallSummary aktualisieren](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Aktualisieren der Eigenschaften eines [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|installedDeviceCount|Int32|Die Anzahl der Geräte, die diese APP erfolgreich installiert haben.|
|failedDeviceCount|Int32|Anzahl der Geräte, die diese APP nicht installiert haben.|
|notApplicableDeviceCount|Int32|Die Anzahl der Geräte, die für diese APP nicht anwendbar sind.|
|notInstalledDeviceCount|Int32|Anzahl der Geräte, auf denen diese APP nicht installiert ist.|
|pendingInstallDeviceCount|Int32|Anzahl der Geräte, die zur Installation dieser APP benachrichtigt wurden.|
|installedUserCount|Int32|Die Anzahl der Benutzer, deren Geräte alle für die Installation dieser APP erfolgreich waren.|
|failedUserCount|Int32|Die Anzahl der Benutzer, die über ein Gerät verfügen, für das diese APP nicht installiert werden konnte.|
|notApplicableUserCount|Int32|Die Anzahl der Benutzer, deren Geräte für diese APP nicht anwendbar waren.|
|notInstalledUserCount|Int32|Die Anzahl von Benutzern, die über 1 oder mehr Geräte verfügen, die diese APP nicht installiert haben.|
|pendingInstallUserCount|Int32|Die Anzahl der Benutzer mit mindestens 1 Gerät, die zur Installation dieser APP benachrichtigt wurden und über 0 Geräte mit Fehlern verfügen.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```




