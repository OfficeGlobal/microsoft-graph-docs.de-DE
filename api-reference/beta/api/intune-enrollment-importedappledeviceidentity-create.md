---
title: Erstellen von importedAppleDeviceIdentity
description: Erstellen eines neuen ImportedAppleDeviceIdentity-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cf6f897d44774ceba92b2d2c965f7cc561001383
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925079"
---
# <a name="create-importedappledeviceidentity"></a>Erstellen von importedAppleDeviceIdentity

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Erstellen eines neuen [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts.
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
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a>Anforderungsheader
|Header|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung für das Objekt ImportedAppleDeviceIdentity eine JSON-Darstellung.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ImportedAppleDeviceIdentity erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|serialNumber|Zeichenfolge|Seriennummer des Geräts|
|requestedEnrollmentProfileId|Zeichenfolge|Registrierung Profil Id Admin beabsichtigt, auf dem Gerät während der nächsten Registrierung anwenden|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|Das Zeit Registrierung Profil zugewiesen wurde das Gerät|
|isSupervised|Boolescher Wert|Gibt an, ob das Gerät Apple überwacht wird. Weitere Informationen finden Sie unter:https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Apple Gerät Discovery-Quelle. Mögliche Werte sind: `unknown`, `adminImport` und `deviceEnrollmentProgram`.|
|createdDateTime|DateTimeOffset|Erstellte Datum-Uhrzeit des Geräts|
|lastContactedDateTime|DateTimeOffset|Letzte kontaktiert Datum-Uhrzeit des Geräts|
|description|Zeichenfolge|Die Beschreibung des Geräts|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Der Zustand des Geräts in Intune. Mögliche Werte sind: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted` und `blocked`.|
|Plattform|[Plattform](../resources/intune-enrollment-platform.md)|Die Plattform des Geräts. Mögliche Werte sind: `unknown`, `ios`, `android`, `windows`, `windowsMobile` und `macOS`.|



## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
Content-type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 605

{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
  "serialNumber": "Serial Number value",
  "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
  "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
  "isSupervised": true,
  "discoverySource": "adminImport",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```





