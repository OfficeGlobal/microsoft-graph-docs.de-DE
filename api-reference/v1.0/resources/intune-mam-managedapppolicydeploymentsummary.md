---
title: managedAppPolicyDeploymentSummary-Ressourcentyp
description: ManagedAppEntity ist der Basisentitätstyp für alle anderen Entitätstypen im App-Verwaltungsworkflow.
author: tfitzmac
ms.openlocfilehash: 1714a98e4ea6aa04eb7a91c4b6aace1dc78c01fc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302156"
---
# <a name="managedapppolicydeploymentsummary-resource-type"></a>managedAppPolicyDeploymentSummary-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

ManagedAppEntity ist der Basisentitätstyp für alle anderen Entitätstypen im App-Verwaltungsworkflow.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAppPolicyDeploymentSummary abrufen](../api/intune-mam-managedapppolicydeploymentsummary-get.md)|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Lesen von Eigenschaften und Beziehungen des [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)-Objekts.|
|[managedAppPolicyDeploymentSummary aktualisieren](../api/intune-mam-managedapppolicydeploymentsummary-update.md)|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Aktualisieren der Eigenschaften eines [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Noch nicht dokumentiert|
|configurationDeployedUserCount|Int32|Noch nicht dokumentiert|
|lastRefreshTime|DateTimeOffset|Noch nicht dokumentiert|
|configurationDeploymentSummaryPerApp|Collection von Objekten des Typs [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)|Noch nicht dokumentiert|
|id|String|Schlüssel der Entität|
|Version|String|Version der Entität|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "String",
  "configurationDeployedUserCount": 1024,
  "lastRefreshTime": "String (timestamp)",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "String"
      },
      "configurationAppliedUserCount": 1024
    }
  ],
  "id": "String (identifier)",
  "version": "String"
}
```



