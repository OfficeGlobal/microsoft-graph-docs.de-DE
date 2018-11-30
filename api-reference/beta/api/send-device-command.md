---
title: Gerätebefehl senden
description: 'Diese API ermöglicht die Project-ROM-Funktionen, die ein Gerät mit einem Microsoft-Konto verknüpften Befehl. Nach dem Gespräch GET auf macht `me/devices`, übergeben Sie die ID des Geräts einen Befehl auf Ihrem Gerät ausgeben. Zwei Arten von Befehle werden unterstützt: LaunchURI und AppServices. Wenn Sie LaunchURI verwenden, geben Sie den Parameter *Typ* und *Nutzlast* . Geben Sie für einen Anruf AppService die '
ms.openlocfilehash: bf330ab1234ef6ce22c6a43711621827b628a7ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062085"
---
# <a name="send-device-command"></a>Gerätebefehl senden

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Diese API ermöglicht die Project-ROM-Funktionen, die ein Gerät mit einem Microsoft-Konto verknüpften Befehl. Nach dem Gespräch GET auf macht `me/devices`, übergeben Sie die ID des Geräts einen Befehl auf Ihrem Gerät ausgeben. Zwei Arten von Befehle werden unterstützt: LaunchURI und AppServices. Wenn Sie LaunchURI verwenden, geben Sie den Parameter *Typ* und *Nutzlast* . Geben Sie für einen Anruf AppService *Typ*, *Nutzlast*, *PackageFamilyName*und *AppServiceName* -Parameter.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Nicht unterstützt    |
|Delegiert (persönliches Microsoft-Konto) | Device.Command    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a>Anforderungsheader


| Kopfzeile |Wert
|:----|:------|
|Authorization| Bearer {token}. Erforderlich. |
|Accept | application/json |

## <a name="request-body"></a>Anforderungstext

Geben Sie eine JSON-Darstellung der Befehlseigenschaften im Textkörper Anforderung.

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a>Antwort

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
## <a name="command-properties"></a>Command-Eigenschaften 

|**Name**|**Typ**|**Beschreibung**|
|:----|:------|:------|
|payload | Microsoft.Graph.JSON| Nutzlast zum Senden an ein app-Dienst oder um einen URI auf einem Gerät zu starten. |
|responsePayload | Microsoft.Graph.JSON| Nutzlast von Zielgerät zurückgegeben. |
|postBackURI | String | Postback URI, um nachfolgende Benachrichtigungen von Updates zu senden. |
|packageFamilyName | String | Windows Paket Familienname der Anwendung. |
|appServiceName | String | Name des app-Dienst von der Zielanwendung definiert. Erforderlich, wenn einen app-Dienst zu starten. |
|Typ| String | LaunchURI oder AppService. |
|id| String | Die ID eines Befehls, der an das Gerät gesendet wurde. |
|actionStatus | String | Der [Status](get-device-command-status.md) eines Befehls. |
|error| String| Alle Fehler im Zusammenhang mit der Anforderung aus der Zielanwendung. |

## <a name="launch-uri-example"></a>Starten Sie die URI-Beispiel

Es folgt ein Beispiel für eine Anforderung LaunchURI; Es wird ein URI oder eine Anwendung auf dem Zielcomputer gestartet. Um einen URI oder eine app starten, Ausstellen einer POST-Anforderung mit der ID des Geräts (wie folgt einen GET-Aufruf auf gewonnen `me/devices`). Legen Sie die *Type* -Parameter auf *LaunchURI* und geben Sie einen URI-Wert wie https://bing.com.

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```

#### <a name="response"></a>Antwort 

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


## <a name="app-service-example"></a>Dienst-App-Beispiel

Es folgt ein Beispiel einer Abfrage einen app-Dienst auf einem Gerät. Verwenden Sie einen app-Dienst müssen Sie einen POST-Anruf mit der Id des Geräts (wie folgt einen GET-Aufruf auf gewonnen `me/devices`). Um das folgende Beispiel verwenden zu können, müssen Sie die [ROM app](https://aka.ms/romanapp) auf dem Zielgerät installieren.

In den Anruf müssen verschiedene zusätzliche Eigenschaften festgelegt werden. *Typ* muss auf *AppService*festgelegt werden, *AppServiceName* muss festgelegt werden, auf den Namen des app-Diensts in der Anwendung definiert, *PackageFamilyName* muss auf den in der app-Manifest und *Nutzlast* definierten Familie Paketnamen festgelegt werden enthält die Schlüssel und Werte für den Dienst, den Sie innerhalb der Zielanwendung anrufen.

#### <a name="request"></a>Anforderung

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
