---
title: Update-team
description: Aktualisieren Sie die Eigenschaften des angegebenen Teams.
ms.openlocfilehash: 9d07fd687facc96c1bc4a93c37cb492b321518e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059410"
---
# <a name="update-team"></a><span data-ttu-id="83c45-103">Update-team</span><span class="sxs-lookup"><span data-stu-id="83c45-103">Update team</span></span>

> <span data-ttu-id="83c45-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="83c45-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83c45-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83c45-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="83c45-106">Aktualisieren Sie die Eigenschaften des angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="83c45-106">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83c45-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="83c45-107">Permissions</span></span>
<span data-ttu-id="83c45-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83c45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="83c45-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83c45-110">Permission type</span></span>      | <span data-ttu-id="83c45-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83c45-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83c45-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83c45-112">Delegated (work or school account)</span></span> | <span data-ttu-id="83c45-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83c45-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="83c45-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="83c45-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83c45-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83c45-115">Not supported.</span></span>    |
|<span data-ttu-id="83c45-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83c45-116">Application</span></span> | <span data-ttu-id="83c45-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83c45-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="83c45-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83c45-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="83c45-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83c45-119">Request headers</span></span>
| <span data-ttu-id="83c45-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="83c45-120">Header</span></span>       | <span data-ttu-id="83c45-121">Wert</span><span class="sxs-lookup"><span data-stu-id="83c45-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83c45-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="83c45-122">Authorization</span></span>  | <span data-ttu-id="83c45-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="83c45-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="83c45-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83c45-125">Content-Type</span></span>  | <span data-ttu-id="83c45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83c45-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83c45-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83c45-127">Request body</span></span>
<span data-ttu-id="83c45-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Team](../resources/team.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="83c45-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="83c45-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="83c45-129">Response</span></span>

<span data-ttu-id="83c45-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="83c45-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="83c45-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="83c45-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="83c45-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83c45-132">Request</span></span>
<span data-ttu-id="83c45-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83c45-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  }
}
```
#### <a name="response"></a><span data-ttu-id="83c45-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="83c45-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
