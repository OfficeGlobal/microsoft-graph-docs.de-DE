---
title: Ressource abrufen
description: Mit dieser API können Sie die Binärdateien eines Objekts des Typs resource mit der Eigenschaft „file“ oder der Eigenschaft „image“ abrufen.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 9937040d9e53213946df9eb31cf9136bcfda7c71
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946063"
---
# <a name="get-resource"></a><span data-ttu-id="06cc0-103">Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="06cc0-103">Get resource</span></span>

<span data-ttu-id="06cc0-104">Mit dieser API können Sie die Binärdateien eines Objekts des Typs [resource](../resources/resource.md) mit der Eigenschaft „file“ oder der Eigenschaft „image“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="06cc0-104">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="06cc0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06cc0-105">Permissions</span></span>
<span data-ttu-id="06cc0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06cc0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06cc0-108">Permission type</span></span>      | <span data-ttu-id="06cc0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06cc0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06cc0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06cc0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06cc0-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06cc0-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="06cc0-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06cc0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06cc0-113">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06cc0-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="06cc0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06cc0-114">Application</span></span> | <span data-ttu-id="06cc0-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06cc0-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06cc0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06cc0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="06cc0-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06cc0-117">Request headers</span></span>
| <span data-ttu-id="06cc0-118">Name</span><span class="sxs-lookup"><span data-stu-id="06cc0-118">Name</span></span>       | <span data-ttu-id="06cc0-119">Typ</span><span class="sxs-lookup"><span data-stu-id="06cc0-119">Type</span></span> | <span data-ttu-id="06cc0-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06cc0-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06cc0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06cc0-121">Authorization</span></span>  | <span data-ttu-id="06cc0-122">string</span><span class="sxs-lookup"><span data-stu-id="06cc0-122">string</span></span>  | <span data-ttu-id="06cc0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06cc0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06cc0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06cc0-125">Request body</span></span>
<span data-ttu-id="06cc0-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="06cc0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06cc0-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="06cc0-127">Response</span></span>

<span data-ttu-id="06cc0-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die Binärdaten des Bilds oder der Datei im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06cc0-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="06cc0-129">Hinweis: Bilder werden nicht direkt in einem Browser gerendert, da zum Abrufen eine Autorisierung erforderlich ist, ebenso wie für den Rest des Seiteninhalts.</span><span class="sxs-lookup"><span data-stu-id="06cc0-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="06cc0-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06cc0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06cc0-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06cc0-131">Request</span></span>
<span data-ttu-id="06cc0-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06cc0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="06cc0-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="06cc0-133">Response</span></span>
<span data-ttu-id="06cc0-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="06cc0-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
