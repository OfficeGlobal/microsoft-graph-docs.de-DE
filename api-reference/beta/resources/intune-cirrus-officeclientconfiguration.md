---
title: Ressourcentyp officeClientConfiguration
description: Office-Client-Konfiguration.
author: tfitzmac
ms.openlocfilehash: 67a7845a2e0327e2e5de37d424274f6e2ee35604
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303836"
---
# <a name="officeclientconfiguration-resource-type"></a>Ressourcentyp officeClientConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Office-Client-Konfiguration.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste officeClientConfigurations](../api/intune-cirrus-officeclientconfiguration-list.md)|[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Objekte.|
|[Abrufen von officeClientConfiguration](../api/intune-cirrus-officeclientconfiguration-get.md)|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Objekts.|
|[assign-Aktion](../api/intune-cirrus-officeclientconfiguration-assign.md)|[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung|Ersetzen Sie alle Gruppen für eine Richtlinie.|
|[UpdatePriorities Aktion](../api/intune-cirrus-officeclientconfiguration-updatepriorities.md)|Keines|Aktualisieren Sie die Richtlinie Prioritäten.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|ID des die Richtlinie Office-Client-Konfiguration.|
|userPreferencePayload|Stream|Vorgaben JSON-Zeichenfolge im Binärformat, können diese Werte vom Benutzer außer Kraft gesetzt werden.|
|policyPayload|Stream|Richtlinieneinstellungen für JSON-Zeichenfolge im Binärformat, diese Werte können nicht vom Benutzer geändert werden.|
|description|String|Noch nicht dokumentiert|
|displayName|String|Admin bereitgestellte Beschreibung für den Office-Client Konfigurationsrichtlinie.|
|lastModifiedDateTime|DateTime|Zuletzt geänderte Datetime-Stempel der Richtlinie.|
|Priorität|Int32|Prioritätswert sollte eindeutigen Wert für jede Richtlinie unter einem Mandanten sein und für konfliktlösung verwendet werden, niedrigere Werte bedeuten, dass Priorität hoch ist.|
|userCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Benutzer Einchecken Zusammenfassung für die Richtlinie ein.|
|checkinStatuses|[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung|Liste der Office-Client Einchecken Status.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Auflistung|Die Liste der zugewiesenen Gruppe für die Richtlinie ein.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfiguration",
  "id": "String (identifier)",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "String",
  "displayName": "String",
  "priority": 1024,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ]
}
```



