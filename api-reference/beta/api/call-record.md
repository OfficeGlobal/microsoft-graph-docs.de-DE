---
title: 'Rufen Sie: Datensatz'
description: Notieren Sie den Anruf.
author: VinodRavichandran
ms.openlocfilehash: 44b204a1185881cc9e1c96867e906c658c0d5ed9
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380520"
---
# <a name="call-record"></a><span data-ttu-id="b3b64-103">Rufen Sie: Datensatz</span><span class="sxs-lookup"><span data-stu-id="b3b64-103">call: record</span></span>

> <span data-ttu-id="b3b64-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b3b64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3b64-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3b64-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3b64-106">Notieren Sie den Anruf.</span><span class="sxs-lookup"><span data-stu-id="b3b64-106">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3b64-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b3b64-107">Permissions</span></span>
<span data-ttu-id="b3b64-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3b64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3b64-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3b64-110">Permission type</span></span> | <span data-ttu-id="b3b64-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3b64-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="b3b64-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3b64-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3b64-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3b64-113">Not Supported</span></span>        |
| <span data-ttu-id="b3b64-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3b64-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3b64-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3b64-115">Not Supported</span></span>        |
| <span data-ttu-id="b3b64-116">Application</span><span class="sxs-lookup"><span data-stu-id="b3b64-116">Application</span></span>     | <span data-ttu-id="b3b64-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="b3b64-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="b3b64-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3b64-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="b3b64-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3b64-119">Request headers</span></span>
| <span data-ttu-id="b3b64-120">Name</span><span class="sxs-lookup"><span data-stu-id="b3b64-120">Name</span></span>          | <span data-ttu-id="b3b64-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3b64-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b3b64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3b64-122">Authorization</span></span> | <span data-ttu-id="b3b64-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b3b64-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3b64-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3b64-125">Request body</span></span>
<span data-ttu-id="b3b64-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b3b64-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b3b64-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="b3b64-127">Parameter</span></span>      | <span data-ttu-id="b3b64-128">Typ</span><span class="sxs-lookup"><span data-stu-id="b3b64-128">Type</span></span>    |<span data-ttu-id="b3b64-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3b64-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3b64-130">fordert</span><span class="sxs-lookup"><span data-stu-id="b3b64-130">prompts</span></span>|<span data-ttu-id="b3b64-131">[Mediaprompt](../resources/mediaprompt.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b3b64-131">[mediaprompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="b3b64-132">Auflistung von Ansagen wiedergegeben (falls vorhanden) vor der Aufzeichnung startet.</span><span class="sxs-lookup"><span data-stu-id="b3b64-132">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="b3b64-133">Kunden die Möglichkeit, geben Sie "PlayPrompt" Aktion separat oder als Teil des "Aufzeichnen" - hauptsächlich alle Datensätze einer Aufforderung vorangestellt werden</span><span class="sxs-lookup"><span data-stu-id="b3b64-133">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="b3b64-134">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="b3b64-134">bargeInAllowed</span></span>|<span data-ttu-id="b3b64-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b3b64-135">Boolean</span></span>| <span data-ttu-id="b3b64-136">Benutzern Sie die Eingabe Auswahl, bevor Aufforderung beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="b3b64-136">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="b3b64-137">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b3b64-137">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="b3b64-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b3b64-138">Int32</span></span>| <span data-ttu-id="b3b64-139">Maximale anfänglichen Silence zulässig, von dem Zeitpunkt wir den Eintrag Vorgang bevor wir Timeout und Fehlschlagen des Vorgangs zu starten.</span><span class="sxs-lookup"><span data-stu-id="b3b64-139">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="b3b64-140">Wenn wir eine Aufforderung spielen, startet dieser Zeitgeber nach Aufforderung abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="b3b64-140">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="b3b64-141">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b3b64-141">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="b3b64-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b3b64-142">Int32</span></span>| <span data-ttu-id="b3b64-143">Die maximale Silence Timeout in Sekunden.</span><span class="sxs-lookup"><span data-stu-id="b3b64-143">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="b3b64-144">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="b3b64-144">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="b3b64-145">Int32</span><span class="sxs-lookup"><span data-stu-id="b3b64-145">Int32</span></span>| <span data-ttu-id="b3b64-146">Die maximale Anzahl von Datensätzen Dauer in Sekunden.</span><span class="sxs-lookup"><span data-stu-id="b3b64-146">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="b3b64-147">playBeep</span><span class="sxs-lookup"><span data-stu-id="b3b64-147">playBeep</span></span>|<span data-ttu-id="b3b64-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b3b64-148">Boolean</span></span>| <span data-ttu-id="b3b64-149">Gibt einen Signalton nach Wiedergabe der Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="b3b64-149">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="b3b64-150">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="b3b64-150">streamWhileRecording</span></span>|<span data-ttu-id="b3b64-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b3b64-151">Boolean</span></span>|<span data-ttu-id="b3b64-152">Wenn es sich bei Festlegung auf true festgelegt ist, einen Speicherort der Ressource bereitgestellt werden, sobald die Aufzeichnung gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="b3b64-152">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="b3b64-153">stopTones</span><span class="sxs-lookup"><span data-stu-id="b3b64-153">stopTones</span></span>|<span data-ttu-id="b3b64-154">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="b3b64-154">String collection</span></span>|<span data-ttu-id="b3b64-155">Beenden Sie Töne angegeben, um die Aufzeichnung zu beenden.</span><span class="sxs-lookup"><span data-stu-id="b3b64-155">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="b3b64-156">clientContext</span><span class="sxs-lookup"><span data-stu-id="b3b64-156">clientContext</span></span>|<span data-ttu-id="b3b64-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3b64-157">String</span></span>|<span data-ttu-id="b3b64-158">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="b3b64-158">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="b3b64-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3b64-159">Response</span></span>
<span data-ttu-id="b3b64-160">Gibt `202 Accepted` Antwortcode und ein Location-Header mit einem Uri, um die [CommsOperation](../resources/commsoperation.md) für diese Anforderung erstellt.</span><span class="sxs-lookup"><span data-stu-id="b3b64-160">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="b3b64-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3b64-161">Example</span></span>
<span data-ttu-id="b3b64-162">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="b3b64-162">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b3b64-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3b64-163">Request</span></span>
<span data-ttu-id="b3b64-164">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="b3b64-164">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-record"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/record
Content-Type: application/json
Content-Length: 394

{
  "bargeInAllowed": true,
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "prompts": [
    {
      "@odata.type": "#microsoft.graph.mediaPrompt",
      "mediaInfo": {
        "uri": "https://cdn.contoso.com/beep.wav",
        "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      "loop": 5
    }
  ],
  "maxRecordDurationInSeconds": 1800,
  "initialSilenceTimeoutInSeconds": 10,
  "maxSilenceTimeoutInSeconds": 2,
  "recordingFormat": "wav",
  "playBeep": true,
  "streamWhileRecording": true,
  "stopTones": [ "#", "11", "*" ]
}
```

##### <a name="response"></a><span data-ttu-id="b3b64-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3b64-165">Response</span></span>

> <span data-ttu-id="b3b64-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b3b64-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="b3b64-168">Benachrichtigung - Vorgang abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="b3b64-168">Notification - operation completed</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
      "resourceData": {
        "@odata.type": "#microsoft.graph.recordOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"54451\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed",
        "recordResourceLocation": "https://file.location/17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
        "recordResourceAccessToken": "<access-token>",
        "completionReason": "stopToneDetected"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
