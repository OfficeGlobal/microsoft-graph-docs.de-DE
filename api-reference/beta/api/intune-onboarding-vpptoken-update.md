---
title: VppToken aktualisieren
description: Aktualisieren der Eigenschaften eines vppToken-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4af4f4fdc8bb814614ebd2980a0117e1f8003cba
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147663"
---
# <a name="update-vpptoken"></a>VppToken aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [vppToken](../resources/intune-onboarding-vpptoken.md)-Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

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
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Wird automatisch generiert, wenn AppleVolumePurchaseProgramToken erstellt wird. Schlüssel der Entität.|
|organizationName|Zeichenfolge|Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist. Mögliche Werte sind: `business` und `education`. Mögliche Werte sind: `business` und `education`.|
|appleId|Zeichenfolge|Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.|
|expirationDateTime|DateTimeOffset|Ablaufdatum und -uhrzeit des Apple Volume Purchase Program-Token.|
|lastSyncDateTime|DateTimeOffset|Zeitpunkt der letzten Synchronisierung der Anwendung mit dem Apple Volume Purchase Program Service mithilfe des Apple Volume Purchase Program-Token.|
|token|Zeichenfolge|Aus dem Apple Volume Purchase Program heruntergeladene Zeichenfolge des Apple Volume Purchase Program-Token.|
|lastModifiedDateTime|DateTimeOffset|Letztes Änderungsdatum und letzter Änderungszeitpunkt des Apple Volume Purchase Program-Token.|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Aktueller Stand des Apple Volume Purchase Program-Token. Mögliche Werte: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Mögliche Werte: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|tokenActionResults|[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) -Sammlung|Die Sammlung von Status der Aktionen, die für das Apple Volume Purchase Program-Token ausgeführt wurden.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Aktueller Synchronisierungsstatus seit der letzten Synchronisierung der Anwendung, die mit dem Apple Volume Purchase Program-Token durchgeführt wurde. Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`. Mögliche Werte sind: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Boolean|Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.|
|countryOrRegion|String|Angabe, ob Anwendungen für das VPP-Token automatisch aktualisiert werden.|
|dataSharingConsentGranted|Boolescher Wert|Einwilligung zur Datenfreigabe mit dem Apple Volume Purchase-Programm.|
|displayName|Zeichenfolge|Ein vom Administrator angegebener, von Token angezeigter Name.|
|LocationName|Zeichenfolge|Von Apple VSS zurückgegebener Tokensort.|
|claimTokenManagementFromExternalMdm|Boolescher Wert|Zustimmung des Administrators, um die Forderungs Tokenverwaltung über externes MDM zu ermöglichen.|
|Rolescopetagids zur|String collection|Rollenbereichs Tags-IDs, die dieser Entität zugewiesen sind.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [vppToken](../resources/intune-onboarding-vpptoken.md) im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
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
HTTP/1.1 200 OK
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




