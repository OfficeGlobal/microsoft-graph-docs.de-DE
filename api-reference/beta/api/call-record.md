---
title: 'Rufen Sie: Datensatz'
description: Notieren Sie den Anruf.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1f119cfece969c01e68773e5985eab4010dc9874
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574859"
---
# <a name="call-record"></a><span data-ttu-id="4d672-103">Rufen Sie: Datensatz</span><span class="sxs-lookup"><span data-stu-id="4d672-103">call: record</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d672-104">Notieren Sie den Anruf.</span><span class="sxs-lookup"><span data-stu-id="4d672-104">Record the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d672-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d672-105">Permissions</span></span>
<span data-ttu-id="4d672-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d672-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d672-108">Permission type</span></span> | <span data-ttu-id="4d672-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d672-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="4d672-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d672-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d672-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d672-111">Not Supported</span></span>        |
| <span data-ttu-id="4d672-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d672-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d672-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d672-113">Not Supported</span></span>        |
| <span data-ttu-id="4d672-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d672-114">Application</span></span>     | <span data-ttu-id="4d672-115">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="4d672-115">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="4d672-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d672-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/record
POST /applications/{id}/calls/{id}/record
```

## <a name="request-headers"></a><span data-ttu-id="4d672-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d672-117">Request headers</span></span>
| <span data-ttu-id="4d672-118">Name</span><span class="sxs-lookup"><span data-stu-id="4d672-118">Name</span></span>          | <span data-ttu-id="4d672-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d672-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4d672-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d672-120">Authorization</span></span> | <span data-ttu-id="4d672-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d672-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d672-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d672-123">Request body</span></span>
<span data-ttu-id="4d672-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4d672-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d672-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="4d672-125">Parameter</span></span>      | <span data-ttu-id="4d672-126">Typ</span><span class="sxs-lookup"><span data-stu-id="4d672-126">Type</span></span>    |<span data-ttu-id="4d672-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d672-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d672-128">fordert</span><span class="sxs-lookup"><span data-stu-id="4d672-128">prompts</span></span>|<span data-ttu-id="4d672-129">[MediaPrompt](../resources/mediaprompt.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4d672-129">[mediaPrompt](../resources/mediaprompt.md) collection</span></span> | <span data-ttu-id="4d672-130">Auflistung von Ansagen wiedergegeben (falls vorhanden) vor der Aufzeichnung startet.</span><span class="sxs-lookup"><span data-stu-id="4d672-130">Collection of prompts to play (if any) before recording starts.</span></span> <span data-ttu-id="4d672-131">Kunden die Möglichkeit, geben Sie "PlayPrompt" Aktion separat oder als Teil des "Aufzeichnen" - hauptsächlich alle Datensätze einer Aufforderung vorangestellt werden</span><span class="sxs-lookup"><span data-stu-id="4d672-131">Customers can choose to specify "playPrompt" action separately or specify as part of "record" - mostly all records are preceeded by a prompt</span></span> |
|<span data-ttu-id="4d672-132">bargeInAllowed</span><span class="sxs-lookup"><span data-stu-id="4d672-132">bargeInAllowed</span></span>|<span data-ttu-id="4d672-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d672-133">Boolean</span></span>| <span data-ttu-id="4d672-134">Benutzern Sie die Eingabe Auswahl, bevor Aufforderung beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="4d672-134">Allow users to enter choice before prompt finishes.</span></span>                                                                 |
|<span data-ttu-id="4d672-135">initialSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="4d672-135">initialSilenceTimeoutInSeconds</span></span> | <span data-ttu-id="4d672-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4d672-136">Int32</span></span>| <span data-ttu-id="4d672-137">Maximale anfänglichen Silence zulässig, von dem Zeitpunkt wir den Eintrag Vorgang bevor wir Timeout und Fehlschlagen des Vorgangs zu starten.</span><span class="sxs-lookup"><span data-stu-id="4d672-137">Maximum initial silence allowed from the time we start the record operation before we timeout and fail the operation.</span></span> <span data-ttu-id="4d672-138">Wenn wir eine Aufforderung spielen, startet dieser Zeitgeber nach Aufforderung abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="4d672-138">If we are playing a prompt, then this timer starts after prompt finishes.</span></span> |
|<span data-ttu-id="4d672-139">maxSilenceTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="4d672-139">maxSilenceTimeoutInSeconds</span></span>|<span data-ttu-id="4d672-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4d672-140">Int32</span></span>| <span data-ttu-id="4d672-141">Die maximale Silence Timeout in Sekunden.</span><span class="sxs-lookup"><span data-stu-id="4d672-141">The maximum silence timeout in seconds.</span></span>|
|<span data-ttu-id="4d672-142">maxRecordDurationInSeconds</span><span class="sxs-lookup"><span data-stu-id="4d672-142">maxRecordDurationInSeconds</span></span>|<span data-ttu-id="4d672-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4d672-143">Int32</span></span>| <span data-ttu-id="4d672-144">Die maximale Anzahl von Datensätzen Dauer in Sekunden.</span><span class="sxs-lookup"><span data-stu-id="4d672-144">The maximum record duration in seconds.</span></span>|
|<span data-ttu-id="4d672-145">playBeep</span><span class="sxs-lookup"><span data-stu-id="4d672-145">playBeep</span></span>|<span data-ttu-id="4d672-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d672-146">Boolean</span></span>| <span data-ttu-id="4d672-147">Gibt einen Signalton nach Wiedergabe der Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="4d672-147">Plays a beep after playing the prompt.</span></span>|
|<span data-ttu-id="4d672-148">streamWhileRecording</span><span class="sxs-lookup"><span data-stu-id="4d672-148">streamWhileRecording</span></span>|<span data-ttu-id="4d672-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d672-149">Boolean</span></span>|<span data-ttu-id="4d672-150">Wenn es sich bei Festlegung auf true festgelegt ist, einen Speicherort der Ressource bereitgestellt werden, sobald die Aufzeichnung gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="4d672-150">If set to true, a resource location will be provided as soon as the recording starts.</span></span> |
|<span data-ttu-id="4d672-151">stopTones</span><span class="sxs-lookup"><span data-stu-id="4d672-151">stopTones</span></span>|<span data-ttu-id="4d672-152">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4d672-152">String collection</span></span>|<span data-ttu-id="4d672-153">Beenden Sie Töne angegeben, um die Aufzeichnung zu beenden.</span><span class="sxs-lookup"><span data-stu-id="4d672-153">Stop tones specified to end recording.</span></span>|
|<span data-ttu-id="4d672-154">clientContext</span><span class="sxs-lookup"><span data-stu-id="4d672-154">clientContext</span></span>|<span data-ttu-id="4d672-155">String</span><span class="sxs-lookup"><span data-stu-id="4d672-155">String</span></span>|<span data-ttu-id="4d672-156">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="4d672-156">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="4d672-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d672-157">Response</span></span>
<span data-ttu-id="4d672-158">Gibt `202 Accepted` Antwortcode und ein Location-Header mit einem Uri, um die [CommsOperation](../resources/commsoperation.md) für diese Anforderung erstellt.</span><span class="sxs-lookup"><span data-stu-id="4d672-158">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="4d672-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d672-159">Example</span></span>
<span data-ttu-id="4d672-160">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="4d672-160">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4d672-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d672-161">Request</span></span>
<span data-ttu-id="4d672-162">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="4d672-162">The following example shows the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="4d672-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d672-163">Response</span></span>

> <span data-ttu-id="4d672-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4d672-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.recordOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="4d672-166">Benachrichtigung - Vorgang abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="4d672-166">Notification - operation completed</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "call: record",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-record.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
