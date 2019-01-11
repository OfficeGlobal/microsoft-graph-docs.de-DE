---
title: Abrufen von Anrufen
description: Rufen Sie die Eigenschaften und die Beziehungen eines Anrufs-Objekts ab.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c209c263f2dfcffe274bf726296d7e6c427afa6d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833551"
---
# <a name="get-call"></a><span data-ttu-id="b99b3-103">Abrufen von Anrufen</span><span class="sxs-lookup"><span data-stu-id="b99b3-103">Get call</span></span>

> <span data-ttu-id="b99b3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b99b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b99b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b99b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b99b3-106">Rufen Sie die Eigenschaften und die Beziehungen eines Anrufs-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="b99b3-106">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b99b3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b99b3-107">Permissions</span></span>
<span data-ttu-id="b99b3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b99b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b99b3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b99b3-110">Permission type</span></span> | <span data-ttu-id="b99b3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b99b3-111">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="b99b3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b99b3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b99b3-113">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b99b3-113">Not Supported.</span></span>                         |
| <span data-ttu-id="b99b3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b99b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b99b3-115">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b99b3-115">Not Supported.</span></span>                         |
| <span data-ttu-id="b99b3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b99b3-116">Application</span></span>                            | <span data-ttu-id="b99b3-117">Keine.</span><span class="sxs-lookup"><span data-stu-id="b99b3-117">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="b99b3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b99b3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b99b3-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b99b3-119">Optional query parameters</span></span>
<span data-ttu-id="b99b3-120">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="b99b3-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b99b3-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b99b3-121">Request headers</span></span>
| <span data-ttu-id="b99b3-122">Name</span><span class="sxs-lookup"><span data-stu-id="b99b3-122">Name</span></span>          | <span data-ttu-id="b99b3-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b99b3-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b99b3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b99b3-124">Authorization</span></span> | <span data-ttu-id="b99b3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b99b3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b99b3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b99b3-127">Request body</span></span>
<span data-ttu-id="b99b3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b99b3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b99b3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b99b3-129">Response</span></span>
<span data-ttu-id="b99b3-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines Objekts [aufrufen,](../resources/call.md) in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b99b3-130">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b99b3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b99b3-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b99b3-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b99b3-132">Request</span></span>
<span data-ttu-id="b99b3-133">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="b99b3-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="b99b3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b99b3-134">Response</span></span>

> <span data-ttu-id="b99b3-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b99b3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2821

{
  "activeModalities": [
    "unknown"
  ],
  "answeredBy": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "callRoutes": [
    {
      "final": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "original": {
        "phone": {
          "id": "+14258828080"
        }
      },
      "routingType": "forwarded"
    }
  ],
  "callbackUri": "callbackUri-value",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "direction": "incoming",
  "id": "id-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "meetingCapability": {
    "allowAnonymousUsersToDialOut": true,
    "allowAnonymousUsersToStartMeeting": true,
    "autoAdmittedUsers": "everyoneInCompany"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "allowConversationWithoutHost": true
  },
  "myParticipantId": "myParticipantId-value",
  "requestedModalities": [
    "audio", "video"
  ],
  "ringingTimeoutInSeconds": 99,
  "routingPolicies": [
    "none"
  ],
  "source": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "state": "incoming",
  "subject": "subject-value",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value"
    }
  ],
  "tenantId": "tenantId-value",
  "terminationReason": "terminationReason-value",
  "toneInfo": {
    "sequenceId": 99,
    "tone": "tone0"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
