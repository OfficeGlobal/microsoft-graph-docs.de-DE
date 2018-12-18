---
title: userInstallStateSummary-Ressourcentyp
description: Enthält Eigenschaften für die Zusammenfassung des Installationsstatus für einen Benutzer.
author: tfitzmac
ms.openlocfilehash: 3d8976cd7db7baabaec60bdf3fe2ed18094156c1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314385"
---
# <a name="userinstallstatesummary-resource-type"></a>userInstallStateSummary-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|id|String|Schlüssel der Entität|
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





