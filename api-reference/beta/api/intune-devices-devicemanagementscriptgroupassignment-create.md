---
title: DeviceManagementScriptGroupAssignment erstellen
description: Erstellen eines neuen deviceManagementScriptGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39053b6b56e130f66f8911ca60e4ed95effce385
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163412"
---
# <a name="create-devicemanagementscriptgroupassignment"></a>DeviceManagementScriptGroupAssignment erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellen eines neuen [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceManagementScriptGroupAssignment-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceManagementScriptGroupAssignment erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Zuordnungs Entität "Device Management Script Group".|
|targetGroupId|Zeichenfolge|Die ID der Azure Active Directory-Gruppe, auf die wir das Skript ausrichten.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```




