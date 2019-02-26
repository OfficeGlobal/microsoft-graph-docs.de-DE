---
title: userInstallStateSummary-Ressourcentyp
description: Enthält Eigenschaften für die Zusammenfassung des Installationsstatus für einen Benutzer.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e7c219ef2128f6d15a0efc6e98ec781e2c47ffe
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262573"
---
# <a name="userinstallstatesummary-resource-type"></a>userInstallStateSummary-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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



