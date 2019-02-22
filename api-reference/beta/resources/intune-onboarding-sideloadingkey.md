---
title: sideLoadingKey-Ressourcentyp
description: SideLoadingKey-Entität ist für Windows 8-und 8,1-Geräte mit intallen Branchen-Apps für einen Mandanten erforderlich.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7897a50861910b67763b7d694a30096509c6c56c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170525"
---
# <a name="sideloadingkey-resource-type"></a>sideLoadingKey-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

SideLoadingKey-Entität ist für Windows 8-und 8,1-Geräte mit intallen Branchen-Apps für einen Mandanten erforderlich.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[SideLoadingKeies aufListen](../api/intune-onboarding-sideloadingkey-list.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekte.|
|[SideLoadingKey abrufen](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Lesen von Eigenschaften und Beziehungen des [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekts.|
|[SideLoadingKey erstellen](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Erstellen eines neuen [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekts.|
|[SideLoadingKey löschen](../api/intune-onboarding-sideloadingkey-delete.md)|Keine|Löscht eine [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).|
|[SideLoadingKey aktualisieren](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Aktualisieren der Eigenschaften eines [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutige ID des seitlichen Lade Schlüssels.|
|Wert|Zeichenfolge|Seiten Ladeschlüssel Wert, es ist 5x5-Wert, getrennt durch hiphens.|
|displayName|Zeichenfolge|Der Name des Seiten Lade Schlüssels wird den ITPro-Administratoren angezeigt.|
|description|String|Seiten Ladeschlüssel Beschreibung, die den ITPro-Administratoren angezeigt wird..|
|totalActivation|Int32|Die Gesamt Aktivierung des Seiten Lade Schlüssels wird den ITPro-Administratoren angezeigt.|
|lastUpdatedDateTime|Zeichenfolge|Das Datum der letzten Aktualisierung, die den ITPro-Administratoren angezeigt werden.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```




