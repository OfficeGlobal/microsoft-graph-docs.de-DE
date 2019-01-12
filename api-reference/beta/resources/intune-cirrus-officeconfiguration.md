---
title: Ressourcentyp officeConfiguration
description: Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 767782e26dd203e2ab5488b30520d8cbcf44d1e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921360"
---
# <a name="officeconfiguration-resource-type"></a>Ressourcentyp officeConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|Abrufen von officeConfiguration|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md) -Objekts.|
|OfficeConfiguration aktualisieren|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|ID des Office-Konfiguration.|
|tenantCheckinStatuses|[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung|Liste der Office-Client Einchecken Status.|
|tenantUserCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Entität, die Mandanten Einchecken Statuen beschreibt.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|clientConfigurations|[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Auflistung|Liste der Office-Client-Konfiguration.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
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
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```



