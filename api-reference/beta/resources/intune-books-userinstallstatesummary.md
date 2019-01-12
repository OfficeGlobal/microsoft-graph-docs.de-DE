---
title: userInstallStateSummary-Ressourcentyp
description: Enthält Eigenschaften für die Zusammenfassung des Installationsstatus für einen Benutzer.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6835dcad87fbf16a8dc81b6c9f9ab124a9834a3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931853"
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





