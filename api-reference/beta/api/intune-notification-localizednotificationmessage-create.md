---
title: localizedNotificationMessage erstellen
description: Erstellen eines neuen localizedNotificationMessage-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bf0187177a80428924af6276eaf9df6f6456e2d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950795"
---
# <a name="create-localizednotificationmessage"></a>localizedNotificationMessage erstellen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Erstellen eines neuen [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)-Objekts.
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
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a>Anforderungsheader
|Header|Wert|
|:---|:---|
|Authorization|Bearer&lt;token&gt; erforderlich|
|Annehmen|application/json|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON Darstellung für das localizedNotificationMessage-Objekt an.

In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der localizedNotificationMessage erforderlich sind.

|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|Gebietsschema|Zeichenfolge|Das Gebietsschema für das diese Nachricht bestimmt ist.|
|Betreff|Zeichenfolge|Die Vorlage für den Betreff der Nachricht.|
|messageTemplate|Zeichenfolge|Die Vorlage für den Inhalt der Nachricht.|
|isDefault|Boolescher Wert|Die Kennzeichnung gibt an, ob dies das Standard-Gebietsschema für die Fallbacksprache ist. Dieser Kennzeichnung kann nur festgelegt werden. Um die Festlegung aufzuheben, setzen Sie diese Eigenschaft bei einer anderen lokalisierten Benachrichtigung auf „true“.|



## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) im Antworttext zurück.

## <a name="example"></a>Beispiel
### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "7a777708-7708-7a77-0877-777a0877777a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```





