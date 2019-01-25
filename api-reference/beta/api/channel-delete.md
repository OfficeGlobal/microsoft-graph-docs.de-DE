---
title: DDE-Kanal löschen
description: Löschen Sie den Kanal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 734df0a79881993f4e002562e5125305b624c4c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525332"
---
# <a name="delete-channel"></a><span data-ttu-id="6b2af-103">DDE-Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="6b2af-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b2af-104">Löschen Sie den [Kanal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="6b2af-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="6b2af-105">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="6b2af-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="6b2af-106">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="6b2af-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b2af-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6b2af-107">Permissions</span></span>
<span data-ttu-id="6b2af-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b2af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b2af-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b2af-110">Permission type</span></span>      | <span data-ttu-id="6b2af-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b2af-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b2af-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b2af-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6b2af-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b2af-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b2af-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b2af-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b2af-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b2af-115">Not supported.</span></span>    |
|<span data-ttu-id="6b2af-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b2af-116">Application</span></span> | <span data-ttu-id="6b2af-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b2af-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="6b2af-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="6b2af-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6b2af-119">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="6b2af-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6b2af-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b2af-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6b2af-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b2af-121">Request headers</span></span>
| <span data-ttu-id="6b2af-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6b2af-122">Header</span></span>       | <span data-ttu-id="6b2af-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6b2af-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b2af-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b2af-124">Authorization</span></span>  | <span data-ttu-id="6b2af-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b2af-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b2af-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b2af-127">Request body</span></span>
<span data-ttu-id="6b2af-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6b2af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b2af-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b2af-129">Response</span></span>

<span data-ttu-id="6b2af-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b2af-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b2af-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b2af-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b2af-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b2af-133">Request</span></span>
<span data-ttu-id="6b2af-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b2af-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="6b2af-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b2af-135">Response</span></span>

<span data-ttu-id="6b2af-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6b2af-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
