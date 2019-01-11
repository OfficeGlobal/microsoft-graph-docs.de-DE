---
title: Gerätebefehl senden
description: 'Diese API ermöglicht die Project-ROM-Funktionen, die ein Gerät mit einem Microsoft-Konto verknüpften Befehl. Nach dem Gespräch GET auf macht `me/devices`, übergeben Sie die ID des Geräts einen Befehl auf Ihrem Gerät ausgeben. Zwei Arten von Befehle werden unterstützt: LaunchURI und AppServices. Wenn Sie LaunchURI verwenden, geben Sie den Parameter *Typ* und *Nutzlast* . Geben Sie für einen Anruf AppService die '
localization_priority: Normal
ms.openlocfilehash: 54349e2f43a776523614b0cd2abbc209e89305fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891987"
---
# <a name="send-device-command"></a><span data-ttu-id="cd430-107">Gerätebefehl senden</span><span class="sxs-lookup"><span data-stu-id="cd430-107">Send device command</span></span>

> <span data-ttu-id="cd430-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cd430-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd430-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cd430-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd430-110">Diese API ermöglicht die Project-ROM-Funktionen, die ein Gerät mit einem Microsoft-Konto verknüpften Befehl.</span><span class="sxs-lookup"><span data-stu-id="cd430-110">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="cd430-111">Nach dem Gespräch GET auf macht `me/devices`, übergeben Sie die ID des Geräts einen Befehl auf Ihrem Gerät ausgeben.</span><span class="sxs-lookup"><span data-stu-id="cd430-111">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="cd430-112">Zwei Arten von Befehle werden unterstützt: LaunchURI und AppServices.</span><span class="sxs-lookup"><span data-stu-id="cd430-112">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="cd430-113">Wenn Sie LaunchURI verwenden, geben Sie den Parameter *Typ* und *Nutzlast* .</span><span class="sxs-lookup"><span data-stu-id="cd430-113">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="cd430-114">Geben Sie für einen Anruf AppService *Typ*, *Nutzlast*, *PackageFamilyName*und *AppServiceName* -Parameter.</span><span class="sxs-lookup"><span data-stu-id="cd430-114">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd430-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd430-115">Permissions</span></span>

<span data-ttu-id="cd430-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd430-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cd430-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd430-118">Permission type</span></span>      | <span data-ttu-id="cd430-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd430-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd430-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd430-120">Delegated (work or school account)</span></span> | <span data-ttu-id="cd430-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd430-121">Not supported.</span></span>    |
|<span data-ttu-id="cd430-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd430-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd430-123">Device.Command</span><span class="sxs-lookup"><span data-stu-id="cd430-123">Device.Command</span></span>    |
|<span data-ttu-id="cd430-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd430-124">Application</span></span> | <span data-ttu-id="cd430-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd430-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd430-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd430-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="cd430-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd430-127">Request headers</span></span>


| <span data-ttu-id="cd430-128">Header</span><span class="sxs-lookup"><span data-stu-id="cd430-128">Header</span></span> |<span data-ttu-id="cd430-129">Wert</span><span class="sxs-lookup"><span data-stu-id="cd430-129">Value</span></span>
|:----|:------|
|<span data-ttu-id="cd430-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd430-130">Authorization</span></span>| <span data-ttu-id="cd430-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd430-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="cd430-133">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cd430-133">Accept</span></span> | <span data-ttu-id="cd430-134">application/json</span><span class="sxs-lookup"><span data-stu-id="cd430-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd430-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd430-135">Request body</span></span>

<span data-ttu-id="cd430-136">Geben Sie eine JSON-Darstellung der Befehlseigenschaften im Textkörper Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd430-136">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="cd430-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd430-137">Response</span></span>

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
## <a name="command-properties"></a><span data-ttu-id="cd430-138">Command-Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cd430-138">Command properties</span></span> 

