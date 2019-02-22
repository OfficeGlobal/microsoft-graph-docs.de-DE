---
title: GroupPolicyPresentationTextBox erstellen
description: Erstellen eines neuen groupPolicyPresentationTextBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27cac89799716f0cc08ee6d76ebddae452df3cea
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153494"
---
# <a name="create-grouppolicypresentationtextbox"></a>GroupPolicyPresentationTextBox erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) -Objekts.

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
Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationTextBox-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationTextBox erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|label|String|Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität. Der Standardwert ist Empty. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Entität. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Zeichenfolge|Lokalisierte Standardzeichenfolge, die im Textfeld angezeigt wird. Der Standardwert ist Empty.|
|erforderlich|Boolescher Wert|Anforderung zur Eingabe eines Werts in das Textfeld. Der Standardwert ist "false".|
|maxLength|Int64|Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen angibt. Der Standardwert ist 1023.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```




