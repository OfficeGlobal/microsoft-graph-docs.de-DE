---
title: Liste Benutzer Geräte
description: Rufen Sie eine Liste der Geräte für Benutzer, die Project-ROM-Funktionen zu unterstützen. Dazu gehören die Möglichkeit zum Starten einer Anwendung oder Nachricht oder Senden von Daten an eine Anwendung. Führen Sie nach der in mich einen Anruf GET / Geräten, übergeben Sie die ID des Geräts, einen Befehl auf Ihrem Gerät zu senden.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 891f66691149106d4ff5a2951170524203eb2ea7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509525"
---
# <a name="list-user-devices"></a>Liste Benutzer Geräte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rufen Sie eine Liste der Geräte für Benutzer, die Project-ROM-Funktionen zu unterstützen. Dazu gehören die Möglichkeit zum Starten einer Anwendung oder Nachricht oder Senden von Daten an eine Anwendung. Führen Sie nach der in mich einen Anruf GET / Geräten, übergeben Sie die ID des Geräts auf Ihrem Gerät [Senden eines Befehls an](send-device-command.md) .

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Nicht unterstützt    |
|Delegiert (persönliches Microsoft-Konto) | Device.Read    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a>Anforderungsheader

| Kopfzeile |Wert
|:----|:------|
|Authorization| Bearer {token}. Erforderlich. |
|Annehmen | application/json |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn erfolgreich, gibt diese Methode einen 200 Antwortcode und die Benutzereigenschaften Gerät im Antworttext.

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```

<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
  "value": [
    {
      "name": "name",
      "id": "id",
      "status": "status",
      "platform": "platform",
      "kind": "formFactor",
      "model": "model",
      "manufacturer": "manufacturer",
    }
  ]
}
```

## <a name="example"></a>Beispiel
In diesem Beispiel wird die Liste der Geräte für einen Benutzer zurückgegeben. Auf einem Gerät mit command `me/devices/{id}/command`, müssen Sie die ID des Geräts zu erhalten, die zurückgegeben wird.

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 140

{
  "value": [
    {
      "Name": "JimSurface",
      "id": "6841b3db-2b55-467b-ad84-79a41a4ef665",
      "Manufacturer": "Microsoft Corporation",
      "Model": "Surface Book",
      "Kind": "Tablet",
      "Status": "Unknown",
      "Platform": "Windows"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-devices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
