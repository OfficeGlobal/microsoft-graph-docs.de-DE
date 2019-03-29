---
title: ManagementConditionStatement erstellen
description: Erstellen eines neuen managementConditionStatement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e4531f8819be505587a27008f36fb9c06f2d92a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971640"
---
# <a name="create-managementconditionstatement"></a>ManagementConditionStatement erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

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
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das managementConditionStatement-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managementConditionStatement erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für die Verwaltungs Bedingungsanweisung. Vom System generierter Wert, der bei der Erstellung zugewiesen wird.|
|displayName|String|Der vom Administrator definierte Name der Verwaltungs Bedingungsanweisung.|
|description|Zeichenfolge|Die vom Administrator definierte Beschreibung der Verwaltungs Bedingungsanweisung.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Verwaltungs Bedingungsanweisung erstellt wurde. Generierte Dienstseite.|
|modifiedDateTime|DateTimeOffset|Der Zeitpunkt, zu dem die Anweisung für die Verwaltungsbedingung zuletzt geändert wurde. Aktualisierte Dienstseite.|
|Ausdruck|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|Der Ausdruck der Verwaltungs Bedingungsanweisung, mit dem ausgewertet wird, ob eine Anweisung für die Verwaltungsbedingung aktiviert/deaktiviert wurde.|
|eTag|String|ETag der Verwaltungs Bedingungsanweisung. Aktualisierte Dienstseite.|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung|Die entsprechenden Plattformen für diese Verwaltungs Bedingungsanweisung.
Dies wird berechnet anhand der Verwaltungsbedingungen, die mit der Verwaltungs Bedingungsanweisung verbunden sind, und dem Auffinden der Schnittstelle der entsprechenden Plattformen. Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```




