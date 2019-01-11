---
title: Befehl Gerätestatus anfordern.
description: Rufen Sie den Status eines Befehls auf einem Gerät. Die vollständige Liste der Statuscodes finden Sie unter Liste der ActionStatus.
localization_priority: Normal
ms.openlocfilehash: 9dca743a50f248abee76fb4d54352df3d400ada1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883132"
---
# <a name="get-device-command-status"></a><span data-ttu-id="f18e3-104">Befehl Gerätestatus anfordern.</span><span class="sxs-lookup"><span data-stu-id="f18e3-104">Get device command status</span></span>

> <span data-ttu-id="f18e3-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f18e3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f18e3-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f18e3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f18e3-107">Rufen Sie den Status eines Befehls auf einem Gerät.</span><span class="sxs-lookup"><span data-stu-id="f18e3-107">Get the status of a command on a device.</span></span> <span data-ttu-id="f18e3-108">Die vollständige Liste der Statuscodes finden Sie unter [Liste der ActionStatus](#list-of-actionstatus).</span><span class="sxs-lookup"><span data-stu-id="f18e3-108">For the  full list of status codes, see [List of actionStatus](#list-of-actionstatus).</span></span>

## <a name="permissions"></a><span data-ttu-id="f18e3-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f18e3-109">Permissions</span></span>

<span data-ttu-id="f18e3-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f18e3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f18e3-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f18e3-112">Permission type</span></span>      | <span data-ttu-id="f18e3-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f18e3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f18e3-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f18e3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f18e3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f18e3-115">Not supported.</span></span>    |
|<span data-ttu-id="f18e3-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f18e3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f18e3-117">Device.Command</span><span class="sxs-lookup"><span data-stu-id="f18e3-117">Device.Command</span></span>    |
|<span data-ttu-id="f18e3-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f18e3-118">Application</span></span> | <span data-ttu-id="f18e3-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f18e3-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f18e3-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f18e3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f18e3-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f18e3-121">Request headers</span></span>

| <span data-ttu-id="f18e3-122">Header</span><span class="sxs-lookup"><span data-stu-id="f18e3-122">Header</span></span> |<span data-ttu-id="f18e3-123">Wert</span><span class="sxs-lookup"><span data-stu-id="f18e3-123">Value</span></span>
|:----|:------|
|<span data-ttu-id="f18e3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f18e3-124">Authorization</span></span>| <span data-ttu-id="f18e3-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f18e3-p105">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f18e3-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f18e3-127">Accept</span></span> | <span data-ttu-id="f18e3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f18e3-128">application/json</span></span> |

## <a name="response"></a><span data-ttu-id="f18e3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f18e3-129">Response</span></span>
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

## <a name="list-of-actionstatus"></a><span data-ttu-id="f18e3-130">Liste der actionStatus</span><span class="sxs-lookup"><span data-stu-id="f18e3-130">List of actionStatus</span></span>

- <span data-ttu-id="f18e3-131">Anfordern von / / Befehl erstellt wurde und wartet auf Verarbeitung</span><span class="sxs-lookup"><span data-stu-id="f18e3-131">requesting, // Command has been created and is waiting to be processed</span></span>
- <span data-ttu-id="f18e3-132">SentToTarget, / / Befehl an das Gerät gesendet wurde</span><span class="sxs-lookup"><span data-stu-id="f18e3-132">sentToTarget, // Command has been sent to the target device</span></span>
- <span data-ttu-id="f18e3-133">ausführen, / / Zielgerät Bestätigung des Befehls bestätigt und ausgeführt wird</span><span class="sxs-lookup"><span data-stu-id="f18e3-133">executing, // Target device acknowledged receipt of the command and is executing it</span></span>
- <span data-ttu-id="f18e3-134">abgeschlossen, / / Command Ausführung beendet</span><span class="sxs-lookup"><span data-stu-id="f18e3-134">completed, // Command execution completed</span></span>
- <span data-ttu-id="f18e3-135">FailedToSend, / / -Dienst konnte nicht auf das Zielgerät Befehl senden</span><span class="sxs-lookup"><span data-stu-id="f18e3-135">failedToSend, // Service failed to send command to target device</span></span>
- <span data-ttu-id="f18e3-136">ExecutionFailed, / / Command fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="f18e3-136">executionFailed, // Command execution failed</span></span>
- <span data-ttu-id="f18e3-137">CommandDropped, / / Befehl vom Client gelöscht, wenn ConnectedStandby Gerät ist</span><span class="sxs-lookup"><span data-stu-id="f18e3-137">commandDropped, // Command dropped by client if device is in ConnectedStandby state</span></span>
- <span data-ttu-id="f18e3-138">Abbrechen, / / Abbrechen des Befehls</span><span class="sxs-lookup"><span data-stu-id="f18e3-138">cancel, // Cancel the command</span></span>
- <span data-ttu-id="f18e3-139">Abbrechen, / / den Befehl wird abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="f18e3-139">cancelling, // Cancelling the command</span></span>
- <span data-ttu-id="f18e3-140">abgebrochen, / / Befehl wurde abgebrochen</span><span class="sxs-lookup"><span data-stu-id="f18e3-140">canceled, // Command has been cancelled</span></span>
- <span data-ttu-id="f18e3-141">Wiederholen, / / Dienst wird zum Senden von Befehl an Ziel wiederholen</span><span class="sxs-lookup"><span data-stu-id="f18e3-141">retry, // Service is retrying to send command to target</span></span>
- <span data-ttu-id="f18e3-142">abgelaufen, / / Befehl Verarbeitung Ablaufzeit überschritten</span><span class="sxs-lookup"><span data-stu-id="f18e3-142">expired, // Command processing exceeded expiry time</span></span>
- <span data-ttu-id="f18e3-143">Fehler: / / Interner Fehler beim Ausführen des Befehls</span><span class="sxs-lookup"><span data-stu-id="f18e3-143">error, // Internal error while processing the command</span></span>
- <span data-ttu-id="f18e3-144">Benutzerdefinierte / / benutzerdefinierte Status</span><span class="sxs-lookup"><span data-stu-id="f18e3-144">custom // Custom status</span></span>

## <a name="example"></a><span data-ttu-id="f18e3-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f18e3-145">Example</span></span>

<span data-ttu-id="f18e3-146">In diesem Beispiel benötigen Sie die ID des Geräts und die ID des Befehls, die zu einem Gerät ausgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f18e3-146">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="f18e3-147">Das Gerät ID wird zurückgegeben, beim Ausgeben eines GET-Anruf, um `/me/devices`, und rufen Sie der Befehl ID wird zurückgegeben, wenn einen Beitrag wie folgt auf `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="f18e3-147">The device ID is returned when issuing a GET call to `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="f18e3-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f18e3-148">Request</span></span>

<span data-ttu-id="f18e3-149">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="f18e3-149">The following example shows the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="f18e3-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="f18e3-150">Response</span></span>

<span data-ttu-id="f18e3-151">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="f18e3-151">The following example shows the response.</span></span>
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


## <a name="get-command-payload"></a><span data-ttu-id="f18e3-152">Abrufen der Befehl Nutzlast</span><span class="sxs-lookup"><span data-stu-id="f18e3-152">Get command payload</span></span>

<span data-ttu-id="f18e3-153">Rufen Sie eine Antwort Nutzlast für eine bestimmte Aktion auf einem Gerät.</span><span class="sxs-lookup"><span data-stu-id="f18e3-153">Get a response payload for a specific action on a device.</span></span> <span data-ttu-id="f18e3-154">Nutzlast Antwort wird beim Abfragen eines app-Service verwendet, für die Übermittlung von Daten zurück.</span><span class="sxs-lookup"><span data-stu-id="f18e3-154">The response payload is used when querying an app service to carry data back.</span></span>


### <a name="permissions"></a><span data-ttu-id="f18e3-155">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f18e3-155">Permissions</span></span>

<span data-ttu-id="f18e3-p108">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f18e3-p108">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f18e3-158">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f18e3-158">Permission type</span></span>      | <span data-ttu-id="f18e3-159">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f18e3-159">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f18e3-160">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f18e3-160">Delegated (work or school account)</span></span> | <span data-ttu-id="f18e3-161">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f18e3-161">Not supported.</span></span>    |
|<span data-ttu-id="f18e3-162">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f18e3-162">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f18e3-163">Device.Command</span><span class="sxs-lookup"><span data-stu-id="f18e3-163">Device.Command</span></span>    |
|<span data-ttu-id="f18e3-164">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f18e3-164">Application</span></span> | <span data-ttu-id="f18e3-165">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f18e3-165">Not supported.</span></span> |

### <a name="http-request"></a><span data-ttu-id="f18e3-166">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f18e3-166">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a><span data-ttu-id="f18e3-167">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f18e3-167">Request headers</span></span>

| <span data-ttu-id="f18e3-168">Header</span><span class="sxs-lookup"><span data-stu-id="f18e3-168">Header</span></span> |<span data-ttu-id="f18e3-169">Wert</span><span class="sxs-lookup"><span data-stu-id="f18e3-169">Value</span></span>
|:----|:------|
|<span data-ttu-id="f18e3-170">Authorization</span><span class="sxs-lookup"><span data-stu-id="f18e3-170">Authorization</span></span>| <span data-ttu-id="f18e3-p109">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f18e3-p109">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f18e3-173">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f18e3-173">Accept</span></span> | <span data-ttu-id="f18e3-174">application/json</span><span class="sxs-lookup"><span data-stu-id="f18e3-174">application/json</span></span> |

### <a name="response"></a><span data-ttu-id="f18e3-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="f18e3-175">Response</span></span>
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

### <a name="example"></a><span data-ttu-id="f18e3-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f18e3-176">Example</span></span>

<span data-ttu-id="f18e3-177">In diesem Beispiel benötigen Sie die ID des Geräts und die ID des Befehls, die zu einem Gerät ausgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f18e3-177">In this example, you will need the ID of the device and the ID of the command that has been issued to a device.</span></span> <span data-ttu-id="f18e3-178">Rufen Sie das Gerät ID wird zurückgegeben, wenn einen GET ausstellen für `/me/devices`, und rufen Sie der Befehl ID wird zurückgegeben, wenn einen Beitrag wie folgt auf `/me/devices/{id}/command`.</span><span class="sxs-lookup"><span data-stu-id="f18e3-178">The device ID is returned when issuing a GET call on `/me/devices`, and the command ID is returned when doing a POST call on `/me/devices/{id}/command`.</span></span>

#### <a name="request"></a><span data-ttu-id="f18e3-179">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f18e3-179">Request</span></span>

<span data-ttu-id="f18e3-180">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="f18e3-180">The following example shows the request.</span></span>

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a><span data-ttu-id="f18e3-181">Antwort</span><span class="sxs-lookup"><span data-stu-id="f18e3-181">Response</span></span>

<span data-ttu-id="f18e3-182">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="f18e3-182">The following example shows the response.</span></span>

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
