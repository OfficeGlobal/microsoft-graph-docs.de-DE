---
title: Androidmanagedstoreaccountenterprisesettings hinzugefügt-Ressourcentyp
description: Enterprise-Einstellungen für ein Android-Konto mit verwaltetem Speicher.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd6f278963bd37276b808f221d1902fd82e23a48
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159136"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>Androidmanagedstoreaccountenterprisesettings hinzugefügt-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enterprise-Einstellungen für ein Android-Konto mit verwaltetem Speicher.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Androidmanagedstoreaccountenterprisesettings hinzugefügt abrufen](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|Lesen von Eigenschaften und Beziehungen des [androidmanagedstoreaccountenterprisesettings hinzugefügt](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekts.|
|[Androidmanagedstoreaccountenterprisesettings hinzugefügt aktualisieren](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|Aktualisieren der Eigenschaften eines [androidmanagedstoreaccountenterprisesettings hinzugefügt](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) -Objekts.|
|[Aktion „requestSignupUrl“](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|Zeichenfolge|Noch nicht dokumentiert|
|[Aktion „completeSignup“](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|Keine|Noch nicht dokumentiert|
|[Aktion „syncApps“](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|Keine|Noch nicht dokumentiert|
|[Aktion „unbind“](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|Keiner|Noch nicht dokumentiert|
|[createGooglePlayWebToken-Aktion](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|Zeichenfolge|Generiert ein webtoken, das in einer einbettbaren Komponente verwendet wird.|
|[setAndroidDeviceOwnerFullyManagedEnrollmentState-Aktion](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-setandroiddeviceownerfullymanagedenrollmentstate.md)|Keine|Legt die Androidmanagedstoreaccountenterprisesettings hinzugefügt-AndroidDeviceOwnerFullyManagedEnrollmentEnabled auf den angegebenen Wert fest.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Das Android Store-Konto Enterprise-Einstellungs-ID|
|bindStatus|[androidManagedStoreAccountBindStatus](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|Binden des Status des Mandanten mit der Google EMM-API. Mögliche Werte: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde.|
|lastAppSyncStatus|[androidManagedStoreAccountAppSyncStatus](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|Ergebnis der letzten Anwendungssynchronisierung. Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.|
|ownerUserPrincipalName|Zeichenfolge|Besitzer-UPN, der das Unternehmen erstellt hat|
|ownerOrganizationName|Zeichenfolge|Name der Organisation, die beim Onboarding von Android Enterprise verwendet wird|
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt der letzten Änderung für Android Enterprise-Einstellungen|
|enrollmentTarget|[androidManagedStoreAccountEnrollmentTarget](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|Gibt an, welche Benutzer Geräte in der Android Enterprise-Geräteverwaltung registrieren können. Mögliche Werte: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Zeichenfolgenauflistung|Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.|
|deviceOwnerManagementEnabled|Boolescher Wert|Gibt an, ob dieses Konto für die Verwaltung von Android-Geräte Besitzern mit CloudDPC läuft.|
|companyCodes|[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) -Sammlung|Buchungskreise für Androidmanagedstoreaccountenterprisesettings hinzugefügt|
|androidDeviceOwnerFullyManagedEnrollmentEnabled|Boolescher Wert|Buchungskreise für Androidmanagedstoreaccountenterprisesettings hinzugefügt|

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
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "String",
      "qrCodeContent": "String",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "String",
        "value": "binary"
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```




