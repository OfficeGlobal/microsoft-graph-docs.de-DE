---
title: Patch-Kanal
description: Aktualisieren Sie die Eigenschaften des angegebenen Kanals.
ms.openlocfilehash: 833b5cf4999f43e9de799691a9f6d7a98318d4fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058317"
---
# <a name="patch-channel"></a><span data-ttu-id="f02ed-103">Patch-Kanal</span><span class="sxs-lookup"><span data-stu-id="f02ed-103">Patch channel</span></span>

> <span data-ttu-id="f02ed-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f02ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f02ed-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f02ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f02ed-106">Aktualisieren Sie die Eigenschaften des angegebenen [DDE-Kanal](../resources/channel.md)an.</span><span class="sxs-lookup"><span data-stu-id="f02ed-106">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="f02ed-107">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="f02ed-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="f02ed-108">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="f02ed-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="f02ed-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f02ed-109">Permissions</span></span>
<span data-ttu-id="f02ed-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f02ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f02ed-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f02ed-112">Permission type</span></span>      | <span data-ttu-id="f02ed-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f02ed-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f02ed-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f02ed-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f02ed-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f02ed-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f02ed-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f02ed-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f02ed-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f02ed-117">Not supported.</span></span>    |
|<span data-ttu-id="f02ed-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f02ed-118">Application</span></span> | <span data-ttu-id="f02ed-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f02ed-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f02ed-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f02ed-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f02ed-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f02ed-121">Request headers</span></span>
| <span data-ttu-id="f02ed-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f02ed-122">Header</span></span>       | <span data-ttu-id="f02ed-123">Wert</span><span class="sxs-lookup"><span data-stu-id="f02ed-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f02ed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f02ed-124">Authorization</span></span>  | <span data-ttu-id="f02ed-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f02ed-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f02ed-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f02ed-127">Content-Type</span></span>  | <span data-ttu-id="f02ed-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f02ed-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f02ed-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f02ed-129">Request body</span></span>
<span data-ttu-id="f02ed-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Channel](../resources/channel.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f02ed-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f02ed-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f02ed-131">Response</span></span>

<span data-ttu-id="f02ed-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f02ed-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f02ed-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f02ed-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f02ed-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f02ed-134">Request</span></span>
<span data-ttu-id="f02ed-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f02ed-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="f02ed-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f02ed-136">Response</span></span>
<span data-ttu-id="f02ed-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f02ed-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
