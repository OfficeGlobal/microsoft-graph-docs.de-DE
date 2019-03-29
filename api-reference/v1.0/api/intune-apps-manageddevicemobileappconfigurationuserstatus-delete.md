---
title: managedDeviceMobileAppConfigurationUserStatus löschen
description: Löscht ein managedDeviceMobileAppConfigurationUserStatus-Objekt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 524c82ad1a0b50dd16b98f27d55d3fe66c551ca3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985445"
---
# <a name="delete-manageddevicemobileappconfigurationuserstatus"></a>managedDeviceMobileAppConfigurationUserStatus löschen

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Löscht ein [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)-Objekt.

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
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 204 No Content
```



