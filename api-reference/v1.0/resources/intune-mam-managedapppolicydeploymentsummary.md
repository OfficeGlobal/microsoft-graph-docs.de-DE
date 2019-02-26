---
title: managedAppPolicyDeploymentSummary-Ressourcentyp
description: ManagedAppEntity ist der Basisentitätstyp für alle anderen Entitätstypen im App-Verwaltungsworkflow.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 84ca52db1321bc3a2fa356de50e1446f662e725b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256371"
---
# <a name="managedapppolicydeploymentsummary-resource-type"></a>managedAppPolicyDeploymentSummary-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|string|Schlüssel der Entität|
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



