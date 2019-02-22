---
title: GroupPolicyDefinitionFile aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyDefinitionFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e204382f9237428b30362f7464264f732e13541a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169412"
---
# <a name="update-grouppolicydefinitionfile"></a>GroupPolicyDefinitionFile aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.

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
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Der lokalisierte Anzeigename der ADMX-Datei.|
|description|Zeichenfolge|Die lokalisierte Beschreibung der Richtlinieneinstellungen in der ADMX-Datei. Der Standardwert ist Empty.|
|languageCodes|String collection|Die unterstützten Sprachcodes für die ADMX-Datei.|
|targetPrefix|Zeichenfolge|Gibt den logischen Namen an, der auf den Namespace innerhalb der ADMX-Datei verweist.|
|targetNamespace|Zeichenfolge|Gibt den URI an, der zum Identifizieren des Namespaces innerhalb der ADMX-Datei verwendet wird.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Gibt den Typ der Gruppenrichtlinie an. Mögliche Werte sind: `admxBacked` und `admxIngested`.|
|id|Zeichenfolge|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Entität.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




