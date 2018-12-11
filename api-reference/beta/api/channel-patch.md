---
title: Patch-Kanal
description: Aktualisieren Sie die Eigenschaften des angegebenen Kanals.
ms.openlocfilehash: c7cc2db83fbab0e04f1620d71c4c7cf7a69b526f
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222380"
---
# <a name="patch-channel"></a><span data-ttu-id="07d71-103">Patch-Kanal</span><span class="sxs-lookup"><span data-stu-id="07d71-103">Patch channel</span></span>

> <span data-ttu-id="07d71-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07d71-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07d71-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07d71-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07d71-106">Aktualisieren Sie die Eigenschaften des angegebenen [DDE-Kanal](../resources/channel.md)an.</span><span class="sxs-lookup"><span data-stu-id="07d71-106">Update the properties of the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="07d71-107">**Hinweis**: Es ist ein bekanntes Problem mit Berechtigungen und diese API.</span><span class="sxs-lookup"><span data-stu-id="07d71-107">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="07d71-108">Weitere Informationen hierzu finden Sie unter der [Problemliste bezeichnet](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="07d71-108">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="07d71-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07d71-109">Permissions</span></span>
<span data-ttu-id="07d71-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07d71-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07d71-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07d71-112">Permission type</span></span>      | <span data-ttu-id="07d71-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07d71-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07d71-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07d71-114">Delegated (work or school account)</span></span> | <span data-ttu-id="07d71-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d71-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="07d71-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07d71-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07d71-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07d71-117">Not supported.</span></span>    |
|<span data-ttu-id="07d71-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07d71-118">Application</span></span> | <span data-ttu-id="07d71-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d71-119">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="07d71-120">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="07d71-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="07d71-121">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="07d71-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="07d71-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07d71-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="07d71-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07d71-123">Request headers</span></span>
| <span data-ttu-id="07d71-124">Header</span><span class="sxs-lookup"><span data-stu-id="07d71-124">Header</span></span>       | <span data-ttu-id="07d71-125">Wert</span><span class="sxs-lookup"><span data-stu-id="07d71-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="07d71-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="07d71-126">Authorization</span></span>  | <span data-ttu-id="07d71-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07d71-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="07d71-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="07d71-129">Content-Type</span></span>  | <span data-ttu-id="07d71-130">application/json</span><span class="sxs-lookup"><span data-stu-id="07d71-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="07d71-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07d71-131">Request body</span></span>
<span data-ttu-id="07d71-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Channel](../resources/channel.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="07d71-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="07d71-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="07d71-133">Response</span></span>

<span data-ttu-id="07d71-134">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07d71-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07d71-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07d71-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07d71-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07d71-136">Request</span></span>
<span data-ttu-id="07d71-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="07d71-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="07d71-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="07d71-138">Response</span></span>
<span data-ttu-id="07d71-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07d71-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
