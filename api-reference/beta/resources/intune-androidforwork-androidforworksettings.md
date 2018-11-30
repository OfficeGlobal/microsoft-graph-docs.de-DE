---
title: Ressourcentyp „androidForWorkSettings“
description: Einstellungen für Android for Work
ms.openlocfilehash: 3c7aca729f145bb69447e442b7daddbfcf90c8c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058780"
---
# <a name="androidforworksettings-resource-type"></a>Ressourcentyp „androidForWorkSettings“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Einstellungen für Android for Work
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von „androidForWorkSettings“](../api/intune-androidforwork-androidforworksettings-get.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Liest Eigenschaften und Beziehungen des Objekts [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Aktualisieren von „androidForWorkSettings“](../api/intune-androidforwork-androidforworksettings-update.md)|[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)|Aktualisiert die Eigenschaften eines Objekts des Typs [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).|
|[Aktion „requestSignupUrl“](../api/intune-androidforwork-androidforworksettings-requestsignupurl.md)|String|Noch nicht dokumentiert|
|[Aktion „completeSignup“](../api/intune-androidforwork-androidforworksettings-completesignup.md)|Keiner|Noch nicht dokumentiert|
|[Aktion „syncApps“](../api/intune-androidforwork-androidforworksettings-syncapps.md)|Keiner|Noch nicht dokumentiert|
|[Aktion „unbind“](../api/intune-androidforwork-androidforworksettings-unbind.md)|Keiner|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Android for Work-Einstellungsbezeichner.|
|bindStatus|[androidForWorkBindStatus](../resources/intune-androidforwork-androidforworkbindstatus.md)|Status des Mandanten mit der Google EMM-API zu binden. Mögliche Werte: sind `notBound`, `bound`, `boundAndValidated` und `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde.|
|lastAppSyncStatus|[androidForWorkSyncStatus](../resources/intune-androidforwork-androidforworksyncstatus.md)|Letzte Anwendung Sync Ergebnis. Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.|
|ownerUserPrincipalName|String|Besitzer-UPN, der das Unternehmen erstellt hat|
|ownerOrganizationName|String|Organisationsname, der beim Android for Work-Onboarding verwendet wird|
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt, zu dem die Android for Work-Einstellungen zuletzt geändert wurden|
|enrollmentTarget|[androidForWorkEnrollmentTarget](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|Gibt an, welche Benutzer Geräte in Android für die Verwaltung von Geräten registrieren können. Mögliche Werte: sind `none`, `all`, `targeted` und `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Zeichenfolgenauflistung|Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.|
|deviceOwnerManagementEnabled|Boolesch|Gibt an, ob dieses Konto für Android Besitzer Gerätemanagement mit CloudDPC flighting ist.|

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





