---
title: SideLoadingKey aktualisieren
description: Aktualisieren der Eigenschaften eines sideLoadingKey-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 408cc20d76eaa06260ddd1a0de485cc3a2d57abc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977534"
---
# <a name="update-sideloadingkey"></a>SideLoadingKey aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekts.

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
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutige ID des seitlichen Lade Schlüssels.|
|value|Zeichenfolge|Seiten Ladeschlüssel Wert, es ist 5x5-Wert, getrennt durch hiphens.|
|displayName|String|Der Name des Seiten Lade Schlüssels wird den ITPro-Administratoren angezeigt.|
|description|Zeichenfolge|Seiten Ladeschlüssel Beschreibung, die den ITPro-Administratoren angezeigt wird..|
|totalActivation|Int32|Die Gesamt Aktivierung des Seiten Lade Schlüssels wird den ITPro-Administratoren angezeigt.|
|lastUpdatedDateTime|String|Das Datum der letzten Aktualisierung, die den ITPro-Administratoren angezeigt werden.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```




