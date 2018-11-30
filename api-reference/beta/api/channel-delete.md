---
title: DDE-Kanal löschen
description: Löschen Sie den Kanal.
ms.openlocfilehash: 8f34db306ae42493cf23f29117aece6fd4942c2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058042"
---
# <a name="delete-channel"></a><span data-ttu-id="7ad40-103">DDE-Kanal löschen</span><span class="sxs-lookup"><span data-stu-id="7ad40-103">Delete channel</span></span>

> <span data-ttu-id="7ad40-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7ad40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ad40-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ad40-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ad40-106">Löschen Sie den [Kanal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="7ad40-106">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="7ad40-107">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="7ad40-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="7ad40-108">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="7ad40-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="7ad40-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7ad40-109">Permissions</span></span>
<span data-ttu-id="7ad40-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ad40-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ad40-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7ad40-112">Permission type</span></span>      | <span data-ttu-id="7ad40-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7ad40-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ad40-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7ad40-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7ad40-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ad40-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ad40-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7ad40-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ad40-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7ad40-117">Not supported.</span></span>    |
|<span data-ttu-id="7ad40-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7ad40-118">Application</span></span> | <span data-ttu-id="7ad40-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ad40-119">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="7ad40-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ad40-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7ad40-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7ad40-121">Request headers</span></span>
| <span data-ttu-id="7ad40-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7ad40-122">Header</span></span>       | <span data-ttu-id="7ad40-123">Wert</span><span class="sxs-lookup"><span data-stu-id="7ad40-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ad40-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ad40-124">Authorization</span></span>  | <span data-ttu-id="7ad40-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7ad40-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ad40-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7ad40-127">Request body</span></span>
<span data-ttu-id="7ad40-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7ad40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ad40-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ad40-129">Response</span></span>

<span data-ttu-id="7ad40-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7ad40-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ad40-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7ad40-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ad40-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7ad40-133">Request</span></span>
<span data-ttu-id="7ad40-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7ad40-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="7ad40-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7ad40-135">Response</span></span>

<span data-ttu-id="7ad40-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7ad40-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
