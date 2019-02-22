---
title: Ressourcentyp „androidForWorkSettings“
description: Einstellungen für Android for Work
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 016b0c727afb5a4c1864c8e02b91491c54f42b77
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165709"
---
# <a name="androidforworksettings-resource-type"></a>Ressourcentyp „androidForWorkSettings“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Einstellungen für Android for Work

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von „androidForWorkSettings“](../api/intune-androidforwork-androidforworksettings-get.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Liest Eigenschaften und Beziehungen des Objekts [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Aktualisieren von „androidForWorkSettings“](../api/intune-androidforwork-androidforworksettings-update.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Aktualisiert die Eigenschaften eines Objekts des Typs [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Aktion „requestSignupUrl“](../api/intune-androidforwork-androidforworksettings-requestsignupurl.md)|String|Noch nicht dokumentiert|
|[Aktion „completeSignup“](../api/intune-androidforwork-androidforworksettings-completesignup.md)|Keine|Noch nicht dokumentiert|
|[Aktion „syncApps“](../api/intune-androidforwork-androidforworksettings-syncapps.md)|Keine|Noch nicht dokumentiert|
|[Aktion „unbind“](../api/intune-androidforwork-androidforworksettings-unbind.md)|Keiner|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Android for Work-Einstellungsbezeichner.|
|bindStatus|[androidForWorkBindStatus](../resources/intune-androidforwork-androidforworkbindstatus.md)|Binden des Status des Mandanten mit der Google EMM-API. Mögliche Werte: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde.|
|lastAppSyncStatus|[androidForWorkSyncStatus](../resources/intune-androidforwork-androidforworksyncstatus.md)|Ergebnis der letzten Anwendungssynchronisierung. Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.|
|ownerUserPrincipalName|Zeichenfolge|Besitzer-UPN, der das Unternehmen erstellt hat|
|ownerOrganizationName|Zeichenfolge|Organisationsname, der beim Android for Work-Onboarding verwendet wird|
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt, zu dem die Android for Work-Einstellungen zuletzt geändert wurden|
|enrollmentTarget|[androidForWorkEnrollmentTarget](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|Gibt an, welche Benutzer Geräte in Android für die Arbeitsgeräte Verwaltung registrieren können. Mögliche Werte: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Zeichenfolgenauflistung|Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.|
|deviceOwnerManagementEnabled|Boolescher Wert|Gibt an, ob dieses Konto für die Verwaltung von Android-Geräte Besitzern mit CloudDPC läuft.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": true
}
```




