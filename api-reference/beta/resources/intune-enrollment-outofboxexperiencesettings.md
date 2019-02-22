---
title: Dem outofboxexperiencesettings-Ressourcentyp
description: Einstellung für die Out-of-Box-Erfahrung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1148ba609a6533dcc6cedb9abd50e9191dceb5d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145528"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Dem outofboxexperiencesettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Einstellung für die Out-of-Box-Erfahrung

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|hidePrivacySettings|Boolescher Wert|Ein-oder Ausblenden von Datenschutzeinstellungen für Benutzer|
|hideEULA|Boolescher Wert|Ein-oder Ausblenden des EULAs für Benutzer|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Benutzertyp. Mögliche Werte sind: `administrator` und `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD-Join-Authentifizierungstyp. Mögliche Werte sind: `singleUser` und `shared`.|
|skipKeyboardSelectionPage|Boolescher Wert|Wenn diese Einstellung festgelegt ist, überspringen Sie die Seite mit der Tastaturauswahl, wenn Sprache und Region festgelegt sind.|
|hideEscapeLink|Boolescher Wert|Wenn dieser Wert auf "true" festgelegt ist, kann der Benutzer nicht mit einem anderen Konto als bei der Unternehmensanmeldung beginnen.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```




