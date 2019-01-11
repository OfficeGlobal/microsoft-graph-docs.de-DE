---
title: userInstallStateSummary-Ressourcentyp
description: Enthält Eigenschaften für die Zusammenfassung des Installationsstatus für einen Benutzer.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3e63bf8a5f6ab982a8542f483ad8f017c00b1496
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894551"
---
# <a name="userinstallstatesummary-resource-type"></a>userInstallStateSummary-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für die Zusammenfassung des Installationsstatus für einen Benutzer.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[userInstallStateSummaries auflisten](../api/intune-books-userinstallstatesummary-list.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Objekte.|
|[userInstallStateSummary abrufen](../api/intune-books-userinstallstatesummary-get.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Lesen von Eigenschaften und Beziehungen des [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Objekts.|
|[userInstallStateSummary erstellen](../api/intune-books-userinstallstatesummary-create.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Erstellen eines neuen [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Objekts.|
|[userInstallStateSummary löschen](../api/intune-books-userinstallstatesummary-delete.md)|Keine|Löscht ein [UserInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Objekt.|
|[userInstallStateSummary aktualisieren](../api/intune-books-userinstallstatesummary-update.md)|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|Aktualisieren der Eigenschaften eines [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|userName|String|Name des Benutzers|
|installedDeviceCount|Int32|Anzahl der installierten Geräte|
|failedDeviceCount|Int32|Anzahl der fehlgeschlagenen Geräte|
|notInstalledDeviceCount|Int32|Anzahl der nicht installierten Geräte|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceStates|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung|Der Installationsstatus des E-Books.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```



