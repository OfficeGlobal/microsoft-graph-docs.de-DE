---
title: Ressourcentyp mobileAppInstallSummary
description: Enthält Eigenschaften für die Zusammenfassung der Installation einer mobilen App.
ms.openlocfilehash: bda3f798a86b38ca0d1224ce509c355a8aec998a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058622"
---
# <a name="mobileappinstallsummary-resource-type"></a>Ressourcentyp mobileAppInstallSummary

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für die Zusammenfassung der Installation einer mobilen App.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Lesen Sie Eigenschaften und Beziehungen des [MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.|
|[MobileAppInstallSummary aktualisieren](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Aktualisieren Sie die Eigenschaften eines [MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|installedDeviceCount|Int32|Anzahl der Geräte, die diese app erfolgreich installiert haben.|
|failedDeviceCount|Int32|Anzahl der Geräte, die fehlgeschlagen sind, um diese app zu installieren.|
|notApplicableDeviceCount|Int32|Anzahl der Geräte, die für diese app nicht zutreffen.|
|notInstalledDeviceCount|Int32|Anzahl der Geräte, die diese app installiert nicht vorhanden ist.|
|pendingInstallDeviceCount|Int32|Anzahl der Geräte, die diese app installieren benachrichtigt wurden.|
|installedUserCount|Int32|Anzahl der Benutzer, deren Geräte alle erfolgreich ausgeführt wurden, um diese app zu installieren.|
|failedUserCount|Int32|Anzahl der Benutzer, die 1 haben oder weitere Gerät, deren Installation diese app fehlschlug.|
|notApplicableUserCount|Int32|Anzahl der Benutzer, deren Geräte alle nicht zutreffend für diese app waren.|
|notInstalledUserCount|Int32|Anzahl der Benutzer mit 1 oder mehrere Geräte, die diese app nicht installiert haben.|
|pendingInstallUserCount|Int32|Anzahl der Benutzer, die 1 haben oder weitere Geräte, die diese app installieren und 0 Geräte mit Fehlern benachrichtigt wurden.|

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




