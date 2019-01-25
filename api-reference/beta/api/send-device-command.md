---
title: Gerätebefehl senden
description: 'Diese API ermöglicht die Project-ROM-Funktionen, die ein Gerät mit einem Microsoft-Konto verknüpften Befehl. Nach dem Gespräch GET auf macht `me/devices`, übergeben Sie die ID des Geräts einen Befehl auf Ihrem Gerät ausgeben. Zwei Arten von Befehle werden unterstützt: LaunchURI und AppServices. Wenn Sie LaunchURI verwenden, geben Sie den Parameter *Typ* und *Nutzlast* . Geben Sie für einen Anruf AppService die '
localization_priority: Normal
ms.openlocfilehash: d0c25200933a4a87a66349e457c500c496272b08
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526242"
---
# <a name="send-device-command"></a><span data-ttu-id="2a248-107">Gerätebefehl senden</span><span class="sxs-lookup"><span data-stu-id="2a248-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a248-108">Diese API ermöglicht die Project-ROM-Funktionen, die ein Gerät mit einem Microsoft-Konto verknüpften Befehl.</span><span class="sxs-lookup"><span data-stu-id="2a248-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="2a248-109">Nach dem Gespräch GET auf macht `me/devices`, übergeben Sie die ID des Geräts einen Befehl auf Ihrem Gerät ausgeben.</span><span class="sxs-lookup"><span data-stu-id="2a248-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="2a248-110">Zwei Arten von Befehle werden unterstützt: LaunchURI und AppServices.</span><span class="sxs-lookup"><span data-stu-id="2a248-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="2a248-111">Wenn Sie LaunchURI verwenden, geben Sie den Parameter *Typ* und *Nutzlast* .</span><span class="sxs-lookup"><span data-stu-id="2a248-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="2a248-112">Geben Sie für einen Anruf AppService *Typ*, *Nutzlast*, *PackageFamilyName*und *AppServiceName* -Parameter.</span><span class="sxs-lookup"><span data-stu-id="2a248-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a248-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2a248-113">Permissions</span></span>

<span data-ttu-id="2a248-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a248-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2a248-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a248-116">Permission type</span></span>      | <span data-ttu-id="2a248-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a248-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a248-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a248-118">Delegated (work or school account)</span></span> | <span data-ttu-id="2a248-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a248-119">Not supported.</span></span>    |
|<span data-ttu-id="2a248-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a248-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a248-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="2a248-121">Device.Command</span></span>    |
|<span data-ttu-id="2a248-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a248-122">Application</span></span> | <span data-ttu-id="2a248-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a248-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a248-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a248-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="2a248-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a248-125">Request headers</span></span>


| <span data-ttu-id="2a248-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2a248-126">Header</span></span> |<span data-ttu-id="2a248-127">Wert</span><span class="sxs-lookup"><span data-stu-id="2a248-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="2a248-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a248-128">Authorization</span></span>| <span data-ttu-id="2a248-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2a248-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="2a248-131">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2a248-131">Accept</span></span> | <span data-ttu-id="2a248-132">application/json</span><span class="sxs-lookup"><span data-stu-id="2a248-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a248-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a248-133">Request body</span></span>

<span data-ttu-id="2a248-134">Geben Sie eine JSON-Darstellung der Befehlseigenschaften im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a248-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="2a248-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a248-135">Response</span></span>

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
## <a name="command-properties"></a><span data-ttu-id="2a248-136">Command Properties</span><span class="sxs-lookup"><span data-stu-id="2a248-136">Command properties</span></span> 

