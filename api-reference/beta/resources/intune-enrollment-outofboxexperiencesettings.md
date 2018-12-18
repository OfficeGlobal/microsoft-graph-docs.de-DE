---
title: Ressourcentyp outOfBoxExperienceSettings
description: Erleben Sie die Einstellung im Lieferzustand
author: tfitzmac
ms.openlocfilehash: 545fbe5c27063397a4d08c40729227804ebfc56d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308407"
---
# <a name="outofboxexperiencesettings-resource-type"></a>Ressourcentyp outOfBoxExperienceSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Erleben Sie die Einstellung im Lieferzustand
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|hidePrivacySettings|Boolesch|Zeigen Sie an oder blenden Sie der datenschutzeinstellungen für Benutzer aus|
|hideEULA|Boolesch|Anzeigen oder Ausblenden der Endbenutzer-Lizenzvertrag für Benutzer|
|userType|[windowsUserType](../resources/intune-enrollment-windowsusertype.md)|Typ des Benutzers. Mögliche Werte sind: `administrator` und `standard`.|
|deviceUsageType|[windowsDeviceUsageType](../resources/intune-enrollment-windowsdeviceusagetype.md)|AAD Join-Authentifizierungstyp. Mögliche Werte sind: `singleUser` und `shared`.|
|skipKeyboardSelectionPage|Boolesch|Wenn die Seite Set, und klicken Sie dann auf der Tastaturauswahl überspringen, wenn Sprache und Region festgelegt sind|
|hideEscapeLink|Boolesch|Wenn auf True festgelegt, klicken Sie dann den Benutzer über mit anderen Konto auf Unternehmens-Anmeldung nicht gestartet werden kann|

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





