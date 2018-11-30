---
title: Erstellen von online-Besprechung
description: Erstellt eine onlinebesprechung im Auftrag eines Benutzers im Textkörper Anforderung angegeben.
ms.openlocfilehash: c2e62ee3e705f93a97af5682679790b7747cdeef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060965"
---
# <a name="create-online-meeting"></a><span data-ttu-id="6b977-103">Erstellen von online-Besprechung</span><span class="sxs-lookup"><span data-stu-id="6b977-103">Create online meeting</span></span>

> <span data-ttu-id="6b977-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6b977-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b977-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b977-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b977-106">Erstellt eine onlinebesprechung im Auftrag eines Benutzers im Textkörper Anforderung angegeben.</span><span class="sxs-lookup"><span data-stu-id="6b977-106">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="6b977-107">**Hinweis**: die Besprechung wird nicht auf den Kalender des Benutzers angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6b977-107">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b977-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6b977-108">Permissions</span></span>
<span data-ttu-id="6b977-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b977-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b977-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b977-111">Permission type</span></span>                        | <span data-ttu-id="6b977-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b977-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6b977-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b977-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b977-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b977-114">Not Supported</span></span>                               |
| <span data-ttu-id="6b977-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b977-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b977-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b977-116">Not Supported</span></span>                               |
| <span data-ttu-id="6b977-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b977-117">Application</span></span>                            | <span data-ttu-id="6b977-118">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b977-118">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="6b977-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b977-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="6b977-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b977-120">Request headers</span></span>
| <span data-ttu-id="6b977-121">Name</span><span class="sxs-lookup"><span data-stu-id="6b977-121">Name</span></span>          | <span data-ttu-id="6b977-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6b977-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6b977-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b977-123">Authorization</span></span> | <span data-ttu-id="6b977-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b977-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b977-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b977-126">Request body</span></span>
<span data-ttu-id="6b977-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [OnlineMeeting](../resources/onlinemeeting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6b977-127">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6b977-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b977-128">Response</span></span>
<span data-ttu-id="6b977-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortcode und ein [OnlineMeeting](../resources/onlinemeeting.md) -Objekt aus der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6b977-129">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b977-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b977-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6b977-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b977-131">Request</span></span>
<span data-ttu-id="6b977-132">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="6b977-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_onlineMeeting_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/app/onlineMeetings
Content-Type: application/json
Content-Length: 1553

{
  "meetingType": "meetNow",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  },
  "subject": "subject-value"
}
```

<span data-ttu-id="6b977-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OnlineMeeting](../resources/onlinemeeting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6b977-133">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="6b977-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b977-134">Response</span></span>

><span data-ttu-id="6b977-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="6b977-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1574

{
  "accessLevel": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "participantPasscode": "2425999",
    "leaderPasscode": null,
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": "2018-03-19T09:46:02Z",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2018-03-19T09:46:02Z",
  "endDateTime": "2018-03-19T09:46:02Z",
  "entryExitAnnouncement": true,
  "expirationDateTime": "2018-03-19T09:46:02Z",
  "id": "013448345",
  "isCancelled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "meetingType": "meetNow",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "startDateTime": "2018-03-19T09:46:02Z",
  "subject": "Quarterly sales numbers"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
