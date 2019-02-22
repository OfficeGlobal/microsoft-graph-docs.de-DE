---
title: Aktualisieren von „androidForWorkSettings“
description: Aktualisiert die Eigenschaften eines androidForWorkSettings-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65550bc588eb5fb0f4d2f11ac785d458e8821a7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170791"
---
# <a name="update-androidforworksettings"></a>Aktualisieren von „androidForWorkSettings“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisiert die Eigenschaften eines [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)-Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementConfiguration.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)-Objekts an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) erforderlich sind.

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



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```




