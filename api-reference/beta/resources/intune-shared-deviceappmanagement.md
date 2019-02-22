---
title: Ressourcentyp „deviceAppManagement“
description: Singleton-Entität, die als Container für alle Funktionen zur Verwaltung von Apps auf Geräten fungiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a6d4557fb77ecc7a9f635688046b267d08c16d78
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145178"
---
# <a name="deviceappmanagement-resource-type"></a>Ressourcentyp „deviceAppManagement“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Singleton-Entität, die als Container für alle Funktionen zur Verwaltung von Apps auf Geräten fungiert

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von „deviceAppManagement“](../api/intune-shared-deviceappmanagement-get.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).|
|[Aktualisieren von „deviceAppManagement“](../api/intune-shared-deviceappmanagement-update.md)|Aktualisiert die Eigenschaften von Objekten des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).|
|**Onboarding**|
|[Aktion „syncMicrosoftStoreForBusinessApps“](../api/intune-shared-deviceappmanagement-syncmicrosoftstoreforbusinessapps.md)|Keiner|Synchronisiert Intune-Konten mit dem Microsoft Store für Unternehmen.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|**Onboarding**|
|isEnabledForMicrosoftStoreForBusiness|Boolescher Wert|Gibt an, ob das Konto Anwendungen mit dem Microsoft Store für Unternehmen synchronisieren darf.|
|microsoftStoreForBusinessLanguage|String|Die Gebietsschemainformationen, die zur Synchronisierung von Anwendungen mit dem Microsoft Store für Unternehmen verwendet werden. Angegeben werden Kulturen, die für ein Land bzw. eine Region spezifisch sind. Die Namen dieser Kulturen folgen dem Standard RFC 4646 (Windows Vista und höher). Das Format lautet <languagecode2>-<country/regioncode2>. Dabei ist <languagecode2> ein klein geschriebener Code aus zwei Buchstaben nach ISO 639-1 und <country/regioncode2> ein groß geschriebener Code aus zwei Buchstaben nach ISO 3166. Beispiel für eine spezifische Kultur: „en-US“ für „Englisch (Vereinigte Staaten)“.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|Zeitpunkt der letzten Anwendungssynchronisierung mit dem Microsoft Store für Unternehmen|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|Zeitpunkt, zu dem das Konto die Apps letztmals erfolgreich mit dem Microsoft Store für Unternehmen synchronisiert hat|
|microsoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|Die Informationen zum Endbenutzer Portal werden zum Synchronisieren von Anwendungen aus dem Microsoft Store for Business zum InTune-Unternehmensportal verwendet. Es gibt drei Optionen zum Auswählen von \["nur Unternehmensportal", "Unternehmensportal und privater Speicher", "nur privater Speicher"\]. Mögliche Werte sind: `none`, `companyPortal` und `privateStore`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|**Apps**|
|enterpriseCodeSigningCertificates|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) -Sammlung|Das Windows Enterprise-Code Signaturzertifikat.|
|iosLobAppProvisioningConfigurations|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Sammlung|Die Konfigurationen der IOS-Branchen-App-Konfiguration.|
|mobileAppCategories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)-Sammlung|Die Kategorien der mobilen Apps.|
|mobileAppConfigurations|[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Sammlung|Die Konfigurationen der mobilen Apps für verwaltete Geräte.|
|mobileApps|[mobileApp](../resources/intune-apps-mobileapp.md)-Sammlung|Die mobilen Apps.|
|symantecCodeSigningCertificate|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Das WinPhone Symantec-Code Signaturzertifikat.|
|**Bücher**|
|managedEBooks|[managedEBook](../resources/intune-books-managedebook.md)-Sammlung|Das verwaltete E-Book|
|Mobileappconfigurations|[managedEBookCategory](../resources/intune-books-managedebookcategory.md) -Sammlung|Die mobilen eBook-Kategorien.|
|**deviceManagement**|
|windowsManagementApp|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Windows-Verwaltungs-app.|
|**Mobile App Management (MAM)**|
|androidManagedAppProtections|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md)-Sammlung|Richtlinien verwalteter Android-Apps|
|defaultManagedAppProtections|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md)-Sammlung|Standardrichtlinien verwalteter Apps|
|iosManagedAppProtections|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md)-Sammlung|Richtlinien verwalteter iOS-Apps|
|managedAppPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)-Sammlung|Richtlinien verwalteter Apps|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)-Sammlung|Die Registrierungen verwalteter Apps|
|managedAppStatuses|[managedAppStatus](../resources/intune-mam-managedappstatus.md)-Sammlung|Die Status der verwalteten Apps|
|mdmWindowsInformationProtectionPolicies|[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md)-Sammlung|Windows Information Protection für Apps auf in MDM registrierten Geräten|
|targetedManagedAppConfigurations|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Sammlung|Zielkonfigurationen verwalteter Apps|
|windowsInformationProtectionPolicies|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)-Sammlung|Windows Information Protection für Apps auf nicht in MDM registrierten Geräten|
|**Onboarding**|
|sideLoadingKeys|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Sammlung|Seiten Ladeschlüssel, die für die Windows 8-und 8,1-apps-Installation erforderlich sind.|
|vppTokens|[VppToken](../resources/intune-onboarding-vpptoken.md)-Sammlung|Liste von Vpp-Token für diese Organisation.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.  Beachten Sie, dass dies nur ein Beispiel ist. Abfrage Antworten auf tatsächliche Abfragen enthalten die für den Kontext geeigneten Eigenschaften.  
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```



