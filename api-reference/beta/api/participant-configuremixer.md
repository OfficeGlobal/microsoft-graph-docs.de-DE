---
title: 'Teilnehmer: ConfigureMixer'
description: Konfigurieren Sie, wie Audio für andere Teilnehmer an einer Unterhaltung mit mehreren Teilnehmern gemischt wird.
author: VinodRavichandran
ms.openlocfilehash: c15cbc8a8de5a9ba7d7f3c20d20f99bf61006dbf
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380464"
---
# <a name="participant-configuremixer"></a><span data-ttu-id="99873-103">Teilnehmer: ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="99873-103">participant: configureMixer</span></span>

> <span data-ttu-id="99873-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="99873-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99873-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99873-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99873-106">Konfigurieren Sie, wie Audio für andere Teilnehmer an einer Unterhaltung mit mehreren Teilnehmern gemischt wird.</span><span class="sxs-lookup"><span data-stu-id="99873-106">Configure how audio is mixed for different participants in a multiparty conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="99873-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="99873-107">Permissions</span></span>
<span data-ttu-id="99873-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99873-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="99873-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99873-110">Permission type</span></span> | <span data-ttu-id="99873-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99873-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="99873-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99873-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="99873-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99873-113">Not Supported</span></span>        |
| <span data-ttu-id="99873-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99873-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99873-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99873-115">Not Supported</span></span>        |
| <span data-ttu-id="99873-116">Application</span><span class="sxs-lookup"><span data-stu-id="99873-116">Application</span></span>     | <span data-ttu-id="99873-117">Calls.JoinGroupCalls.All Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="99873-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99873-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99873-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/configureMixer
POST /applications/{id}/calls/{id}/participants/configureMixer
```

## <a name="request-headers"></a><span data-ttu-id="99873-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99873-119">Request headers</span></span>
| <span data-ttu-id="99873-120">Name</span><span class="sxs-lookup"><span data-stu-id="99873-120">Name</span></span>          | <span data-ttu-id="99873-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99873-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="99873-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99873-122">Authorization</span></span> | <span data-ttu-id="99873-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99873-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99873-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99873-125">Request body</span></span>
<span data-ttu-id="99873-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="99873-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="99873-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="99873-127">Parameter</span></span>      | <span data-ttu-id="99873-128">Typ</span><span class="sxs-lookup"><span data-stu-id="99873-128">Type</span></span>    |<span data-ttu-id="99873-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99873-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99873-130">participantMixerLevels</span><span class="sxs-lookup"><span data-stu-id="99873-130">participantMixerLevels</span></span>|<span data-ttu-id="99873-131">[ParticipantMixerLevel](../resources/participantmixerlevel.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="99873-131">[participantMixerLevel](../resources/participantmixerlevel.md) collection</span></span>| <span data-ttu-id="99873-132">Konfiguration der Mixer Ebenen für gegebene audio-Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="99873-132">Configuration of mixer levels for given audio participant.</span></span>|
|<span data-ttu-id="99873-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="99873-133">clientContext</span></span>|<span data-ttu-id="99873-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="99873-134">String</span></span>|<span data-ttu-id="99873-135">Der Clientkontext.</span><span class="sxs-lookup"><span data-stu-id="99873-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="99873-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="99873-136">Response</span></span>
<span data-ttu-id="99873-137">Gibt `202 Accepted` Antwortcode und ein Location-Header mit einem Uri, um die [CommsOperation](../resources/commsoperation.md) für diese Anforderung erstellt.</span><span class="sxs-lookup"><span data-stu-id="99873-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="99873-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99873-138">Example</span></span>
<span data-ttu-id="99873-139">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="99873-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="99873-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99873-140">Request</span></span>
<span data-ttu-id="99873-141">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="99873-141">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "participant-configureMixer"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/configureMixer
Content-Type: application/json
Content-Length: 501

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "participantMixerLevels": [
    {
      "participant": "550fae72-d251-43ec-868c-373732c2704f",
      "exclusive": true,
      "ducking": {
        "rampActive": 50,
        "rampInactive": 50,
        "lowerLevel": 10,
        "upperLevel": 50
      },
      "sourceLevels": [
        {
          "participant": "632899f8-2ea1-4604-8413-27bd2892079f",
          "level": 50,
          "duckOthers": false
        }
      ]
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="99873-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="99873-142">Response</span></span>

> <span data-ttu-id="99873-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="99873-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

##### <a name="notification---operation-completed"></a><span data-ttu-id="99873-145">Benachrichtigung - Vorgang abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="99873-145">Notification - operation completed</span></span>

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
        "@odata.type": "#microsoft.graph.commsOperation",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896/operations/0FE0623FD62842EDB4BD8AC290072CC5",
        "@odata.etag": "W/\"1\"",
        "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
        "status": "completed"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant: configureMixer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
