---
title: eBookInstallSummary-Ressourcentyp
description: Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52d08d00bfbc26e0b72ddf53404eff8d55bb72b9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151240"
---
# <a name="ebookinstallsummary-resource-type"></a>eBookInstallSummary-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[eBookInstallSummary abrufen](../api/intune-books-ebookinstallsummary-get.md)|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Lesen der Eigenschaften und Beziehungen von [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekten.|
|[eBookInstallSummary aktualisieren](../api/intune-books-ebookinstallsummary-update.md)|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|installedDeviceCount|Int32|Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.|
|failedDeviceCount|Int32|Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.|
|notInstalledDeviceCount|Int32|Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.|
|installedUserCount|Int32|Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.|
|failedUserCount|Int32|Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.|
|notInstalledUserCount|Int32|Die Anzahl der Benutzer, die das Buch nicht installiert haben.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```




