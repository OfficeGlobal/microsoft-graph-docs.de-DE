---
title: Befehl Gerätestatus anfordern.
description: Rufen Sie den Status eines Befehls auf einem Gerät. Die vollständige Liste der Statuscodes finden Sie unter Liste der ActionStatus.
localization_priority: Normal
ms.openlocfilehash: ae5fe1f2b6b48c0a739911bd20370562e8540f18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510113"
---
# <a name="get-device-command-status"></a><span data-ttu-id="dde76-104">Befehl Gerätestatus anfordern.</span><span class="sxs-lookup"><span data-stu-id="dde76-104">Get device command status</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dde76-105">Rufen Sie den Status eines Befehls auf einem Gerät.</span><span class="sxs-lookup"><span data-stu-id="dde76-105">Get the status of a command on a device.</span></span> <span data-ttu-id="dde76-106">Die vollständige Liste der Statuscodes finden Sie unter [Liste der ActionStatus](#list-of-actionstatus).</span><span class="sxs-lookup"><span data-stu-id="dde76-106">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="dde76-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dde76-107">Permissions</span></span>

<span data-ttu-id="dde76-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dde76-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dde76-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dde76-110">Permission type</span></span>      | <span data-ttu-id="dde76-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dde76-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dde76-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dde76-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dde76-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dde76-113">Not supported.</span></span>    |
|<span data-ttu-id="dde76-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dde76-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dde76-115">Device.Command</span><span class="sxs-lookup"><span data-stu-id="dde76-115">Device.Command</span></span>    |
|<span data-ttu-id="dde76-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dde76-116">Application</span></span> | <span data-ttu-id="dde76-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dde76-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dde76-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dde76-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dde76-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dde76-119">Request headers</span></span>

| <span data-ttu-id="dde76-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dde76-120">Header</span></span> |<span data-ttu-id="dde76-121">Wert</span><span class="sxs-lookup"><span data-stu-id="dde76-121">Value</span></span>
|:----|:------|
|<span data-ttu-id="dde76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dde76-122">Authorization</span></span>| <span data-ttu-id="dde76-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dde76-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="dde76-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dde76-125">Accept</span></span> | <span data-ttu-id="dde76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dde76-126">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="dde76-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="dde76-127">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
  {
    "id": "0",
    "status": "requesting",
    "type": "null",
    "appServiceName": "null",
    "packageFamilyName": "null",
    "error": "null",
    "responsepayload": "null",
    "payload": "null",
    "permissionTicket": "null",
    "postBackUri": "null"
  }
```

## <a name="list-of-actionstatus"></a><span data-ttu-id="dde76-128">Liste der actionStatus</span><span class="sxs-lookup"><span data-stu-id="dde76-128">List of actionStatus</span></span>

- <span data-ttu-id="dde76-129">Anfordern von / / Befehl erstellt wurde und wartet auf Verarbeitung</span><span class="sxs-lookup"><span data-stu-id="dde76-129">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="dde76-130">SentToTarget, / / Befehl an das Gerät gesendet wurde</span><span class="sxs-lookup"><span data-stu-id="dde76-130">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="dde76-131">ausführen, / / Zielgerät Bestätigung des Befehls bestätigt und ausgeführt wird</span><span class="sxs-lookup"><span data-stu-id="dde76-131">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="dde76-132">abgeschlossen, / / Command Ausführung beendet</span><span class="sxs-lookup"><span data-stu-id="dde76-132">completed, // Command execution completed</span></span>
- <span data-ttu-id="dde76-133">FailedToSend, / / -Dienst konnte nicht auf das Zielgerät Befehl senden</span><span class="sxs-lookup"><span data-stu-id="dde76-133">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="dde76-134">ExecutionFailed, / / Command fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="dde76-134">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="dde76-135">CommandDropped, / / Befehl vom Client gelöscht, wenn ConnectedStandby Gerät ist</span><span class="sxs-lookup"><span data-stu-id="dde76-135">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="dde76-136">Abbrechen, / / Abbrechen des Befehls</span><span class="sxs-lookup"><span data-stu-id="dde76-136">cancel, // Cancel the command</span></span>
- <span data-ttu-id="dde76-137">Abbrechen, / / den Befehl wird abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="dde76-137">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="dde76-138">abgebrochen, / / Befehl wurde abgebrochen</span><span class="sxs-lookup"><span data-stu-id="dde76-138">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="dde76-139">Wiederholen, / / Dienst wird zum Senden von Befehl an Ziel wiederholen</span><span class="sxs-lookup"><span data-stu-id="dde76-139">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="dde76-140">abgelaufen, / / Befehl Verarbeitung Ablaufzeit überschritten</span><span class="sxs-lookup"><span data-stu-id="dde76-140">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="dde76-141">Fehler: / / Interner Fehler beim Ausführen des Befehls</span><span class="sxs-lookup"><span data-stu-id="dde76-141">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="dde76-142">Benutzerdefinierte / / benutzerdefinierte Status</span><span class="sxs-lookup"><span data-stu-id="dde76-142">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="dde76-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dde76-143">Example</span></span>

<span data-ttu-id="dde76-144">In diesem Beispiel benötigen Sie die ID des Geräts und die ID des Befehls, die zu einem Gerät ausgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="dde76-144">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="dde76-145">Das Gerät ID wird zurückgegeben, beim Ausgeben eines GET-Anruf, um `/me/devices`, und rufen Sie der Befehl ID wird zurückgegeben, wenn einen Beitrag wie folgt auf `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="dde76-145">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="dde76-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dde76-146">Request</span></span>

