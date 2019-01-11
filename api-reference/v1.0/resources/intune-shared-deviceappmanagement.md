---
title: Ressourcentyp „deviceAppManagement“
description: Singleton-Entität, die als Container für alle Funktionen zur Verwaltung von Apps auf Geräten fungiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 60acbdb63f3bd75bacbc2d2392cbb3ab64cc4b57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825648"
---
# <a name="deviceappmanagement-resource-type"></a>Ressourcentyp „deviceAppManagement“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|**Apps**|
|mobileAppCategories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)-Sammlung|Die Kategorien der mobilen Apps.|
|mobileAppConfigurations|[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Sammlung|Die Konfigurationen der mobilen Apps für verwaltete Geräte.|
|mobileApps|[mobileApp](../resources/intune-apps-mobileapp.md)-Sammlung|Die mobilen Apps.|
|**Bücher**|
|managedEBooks|[managedEBook](../resources/intune-books-managedebook.md)-Sammlung|Das verwaltete E-Book|
|**Mobile app-Verwaltung (MAM)**|
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
|vppTokens|[VppToken](../resources/intune-onboarding-vpptoken.md)-Sammlung|Liste von Vpp-Token für diese Organisation.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.  Beachten Sie, dass dies nur ein Beispiel ist. Abfrageantworten an tatsächlichen Abfragen enthält die Eigenschaften für den Kontext geeignet.  
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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



