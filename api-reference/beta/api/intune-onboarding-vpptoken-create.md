---
title: VppToken erstellen
description: Erstellen Sie ein neues VppToken-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31717a52cf66fdd0c4d2eff0717250a131540e9f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964423"
---
# <a name="create-vpptoken"></a>VppToken erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen Sie ein neues [VppToken](../resources/intune-onboarding-vpptoken.md)-Objekt.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des vppToken-Objekts an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des vppToken erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Dies wird automatisch generiert, wenn das appleVolumePurchaseProgramToken erstellt wird. Es ist der Schlüssel für die Entität.|
|organizationName|Zeichenfolge|Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist. Mögliche Werte sind: `business` und `education`. Mögliche Werte sind: `business` und `education`.|
|appleId|String|Die Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.|
|expirationDateTime|DateTimeOffset|Ablaufdatum und -Uhrzeit des Apple Volume Purchase Program-Tokens|
|lastSyncDateTime|DateTimeOffset|Der Zeitpunkt der letzten Anwendungssynchronisierung mit dem Apple Volume Purchase Program-Dienst mithilfe des Apple Volume Purchase Program-Tokens.|
|token|String|Die Zeichenfolge des Apple Volume Purchase Program-Tokens, die vom Apple Volume Purchase Program heruntergeladen wurde.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung, die dem Apple Volume Purchase Program-Token zugeordnet sind.|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Aktueller Status des Apple Volume Purchase Program-Tokens. Mögliche Werte: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Mögliche Werte: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|tokenActionResults|[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) -Sammlung|Die Sammlung von Status der Aktionen, die für das Apple Volume Purchase Program-Token ausgeführt wurden.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Aktueller Synchronisierungsstatus der letzten Anwendungssynchronisierung, die mit dem Apple Volume Purchase Program-Token ausgelöst wurde. Mögliche Werte sind: `none`, `inProgress`, `completed` und `failed`. Mögliche Werte sind: `none`, `inProgress`, `completed` und `failed`.|
|automaticallyUpdateApps|Boolean|Gibt an, ob Apps für das VPP-Token automatisch aktualisiert werden.|
|countryOrRegion|String|Gibt an, ob Apps für das VPP-Token automatisch aktualisiert werden.|
|dataSharingConsentGranted|Boolescher Wert|Einwilligung zur Datenfreigabe mit dem Apple Volume Purchase-Programm.|
|displayName|Zeichenfolge|Ein vom Administrator angegebener, von Token angezeigter Name.|
|LocationName|String|Von Apple VSS zurückgegebener Tokensort.|
|claimTokenManagementFromExternalMdm|Boolescher Wert|Zustimmung des Administrators, um die Forderungs Tokenverwaltung über externes MDM zu ermöglichen.|
|Rolescopetagids zur|String collection|Rollenbereichs Tags-IDs, die dieser Entität zugewiesen sind.|



## <a name="response"></a>Antwort
Bei Erfolg gibt diese Methode den Antwortcode `201 Created` und ein [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 1002

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1115

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