<span data-ttu-id="dde76-147">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="dde76-147">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="dde76-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="dde76-148">Response</span></span>

<span data-ttu-id="dde76-149">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="dde76-149">The following example shows the response.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "value":
  {
    "id": "0158355AD4D680CC4E2994CC009EFFD7337D1335FCA6ED266…",
    "status": "completed",
    "type": null,
    "appServiceName": null,
    "packageFamilyName": null,
    "error": null,
    "permissionTicket": null,
    "postBackUri": null,
    "payload": null
  }
}
```


## <a name="get-command-payload"></a><span data-ttu-id="dde76-150">Abrufen der Befehl Nutzlast</span><span class="sxs-lookup"><span data-stu-id="dde76-150">Get command payload</span></span>

<span data-ttu-id="dde76-151">Rufen Sie eine Antwort Nutzlast für eine bestimmte Aktion auf einem Gerät.</span><span class="sxs-lookup"><span data-stu-id="dde76-151">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="dde76-152">Nutzlast Antwort wird beim Abfragen eines app-Service verwendet, für die Übermittlung von Daten zurück.</span><span class="sxs-lookup"><span data-stu-id="dde76-152">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="dde76-153">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dde76-153">Permissions</span></span>

<span data-ttu-id="dde76-p107">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dde76-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dde76-156">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dde76-156">Permission type</span></span>      | <span data-ttu-id="dde76-157">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dde76-157">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dde76-158">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dde76-158">Delegated (work or school account)</span></span> | <span data-ttu-id="dde76-159">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dde76-159">Not supported.</span></span>    |
|<span data-ttu-id="dde76-160">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dde76-160">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dde76-161">Device.Command</span><span class="sxs-lookup"><span data-stu-id="dde76-161">Device.Command</span></span>    |
|<span data-ttu-id="dde76-162">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dde76-162">Application</span></span> | <span data-ttu-id="dde76-163">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dde76-163">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="dde76-164">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dde76-164">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="dde76-165">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dde76-165">Request headers</span></span>

| <span data-ttu-id="dde76-166">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dde76-166">Header</span></span> |<span data-ttu-id="dde76-167">Wert</span><span class="sxs-lookup"><span data-stu-id="dde76-167">Value</span></span>
|:----|:------|
|<span data-ttu-id="dde76-168">Authorization</span><span class="sxs-lookup"><span data-stu-id="dde76-168">Authorization</span></span>| <span data-ttu-id="dde76-p108">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dde76-p108">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="dde76-171">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dde76-171">Accept</span></span> | <span data-ttu-id="dde76-172">application/json</span><span class="sxs-lookup"><span data-stu-id="dde76-172">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="dde76-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="dde76-173">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"date-time",
  "Type":"Ok"
}
```

### <a name="example"></a><span data-ttu-id="dde76-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dde76-174">Example</span></span>

<span data-ttu-id="dde76-175">In diesem Beispiel benötigen Sie die ID des Geräts und die ID des Befehls, die zu einem Gerät ausgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="dde76-175">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="dde76-176">Rufen Sie das Gerät ID wird zurückgegeben, wenn einen GET ausstellen für `/me/devices`, und rufen Sie der Befehl ID wird zurückgegeben, wenn einen Beitrag wie folgt auf `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="dde76-176">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="dde76-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dde76-177">Request</span></span>

<span data-ttu-id="dde76-178">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="dde76-178">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="dde76-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="dde76-179">Response</span></span>

<span data-ttu-id="dde76-180">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="dde76-180">The following example shows the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"04/27/2017",
  "Type":"Ok"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/get-device-command-status.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
