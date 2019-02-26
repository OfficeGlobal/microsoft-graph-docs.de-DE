---
title: targetedManagedAppConfiguration-Ressourcentyp
description: Konfiguration für das Übermitteln eines Satzes benutzerdefinierter Einstellungen an alle Benutzer in der Zielsicherheitsgruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdc5edf73d0d07cb4da6244e90b3d68b54c24812
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261572"
---
# <a name="targetedmanagedappconfiguration-resource-type"></a>targetedManagedAppConfiguration-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Konfiguration für das Übermitteln eines Satzes benutzerdefinierter Einstellungen an alle Benutzer in der Zielsicherheitsgruppe.


Erbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[targetedManagedAppConfigurations auflisten](../api/intune-mam-targetedmanagedappconfiguration-list.md)|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekte.|
|[TargetedManagedAppConfiguration abrufen](../api/intune-mam-targetedmanagedappconfiguration-get.md)|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.|
|[TargetedManagedAppConfiguration erstellen](../api/intune-mam-targetedmanagedappconfiguration-create.md)|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Erstellen eines neuen [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.|
|[TargetedManagedAppConfiguration löschen](../api/intune-mam-targetedmanagedappconfiguration-delete.md)|Keine|Löscht ein [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt.|
|[TargetedManagedAppConfiguration aktualisieren](../api/intune-mam-targetedmanagedappconfiguration-update.md)|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)|Aktualisieren der Eigenschaften eines [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)- Objekts.|
|[assign-Aktion](../api/intune-mam-targetedmanagedappconfiguration-assign.md)|Keiner|Noch nicht dokumentiert|
|[targetApps-Aktion](../api/intune-mam-targetedmanagedappconfiguration-targetapps.md)|Keiner|Noch nicht dokumentiert.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Anzeigename der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|description|Zeichenfolge|Beschreibung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Richtlinie Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|id|string|Schlüssel der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|Version|Zeichenfolge|Version der Entität Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|customSettings|[keyValuePair](../resources/intune-mam-keyvaluepair.md)-Sammlung|Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).|
|deployedAppCount|Int32|Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.|
|isAssigned|Boolean|Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|apps|Sammlung von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Liste der Apps, für die die Richtlinie bereitgestellt wurde|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md)|Navigationseigenschaft zu einer Bereitstellungsübersicht für die Konfiguration|
|assignments|Sammlung von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md)|Navigationseigenschaft zu einer Liste von Einschlussgruppen und Ausschlussgruppen, für die die Richtlinie bereitgestellt wurde.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```



