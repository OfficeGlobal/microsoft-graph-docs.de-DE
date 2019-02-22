---
title: resourceOperation erstellen
description: Erstellt neue Objekte des Typs resourceOperation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ecbe52ac2c988967a121904e63d1bd6e00929a5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154152"
---
# <a name="create-resourceoperation"></a>resourceOperation erstellen

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erstellt neue Objekte des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementRBAC.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des resourceOperation-Objekts an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der resourceOperation erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Ressourcenoperation. Er ist schreibgeschützt und wird automatisch generiert.|
|resource|Zeichenfolge|Ressourcenkategorie, zu der dieser Vorgang gehört.|
|resourceName|Zeichenfolge|Name der Ressource, auf die die Operation angewendet wird|
|actionName|Zeichenfolge|Typ von Aktion, den die Operation ausführen wird. Der Wert für „actionName“ sollte prägnant sein und aus möglichst wenigen Wörtern bestehen.|
|description|Zeichenfolge|Beschreibung der Ressourcenoperation. Diese Beschreibung wird angezeigt, wenn der Benutzer im Azure-Portal den Mauszeiger auf der Operation platziert.|
|enabledForScopeValidation|Boolescher Wert|Bestimmt, ob die Berechtigung für Bereiche validiert wird, die pro Rollenzuweisung definiert sind.|



## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [resourceOperation](../resources/intune-rbac-resourceoperation.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 249

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```




