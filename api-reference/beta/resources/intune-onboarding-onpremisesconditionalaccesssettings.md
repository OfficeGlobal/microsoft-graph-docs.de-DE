---
title: onPremisesConditionalAccessSettings-Ressourcentyp
description: Einzelne Entität, die die Exchange-Einstellungen für lokalen bedingten Zugriff für einen Mandanten darstellt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7463abbf44be7db8d94deac0ae22db8fe378493a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150631"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a>onPremisesConditionalAccessSettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Einzelne Entität, die die Exchange-Einstellungen für lokalen bedingten Zugriff für einen Mandanten darstellt.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[onpremisesConditionalAccessSettings abrufen](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Lesen von Eigenschaften und Beziehungen des [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.|
|[onPremisesConditionalAccessSettings aktualisieren](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[onpremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Noch nicht dokumentiert|
|enabled|Boolescher Wert|Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.|
|includedGroups|GUID-Sammlung|Benutzergruppen, für die der lokale bedingte Zugriff gilt. Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.|
|excludedGroups|GUID-Sammlung|Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden. Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.|
|overrideDefaultRule|Boolean|Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```




