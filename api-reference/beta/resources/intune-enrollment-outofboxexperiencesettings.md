---
title: Ressourcentyp outOfBoxExperienceSettings
description: Erleben Sie die Einstellung im Lieferzustand
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af276dd520df9ee3b257650e703813de355bed9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882733"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Ressourcentyp outOfBoxExperienceSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Erleben Sie die Einstellung im Lieferzustand
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|hidePrivacySettings|Boolescher Wert|Zeigen Sie an oder blenden Sie der datenschutzeinstellungen für Benutzer aus|
|hideEULA|Boolescher Wert|Anzeigen oder Ausblenden der Endbenutzer-Lizenzvertrag für Benutzer|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Typ des Benutzers. Mögliche Werte sind: `administrator` und `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD Join-Authentifizierungstyp. Mögliche Werte sind: `singleUser` und `shared`.|
|skipKeyboardSelectionPage|Boolescher Wert|Wenn die Seite Set, und klicken Sie dann auf der Tastaturauswahl überspringen, wenn Sprache und Region festgelegt sind|
|hideEscapeLink|Boolescher Wert|Wenn auf True festgelegt, klicken Sie dann den Benutzer über mit anderen Konto auf Unternehmens-Anmeldung nicht gestartet werden kann|

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





