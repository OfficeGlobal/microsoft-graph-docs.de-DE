---
title: Aktualisieren von „deviceAppManagement“
description: Aktualisiert die Eigenschaften von Objekten des Typs deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f97316e06cec39cd0aeb1b22d6142925d81b77ae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259367"
---
# <a name="update-deviceappmanagement"></a>Aktualisieren von „deviceAppManagement“

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisiert die Eigenschaften von Objekten des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).

## <a name="prerequisites"></a>Voraussetzungen
Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).  Beachten Sie, dass die entsprechende Berechtigung je nach Workflow variiert.

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementApps.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|**Onboarding**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|Gibt an, ob das Konto Anwendungen mit dem Microsoft Store für Unternehmen synchronisieren darf.|
|microsoftStoreForBusinessLanguage|String|Die Gebietsschemainformationen, die zur Synchronisierung von Anwendungen mit dem Microsoft Store für Unternehmen verwendet werden. Angegeben werden Kulturen, die für ein Land bzw. eine Region spezifisch sind. Die Namen dieser Kulturen folgen dem Standard RFC 4646 (Windows Vista und höher). Das Format lautet <languagecode2>-<country/regioncode2>. Dabei ist <languagecode2> ein klein geschriebener Code aus zwei Buchstaben nach ISO 639-1 und <country/regioncode2> ein groß geschriebener Code aus zwei Buchstaben nach ISO 3166. Beispiel für eine spezifische Kultur: „en-US“ für „Englisch (Vereinigte Staaten)“.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|Zeitpunkt der letzten Anwendungssynchronisierung mit dem Microsoft Store für Unternehmen|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|Zeitpunkt, zu dem das Konto die Apps letztmals erfolgreich mit dem Microsoft Store für Unternehmen synchronisiert hat|

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) im Antworttext zurück.

## <a name="example-request"></a>Beispielanforderung

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a>Beispielantwort

Das hier gezeigte Antwortobjekt kann zur Kürze abgeschnitten werden. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



