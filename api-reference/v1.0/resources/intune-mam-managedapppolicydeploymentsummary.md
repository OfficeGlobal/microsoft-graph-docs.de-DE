---
title: managedAppPolicyDeploymentSummary-Ressourcentyp
description: ManagedAppEntity ist der Basisentitätstyp für alle anderen Entitätstypen im App-Verwaltungsworkflow.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ded5ab6bfb4cbd744bfab9a614f3122c8d1ab53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957480"
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
|displayName|Zeichenfolge|Noch nicht dokumentiert|
|configurationDeployedUserCount|Int32|Noch nicht dokumentiert|
|lastRefreshTime|DateTimeOffset|Noch nicht dokumentiert|
|configurationDeploymentSummaryPerApp|Collection von Objekten des Typs [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)|Noch nicht dokumentiert|
|id|Zeichenfolge|Schlüssel der Entität|
|Version|Zeichenfolge|Version der Entität|

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