|<span data-ttu-id="2a248-137">**Name**</span><span class="sxs-lookup"><span data-stu-id="2a248-137">**Name**</span></span>|<span data-ttu-id="2a248-138">**Typ**</span><span class="sxs-lookup"><span data-stu-id="2a248-138">**Type**</span></span>|<span data-ttu-id="2a248-139">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="2a248-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="2a248-140">payload</span><span class="sxs-lookup"><span data-stu-id="2a248-140">payload</span></span> | <span data-ttu-id="2a248-141">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="2a248-141">microsoft.graph.json</span></span>| <span data-ttu-id="2a248-142">Nutzlast zum Senden an ein app-Dienst oder um einen URI auf einem Gerät zu starten.</span><span class="sxs-lookup"><span data-stu-id="2a248-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="2a248-143">responsePayload</span><span class="sxs-lookup"><span data-stu-id="2a248-143">responsePayload</span></span> | <span data-ttu-id="2a248-144">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="2a248-144">microsoft.graph.json</span></span>| <span data-ttu-id="2a248-145">Nutzlast von Zielgerät zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a248-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="2a248-146">postBackURI</span><span class="sxs-lookup"><span data-stu-id="2a248-146">postBackURI</span></span> | <span data-ttu-id="2a248-147">String</span><span class="sxs-lookup"><span data-stu-id="2a248-147">String</span></span> | <span data-ttu-id="2a248-148">Postback URI, um nachfolgende Benachrichtigungen von Updates zu senden.</span><span class="sxs-lookup"><span data-stu-id="2a248-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="2a248-149">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="2a248-149">packageFamilyName</span></span> | <span data-ttu-id="2a248-150">String</span><span class="sxs-lookup"><span data-stu-id="2a248-150">String</span></span> | <span data-ttu-id="2a248-151">Windows Paket Familienname der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="2a248-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="2a248-152">appServiceName</span><span class="sxs-lookup"><span data-stu-id="2a248-152">appServiceName</span></span> | <span data-ttu-id="2a248-153">String</span><span class="sxs-lookup"><span data-stu-id="2a248-153">String</span></span> | <span data-ttu-id="2a248-154">Name des app-Dienst von der Zielanwendung definiert.</span><span class="sxs-lookup"><span data-stu-id="2a248-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="2a248-155">Erforderlich, wenn einen app-Dienst zu starten.</span><span class="sxs-lookup"><span data-stu-id="2a248-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="2a248-156">type</span><span class="sxs-lookup"><span data-stu-id="2a248-156">type</span></span>| <span data-ttu-id="2a248-157">String</span><span class="sxs-lookup"><span data-stu-id="2a248-157">String</span></span> | <span data-ttu-id="2a248-158">LaunchURI oder AppService.</span><span class="sxs-lookup"><span data-stu-id="2a248-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="2a248-159">id</span><span class="sxs-lookup"><span data-stu-id="2a248-159">id</span></span>| <span data-ttu-id="2a248-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a248-160">String</span></span> | <span data-ttu-id="2a248-161">Die ID eines Befehls, der an das Gerät gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="2a248-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="2a248-162">actionStatus</span><span class="sxs-lookup"><span data-stu-id="2a248-162">actionStatus</span></span> | <span data-ttu-id="2a248-163">String</span><span class="sxs-lookup"><span data-stu-id="2a248-163">String</span></span> | <span data-ttu-id="2a248-164">Der [Status](get-device-command-status.md) eines Befehls.</span><span class="sxs-lookup"><span data-stu-id="2a248-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="2a248-165">error</span><span class="sxs-lookup"><span data-stu-id="2a248-165">error</span></span>| <span data-ttu-id="2a248-166">String</span><span class="sxs-lookup"><span data-stu-id="2a248-166">String</span></span>| <span data-ttu-id="2a248-167">Alle Fehler im Zusammenhang mit der Anforderung aus der Zielanwendung.</span><span class="sxs-lookup"><span data-stu-id="2a248-167">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="2a248-168">Starten Sie die URI-Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a248-168">Launch URI example</span></span>

<span data-ttu-id="2a248-169">Es folgt ein Beispiel für eine Anforderung LaunchURI; Es wird ein URI oder eine Anwendung auf dem Zielcomputer gestartet.</span><span class="sxs-lookup"><span data-stu-id="2a248-169">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="2a248-170">Um einen URI oder eine app starten, Ausstellen einer POST-Anforderung mit der ID des Geräts (wie folgt einen GET-Aufruf auf gewonnen `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="2a248-170">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="2a248-171">Legen Sie die *Type* -Parameter auf *LaunchURI* und geben Sie einen URI-Wert wie https://bing.com.</span><span class="sxs-lookup"><span data-stu-id="2a248-171">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="2a248-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a248-172">Request</span></span>

<span data-ttu-id="2a248-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a248-173">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="2a248-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a248-174">Response</span></span> 

<span data-ttu-id="2a248-175">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2a248-175">The following is an example of the response.</span></span>

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


## <a name="app-service-example"></a><span data-ttu-id="2a248-176">Dienst-App-Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a248-176">App service example</span></span>

<span data-ttu-id="2a248-177">Es folgt ein Beispiel einer Abfrage einen app-Dienst auf einem Gerät.</span><span class="sxs-lookup"><span data-stu-id="2a248-177">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="2a248-178">Verwenden Sie einen app-Dienst müssen Sie einen POST-Anruf mit der Id des Geräts (wie folgt einen GET-Aufruf auf gewonnen `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="2a248-178">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="2a248-179">Um das folgende Beispiel verwenden zu können, müssen Sie die [ROM app](https://aka.ms/romanapp) auf dem Zielgerät installieren.</span><span class="sxs-lookup"><span data-stu-id="2a248-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="2a248-180">In den Anruf müssen verschiedene zusätzliche Eigenschaften festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="2a248-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="2a248-181">*Typ* muss auf *AppService*festgelegt werden, *AppServiceName* muss festgelegt werden, auf den Namen des app-Diensts in der Anwendung definiert, *PackageFamilyName* muss auf den in der app-Manifest und *Nutzlast* definierten Familie Paketnamen festgelegt werden enthält die Schlüssel und Werte für den Dienst, den Sie innerhalb der Zielanwendung anrufen.</span><span class="sxs-lookup"><span data-stu-id="2a248-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="2a248-182">Anfordern</span><span class="sxs-lookup"><span data-stu-id="2a248-182">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="2a248-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a248-183">Response</span></span>

<span data-ttu-id="2a248-184">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2a248-184">The following is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/send-device-command.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
