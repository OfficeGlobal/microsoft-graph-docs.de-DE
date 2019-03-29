---
title: MobileAppTroubleshootingEvent erstellen
description: Beschreibt die CREATE mobileAppTroubleshootingEvent-Methode der Microsoft Graph-API für InTune, die mehrere Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 89a191f94d68636226b6a8d41be0d9ba962da761
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979263"
---
# <a name="create-mobileapptroubleshootingevent"></a>MobileAppTroubleshootingEvent erstellen

> **Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)||
|&nbsp; &nbsp; **Geräteverwaltung**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **Problembehandlung**|DeviceManagementManagedDevices.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das mobileAppTroubleshootingEvent-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der mobileAppTroubleshootingEvent erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|GUID des Objekts|
|**Problembehandlung**|
|Zusatzinformationen|[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung|Eine Reihe von String-Schlüssel-und String-Wert-Paaren, die zusätzliche Informationen zum Problem Behandlungs Ereignis bieten.|
|applicationId|String|InTune-Anwendungsbezeichner.|
|correlationId|String|ID, die zum Nachverfolgen des Fehlers im Dienst verwendet wird. |
|eventDateTime|DateTimeOffset|Uhrzeit, zu der das Ereignis aufgetreten ist. |
|eventName|String|Ereignis Name, der dem Problem Behandlungs Ereignis entspricht. Optional.|
|Geschichte|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) -Sammlung|InTune-Problem Behandlungs Historie für mobile Anwendungen|
|managedDeviceIdentifier|Zeichenfolge|Von Intune erstellter oder erfasster Gerätebezeichner|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Objekt mit detaillierten Informationen über den Fehler und dessen Korrektur. |
|userId|String|Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.|

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




