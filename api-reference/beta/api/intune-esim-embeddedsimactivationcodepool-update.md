---
title: EmbeddedSIMActivationCodePool aktualisieren
description: Aktualisieren der Eigenschaften eines embeddedSIMActivationCodePool-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3cf828192443f4640932cdd8ec502c915770dd4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173192"
---
# <a name="update-embeddedsimactivationcodepool"></a>EmbeddedSIMActivationCodePool aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.

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
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für den eingebetteten SIM-Aktivierungscode Pool. Vom System generierter Wert, der bei der Erstellung zugewiesen wird.|
|displayName|Zeichenfolge|Der vom Administrator definierte Name des eingebetteten SIM-Aktivierungscode Pools.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem der eingebettete SIM-Aktivierungscode Pool erstellt wurde. Generierte Dienstseite.|
|modifiedDateTime|DateTimeOffset|Zeitpunkt, zu dem der eingebettete SIM-Aktivierungscode Pool zuletzt geändert wurde. Aktualisierte Dienstseite.|
|activationCodes|[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) -Sammlung|Die Aktivierungscodes, die zu diesem Pool gehören. Diese Navigationseigenschaft wird verwendet, um Aktivierungscodes in InTune bereitzustellen, kann jedoch nicht zum Lesen von Aktivierungscodes aus InTune verwendet werden.|
|activationCodeCount|Int32|Die Gesamtanzahl der Aktivierungscodes, die zu diesem Pool gehören.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```