|<span data-ttu-id="cd430-139">**Name**</span><span class="sxs-lookup"><span data-stu-id="cd430-139">**Name**</span></span>|<span data-ttu-id="cd430-140">**Typ**</span><span class="sxs-lookup"><span data-stu-id="cd430-140">**Type**</span></span>|<span data-ttu-id="cd430-141">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="cd430-141">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="cd430-142">payload</span><span class="sxs-lookup"><span data-stu-id="cd430-142">payload</span></span> | <span data-ttu-id="cd430-143">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="cd430-143">microsoft.graph.json</span></span>| <span data-ttu-id="cd430-144">Nutzlast zum Senden an ein app-Dienst oder um einen URI auf einem Gerät zu starten.</span><span class="sxs-lookup"><span data-stu-id="cd430-144">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="cd430-145">responsePayload</span><span class="sxs-lookup"><span data-stu-id="cd430-145">responsePayload</span></span> | <span data-ttu-id="cd430-146">Microsoft.Graph.JSON</span><span class="sxs-lookup"><span data-stu-id="cd430-146">microsoft.graph.json</span></span>| <span data-ttu-id="cd430-147">Nutzlast von Zielgerät zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd430-147">Payload returned from target device.</span></span> |
|<span data-ttu-id="cd430-148">postBackURI</span><span class="sxs-lookup"><span data-stu-id="cd430-148">postBackURI</span></span> | <span data-ttu-id="cd430-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd430-149">String</span></span> | <span data-ttu-id="cd430-150">Postback URI, um nachfolgende Benachrichtigungen von Updates zu senden.</span><span class="sxs-lookup"><span data-stu-id="cd430-150">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="cd430-151">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="cd430-151">packageFamilyName</span></span> | <span data-ttu-id="cd430-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd430-152">String</span></span> | <span data-ttu-id="cd430-153">Windows Paket Familienname der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="cd430-153">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="cd430-154">appServiceName</span><span class="sxs-lookup"><span data-stu-id="cd430-154">appServiceName</span></span> | <span data-ttu-id="cd430-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd430-155">String</span></span> | <span data-ttu-id="cd430-156">Name des app-Dienst von der Zielanwendung definiert.</span><span class="sxs-lookup"><span data-stu-id="cd430-156">Name of app service defined by the target application.</span></span> <span data-ttu-id="cd430-157">Erforderlich, wenn einen app-Dienst zu starten.</span><span class="sxs-lookup"><span data-stu-id="cd430-157">Required if launching an app service.</span></span> |
|<span data-ttu-id="cd430-158">type</span><span class="sxs-lookup"><span data-stu-id="cd430-158">type</span></span>| <span data-ttu-id="cd430-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd430-159">String</span></span> | <span data-ttu-id="cd430-160">LaunchURI oder AppService.</span><span class="sxs-lookup"><span data-stu-id="cd430-160">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="cd430-161">id</span><span class="sxs-lookup"><span data-stu-id="cd430-161">id</span></span>| <span data-ttu-id="cd430-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd430-162">String</span></span> | <span data-ttu-id="cd430-163">Die ID eines Befehls, der an das Gerät gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="cd430-163">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="cd430-164">actionStatus</span><span class="sxs-lookup"><span data-stu-id="cd430-164">actionStatus</span></span> | <span data-ttu-id="cd430-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd430-165">String</span></span> | <span data-ttu-id="cd430-166">Der [Status](get-device-command-status.md) eines Befehls.</span><span class="sxs-lookup"><span data-stu-id="cd430-166">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="cd430-167">error</span><span class="sxs-lookup"><span data-stu-id="cd430-167">error</span></span>| <span data-ttu-id="cd430-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cd430-168">String</span></span>| <span data-ttu-id="cd430-169">Alle Fehler im Zusammenhang mit der Anforderung aus der Zielanwendung.</span><span class="sxs-lookup"><span data-stu-id="cd430-169">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="cd430-170">Starten Sie die URI-Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd430-170">Launch URI example</span></span>

<span data-ttu-id="cd430-171">Es folgt ein Beispiel für eine Anforderung LaunchURI; Es wird ein URI oder eine Anwendung auf dem Zielcomputer gestartet.</span><span class="sxs-lookup"><span data-stu-id="cd430-171">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="cd430-172">Um einen URI oder eine app starten, Ausstellen einer POST-Anforderung mit der ID des Geräts (wie folgt einen GET-Aufruf auf gewonnen `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="cd430-172">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="cd430-173">Legen Sie die *Type* -Parameter auf *LaunchURI* und geben Sie einen URI-Wert wie https://bing.com.</span><span class="sxs-lookup"><span data-stu-id="cd430-173">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="cd430-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd430-174">Request</span></span>

<span data-ttu-id="cd430-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd430-175">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="cd430-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd430-176">Response</span></span> 

<span data-ttu-id="cd430-177">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cd430-177">The following is an example of the response.</span></span>

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


## <a name="app-service-example"></a><span data-ttu-id="cd430-178">Dienst-App-Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd430-178">App service example</span></span>

<span data-ttu-id="cd430-179">Es folgt ein Beispiel einer Abfrage einen app-Dienst auf einem Gerät.</span><span class="sxs-lookup"><span data-stu-id="cd430-179">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="cd430-180">Verwenden Sie einen app-Dienst müssen Sie einen POST-Anruf mit der Id des Geräts (wie folgt einen GET-Aufruf auf gewonnen `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="cd430-180">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="cd430-181">Um das folgende Beispiel verwenden zu können, müssen Sie die [ROM app](https://aka.ms/romanapp) auf dem Zielgerät installieren.</span><span class="sxs-lookup"><span data-stu-id="cd430-181">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="cd430-182">In den Anruf müssen verschiedene zusätzliche Eigenschaften festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="cd430-182">Several additional properties must be set in the call.</span></span> <span data-ttu-id="cd430-183">*Typ* muss auf *AppService*festgelegt werden, *AppServiceName* muss festgelegt werden, auf den Namen des app-Diensts in der Anwendung definiert, *PackageFamilyName* muss auf den in der app-Manifest und *Nutzlast* definierten Familie Paketnamen festgelegt werden enthält die Schlüssel und Werte für den Dienst, den Sie innerhalb der Zielanwendung anrufen.</span><span class="sxs-lookup"><span data-stu-id="cd430-183">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="cd430-184">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd430-184">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cd430-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd430-185">Response</span></span>

<span data-ttu-id="cd430-186">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cd430-186">The following is an example of the response.</span></span>

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
