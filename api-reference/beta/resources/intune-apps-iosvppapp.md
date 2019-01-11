---
title: Ressourcentyp „iosVppApp“
description: Diese Ressource enthält die Eigenschaften und geerbten Eigenschaften einer iOS-VPP-App (Volume Purchase Program).
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8c85fe2220a9bbc9df6933951c779c5d898eadab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888749"
---
# <a name="iosvppapp-resource-type"></a>Ressourcentyp „iosVppApp“

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Ressource enthält die Eigenschaften und geerbten Eigenschaften einer iOS-VPP-App (Volume Purchase Program).

Sie erbt von [mobileApp](../resources/intune-apps-mobileapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „iosVppApp“](../api/intune-apps-iosvppapp-list.md)|Sammlung von Objekten des Typs[iosVppApp](../resources/intune-apps-iosvppapp.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [iosVppApp](../resources/intune-apps-iosvppapp.md) auf.|
|[Abrufen von „iosVppApp“](../api/intune-apps-iosvppapp-get.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [iosVppApp](../resources/intune-apps-iosvppapp.md).|
|[Erstellen von „iosVppApp“](../api/intune-apps-iosvppapp-create.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md)|Erstellt neue Objekte des Typs [iosVppApp](../resources/intune-apps-iosvppapp.md).|
|[Löschen von „iosVppApp“](../api/intune-apps-iosvppapp-delete.md)|Keiner|Löscht Objekte des Typs [iosVppApp](../resources/intune-apps-iosvppapp.md).|
|[Aktualisieren von „iosVppApp“](../api/intune-apps-iosvppapp-update.md)|[iosVppApp](../resources/intune-apps-iosvppapp.md)|Aktualisiert die Eigenschaften von Objekten des Typs [iosVppApp](../resources/intune-apps-iosvppapp.md).|
|[RevokeAllLicenses Aktion](../api/intune-apps-iosvppapp-revokealllicenses.md)|Keine|REVOKE alle zugewiesenen iOS lizenziert VPP für die angegebene app.|
|[RevokeUserLicense Aktion](../api/intune-apps-iosvppapp-revokeuserlicense.md)|Keine|REVOKE zugewiesen iOS VPP-Benutzerlizenz für die app zu reparieren.|
|[RevokeDeviceLicense Aktion](../api/intune-apps-iosvppapp-revokedevicelicense.md)|Keine|REVOKE zugewiesen iOS VPP Gerätenlizenz für app zu reparieren.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|displayName|Zeichenfolge|Der vom Administrator bereitgestellte oder importierte Titel der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|description|Zeichenfolge|Beschreibung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|publisher|Zeichenfolge|Der Herausgeber der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|isFeatured|Boolescher Wert|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|privacyInformationUrl|Zeichenfolge|URL zur Datenschutzerklärung. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|informationUrl|Zeichenfolge|URL zur Seite mit weiteren Informationen. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|owner|Zeichenfolge|Der Besitzer der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|developer|Zeichenfolge|Der Entwickler der App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|notes|Zeichenfolge|Hinweise zur App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|uploadState|Int32|Der Upload-Zustand. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|usedLicenseCount|Int32|Anzahl von VPP-Lizenzen, die aktuell verwendet werden.|
|totalLicenseCount|Int32|Gesamtanzahl von VPP-Lizenzen.|
|releaseDateTime|DateTimeOffset|Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.|
|appStoreUrl|Zeichenfolge|Store-URL|
|licensingType|[vppLicensingType](../resources/intune-apps-vpplicensingtype.md)|Unterstützter Lizenztyp|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosdevicetype.md)|Gültiger iOS-Gerätetyp|
|vppTokenOrganizationName|Zeichenfolge|Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist. Mögliche Werte sind: `business` und `education`. Mögliche Werte sind: `business` und `education`.|
|vppTokenAppleId|Zeichenfolge|Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist|
|bundleId|Zeichenfolge|Identitätsname|
|vppTokenId|Zeichenfolge|Bezeichner des Tokens VPP diese app zugeordnet.|
|revokeLicenseActionResults|[IosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) -Auflistung|Ergebnisse der widerrufen diese app-Lizenz Aktionen.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Die Installationszusammenfassung für die mobile App. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|deviceStatuses|[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) -Auflistung|Die Liste der Installationsstatus für diese mobile app. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|userStatuses|[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) -Auflistung|Die Liste der Installationsstatus für diese mobile app. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).|
|assignedLicenses|[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Auflistung|Die diese app zugewiesenen Lizenzen.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "releaseDateTime": "String (timestamp)",
  "appStoreUrl": "String",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "String",
  "vppTokenAccountType": "String",
  "vppTokenAppleId": "String",
  "bundleId": "String",
  "vppTokenId": "String",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "String",
      "managedDeviceId": "String",
      "totalLicensesCount": 1024,
      "failedLicensesCount": 1024,
      "actionFailureReason": "String",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ]
}
```





