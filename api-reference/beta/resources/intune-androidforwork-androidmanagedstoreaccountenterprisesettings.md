---
title: Ressourcentyp androidManagedStoreAccountEnterpriseSettings
description: Enterprise-Einstellungen für eine Android verwaltete Konto anmelden.
ms.openlocfilehash: 976e4e2ea9d6e01a81f8f821388a1d4390908754
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062756"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>Ressourcentyp androidManagedStoreAccountEnterpriseSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enterprise-Einstellungen für eine Android verwaltete Konto anmelden.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|Lesen Sie Eigenschaften und Beziehungen des [AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekts.|
|[AndroidManagedStoreAccountEnterpriseSettings aktualisieren](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|Aktualisieren Sie die Eigenschaften eines [AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekts.|
|[Aktion „requestSignupUrl“](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String|Noch nicht dokumentiert|
|[Aktion „completeSignup“](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|Keiner|Noch nicht dokumentiert|
|[Aktion „syncApps“](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|Keiner|Noch nicht dokumentiert|
|[Aktion „unbind“](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|Keiner|Noch nicht dokumentiert|
|[CreateGooglePlayWebToken Aktion](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String|Generiert ein Web-Token, das verwendet wird, in eine Komponente eingebettet werden.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Die Android Enterprise-Konto-ID Einstellungen speichern|
|bindStatus|[androidManagedStoreAccountBindStatus](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|Status des Mandanten mit der Google EMM-API zu binden. Mögliche Werte: sind `notBound`, `bound`, `boundAndValidated` und `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde.|
|lastAppSyncStatus|[androidManagedStoreAccountAppSyncStatus](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|Letzte Anwendung Sync Ergebnis. Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.|
|ownerUserPrincipalName|String|Besitzer-UPN, der das Unternehmen erstellt hat|
|ownerOrganizationName|String|Name der Organisation verwendet, wenn Onboarding Android Enterprise|
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt der letzten Änderung für Android Enterprise-Einstellungen|
|enrollmentTarget|[androidManagedStoreAccountEnrollmentTarget](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|Gibt an, welche Benutzer Geräte in Android Enterprise Gerätemanagement registrieren können. Mögliche Werte: sind `none`, `all`, `targeted` und `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Zeichenfolgenauflistung|Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.|
|deviceOwnerManagementEnabled|Boolesch|Gibt an, ob dieses Konto für Android Besitzer Gerätemanagement mit CloudDPC flighting ist.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAccountEnterpriseSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
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





