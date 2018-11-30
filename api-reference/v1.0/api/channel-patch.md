---
title: Patch-Kanal
description: Aktualisieren Sie die Eigenschaften des angegebenen Kanals.
ms.openlocfilehash: 981de62dcedb42b98016aa99ccaaa8b5cd27ba9c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020121"
---
# <a name="patch-channel"></a><span data-ttu-id="9f970-103">Patch-Kanal</span><span class="sxs-lookup"><span data-stu-id="9f970-103">Patch channel</span></span>



<span data-ttu-id="9f970-104">Aktualisieren Sie die Eigenschaften des angegebenen [DDE-Kanal](../resources/channel.md)an.</span><span class="sxs-lookup"><span data-stu-id="9f970-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="9f970-105">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="9f970-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="9f970-106">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="9f970-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f970-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f970-107">Permissions</span></span>
<span data-ttu-id="9f970-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f970-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f970-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f970-110">Permission type</span></span>      | <span data-ttu-id="9f970-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f970-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f970-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f970-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9f970-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f970-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9f970-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f970-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f970-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f970-115">Not supported.</span></span>    |
|<span data-ttu-id="9f970-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f970-116">Application</span></span> | <span data-ttu-id="9f970-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f970-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f970-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f970-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9f970-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f970-119">Request headers</span></span>
| <span data-ttu-id="9f970-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9f970-120">Header</span></span>       | <span data-ttu-id="9f970-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9f970-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f970-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f970-122">Authorization</span></span>  | <span data-ttu-id="9f970-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f970-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9f970-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f970-125">Content-Type</span></span>  | <span data-ttu-id="9f970-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f970-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f970-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f970-127">Request body</span></span>
<span data-ttu-id="9f970-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Channel](../resources/channel.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9f970-128">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9f970-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f970-129">Response</span></span>

<span data-ttu-id="9f970-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f970-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9f970-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f970-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f970-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f970-132">Request</span></span>
<span data-ttu-id="9f970-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f970-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="9f970-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f970-134">Response</span></span>
<span data-ttu-id="9f970-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f970-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
