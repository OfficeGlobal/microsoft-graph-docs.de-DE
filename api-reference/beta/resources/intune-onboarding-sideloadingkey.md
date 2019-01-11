---
title: Ressourcentyp sideLoadingKey
description: SideLoadingKey Entität ist für Windows 8 und Anwendungsservercomputern installiert Zeile des Geschäfts-Apps für einen Mandanten 8.1 Geräte erforderlich.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b08715ebc8cd19ab4086fd82013301ed89efd183
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814252"
---
# <a name="sideloadingkey-resource-type"></a>Ressourcentyp sideLoadingKey

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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





