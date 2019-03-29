---
title: MacOsVppAppAssignedLicense aktualisieren
description: Aktualisieren der Eigenschaften eines macOsVppAppAssignedLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0481a40d07038c98778c1968347a2c6886fe3a86
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979655"
---
# <a name="update-macosvppappassignedlicense"></a>MacOsVppAppAssignedLicense aktualisieren

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Aktualisieren der Eigenschaften eines [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.

## <a name="prerequisites"></a>Voraussetzungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp|Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)|
|:---|:---|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|DeviceManagementApps.ReadWrite.All|
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung für das [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|userEmailAddress|String|Die Benutzer-e-Mail-Adresse.|
|userId|String|Die Benutzer-ID.|
|userName|String|Der Benutzername.|
|userPrincipalName|String|Der Benutzerprinzipalname.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




