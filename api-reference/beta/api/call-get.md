---
title: Get call
description: Rufen Sie die Eigenschaften und die Beziehungen eines Anrufs-Objekts ab.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f5f530fac12ae61c47a5a5e3e0f900720aac4c4e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640343"
---
# <a name="get-call"></a><span data-ttu-id="c1020-103">Get call</span><span class="sxs-lookup"><span data-stu-id="c1020-103">Get call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1020-104">Rufen Sie die Eigenschaften und die Beziehungen eines Anrufs-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="c1020-104">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1020-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c1020-105">Permissions</span></span>
<span data-ttu-id="c1020-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1020-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1020-108">Permission type</span></span> | <span data-ttu-id="c1020-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1020-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="c1020-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1020-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1020-111">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1020-111">Not Supported.</span></span>                         |
| <span data-ttu-id="c1020-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1020-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1020-113">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1020-113">Not Supported.</span></span>                         |
| <span data-ttu-id="c1020-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1020-114">Application</span></span>                            | <span data-ttu-id="c1020-115">Keine.</span><span class="sxs-lookup"><span data-stu-id="c1020-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="c1020-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1020-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1020-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c1020-117">Optional query parameters</span></span>
<span data-ttu-id="c1020-118">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="c1020-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1020-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1020-119">Request headers</span></span>
| <span data-ttu-id="c1020-120">Name</span><span class="sxs-lookup"><span data-stu-id="c1020-120">Name</span></span>          | <span data-ttu-id="c1020-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1020-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c1020-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1020-122">Authorization</span></span> | <span data-ttu-id="c1020-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c1020-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1020-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1020-125">Request body</span></span>
<span data-ttu-id="c1020-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c1020-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1020-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1020-127">Response</span></span>
<span data-ttu-id="c1020-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines Objekts [aufrufen,](../resources/call.md) in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c1020-128">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1020-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1020-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c1020-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1020-130">Request</span></span>
<span data-ttu-id="c1020-131">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="c1020-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="c1020-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1020-132">Response</span></span>

> <span data-ttu-id="c1020-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c1020-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
