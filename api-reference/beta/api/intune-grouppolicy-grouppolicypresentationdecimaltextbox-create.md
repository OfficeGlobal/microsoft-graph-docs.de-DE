---
title: GroupPolicyPresentationDecimalTextBox erstellen
description: Erstellen eines neuen groupPolicyPresentationDecimalTextBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c518eb990927e98a8ea75f8b71d98811f455557
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167165"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a>GroupPolicyPresentationDecimalTextBox erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) -Objekts.

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
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationDecimalTextBox-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationDecimalTextBox erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|label|String|Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität. Der Standardwert ist Empty. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Entität. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Int64|Eine ganze Zahl ohne Vorzeichen, die den Anfangswert für das Dezimal Textfeld angibt. Der Standardwert ist 1.|
|Spin|Boolescher Wert|Wenn true, erstellen Sie ein Drehfeld-Steuerelement; Erstellen Sie andernfalls ein Textfeld für die numerische Eingabe. Der Standardwert ist true.|
|spinStep|Int64|Eine ganze Zahl ohne Vorzeichen, die die Schrittweite der Änderung für das Drehfeld-Steuerelement angibt. Der Standardwert ist 1.|
|erforderlich|Boolescher Wert|Anforderung zur Eingabe eines Werts im Parameterfeld. Der Standardwert ist false.|
|minValue|Int64|Eine ganze Zahl ohne Vorzeichen, die den minimal zulässigen Wert angibt. Der Standardwert ist 0.|
|maxValue|Int64|Eine ganze Zahl ohne Vorzeichen, die den maximal zulässigen Wert angibt. Der Standardwert ist 9999.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```




