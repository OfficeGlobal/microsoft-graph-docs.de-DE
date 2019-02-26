---
title: Aktualisieren von „termsAndConditions“
description: Aktualisieren der Eigenschaften eines termsAndConditions-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b53feaab217d277ac9d314b97e929a0af994f14
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255157"
---
# <a name="update-termsandconditions"></a>Aktualisieren von „termsAndConditions“

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekts.

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
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekts an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|displayName|Zeichenfolge|Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt) |
|description|String|Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)|
|title|String|Titel der Geschäftsbedingungen (vom Administrator festgelegt). Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|bodyText|Zeichenfolge|Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst. Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|acceptanceStatement|Zeichenfolge|Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt. Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.|
|Version|Int32|Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt. Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.|



## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```



