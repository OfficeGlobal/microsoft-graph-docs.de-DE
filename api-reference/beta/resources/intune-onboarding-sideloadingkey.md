---
title: Ressourcentyp sideLoadingKey
description: SideLoadingKey Entität ist für Windows 8 und Anwendungsservercomputern installiert Zeile des Geschäfts-Apps für einen Mandanten 8.1 Geräte erforderlich.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f7be853faae78e0ac7528d0127fd11b928164ee9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410042"
---
# <a name="sideloadingkey-resource-type"></a>Ressourcentyp sideLoadingKey

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

SideLoadingKey Entität ist für Windows 8 und Anwendungsservercomputern installiert Zeile des Geschäfts-Apps für einen Mandanten 8.1 Geräte erforderlich.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Auflistung|Listeneigenschaften und Beziehungen der [SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekte.|
|[Abrufen von sideLoadingKey](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Lesen Sie Eigenschaften und Beziehungen des [SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekts.|
|[Erstellen von sideLoadingKey](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Erstellen eines neuen [SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekts.|
|[SideLoadingKey löschen](../api/intune-onboarding-sideloadingkey-delete.md)|Keine|Löscht eine [SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).|
|[SideLoadingKey aktualisieren](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Aktualisieren Sie die Eigenschaften eines [SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Seite laden wichtige eindeutigen Bezeichner ab.|
|Wert|Zeichenfolge|Seite Laden von Schlüssel-Wert ist es 5 x 5-Wert durch Hiphens getrennt.|
|displayName|Zeichenfolge|Seite laden Schlüsselname der ITPro Admins angezeigt.|
|description|Zeichenfolge|Seite laden Schlüssel Beschreibung der ITPro Admins angezeigt.|
|totalActivation|Int32|Seite laden Key insgesamt Aktivierung der ITPro Admins angezeigt.|
|lastUpdatedDateTime|Zeichenfolge|Seite laden Schlüssel aktualisiert Datum der letzten die ITPro Admins angezeigt.|

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




