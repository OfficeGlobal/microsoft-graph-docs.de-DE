---
title: Erstellen von „termsAndConditions“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11015a387d4c22a0293a31641da67ccb650ef1cf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171547"
---
# <a name="create-termsandconditions"></a>Erstellen von „termsAndConditions“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Methode erstellt ein neues Objekt des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).

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
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditions“ an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditions“ erstellen.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts.|
|modifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|displayName|Zeichenfolge|Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt) |
|description|String|Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)|
|title|String|Titel der Geschäftsbedingungen (vom Administrator festgelegt). Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|bodyText|Zeichenfolge|Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst. Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|acceptanceStatement|Zeichenfolge|Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt. Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|Version|Int32|Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt. Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 505

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```




