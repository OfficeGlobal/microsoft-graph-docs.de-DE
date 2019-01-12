---
title: Ressourcentyp advancedThreatProtectionOnboardingStateSummary
description: Windows Defender erweiterte Threat Protection Onboarding Übersicht über das Konto.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c308f91862e1d709d92a45d0a83148df5c23fd88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966601"
---
# <a name="advancedthreatprotectiononboardingstatesummary-resource-type"></a>Ressourcentyp advancedThreatProtectionOnboardingStateSummary

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Windows Defender erweiterte Threat Protection Onboarding Übersicht über das Konto.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von advancedThreatProtectionOnboardingStateSummary](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Lesen Sie Eigenschaften und Beziehungen des [AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekts.|
|[AdvancedThreatProtectionOnboardingStateSummary aktualisieren](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-update.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Aktualisieren Sie die Eigenschaften eines [AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner|
|unknownDeviceCount|Int32|Anzahl von unbekannten Geräten|
|notApplicableDeviceCount|Int32|Anzahl der ausgenommenen Geräte|
|compliantDeviceCount|Int32|Anzahl von konformen Geräten|
|remediatedDeviceCount|Int32|Anzahl von korrigierten Geräten|
|nonCompliantDeviceCount|Int32|Anzahl von nicht konformen Geräten|
|errorDeviceCount|Int32|Anzahl von Geräten mit Fehlern|
|conflictDeviceCount|Int32|Anzahl von Geräten mit Konflikt|
|notAssignedDeviceCount|Int32|Anzahl der nicht zugewiesenen Geräte|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|advancedThreatProtectionOnboardingDeviceSettingStates|[AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) -Auflistung|Noch nicht dokumentiert.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notAssignedDeviceCount": 1024
}
```





