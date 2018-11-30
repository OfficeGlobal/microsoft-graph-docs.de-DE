---
title: Ressource abrufen
description: Mit dieser API können Sie die Binärdateien eines Objekts des Typs resource mit der Eigenschaft „file“ oder der Eigenschaft „image“ abrufen.
ms.openlocfilehash: 81c07dca78381ede096c62eba73b0842ae294d55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058739"
---
# <a name="get-resource"></a><span data-ttu-id="65ca0-103">Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="65ca0-103">Get resource</span></span>

> <span data-ttu-id="65ca0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="65ca0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65ca0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65ca0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65ca0-106">Mit dieser API können Sie die Binärdateien eines Objekts des Typs [resource](../resources/resource.md) mit der Eigenschaft „file“ oder der Eigenschaft „image“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="65ca0-106">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="65ca0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="65ca0-107">Permissions</span></span>
<span data-ttu-id="65ca0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65ca0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65ca0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65ca0-110">Permission type</span></span>      | <span data-ttu-id="65ca0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65ca0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65ca0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65ca0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="65ca0-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65ca0-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="65ca0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65ca0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65ca0-115">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65ca0-115">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="65ca0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65ca0-116">Application</span></span> | <span data-ttu-id="65ca0-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65ca0-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65ca0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65ca0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="65ca0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65ca0-119">Request headers</span></span>
| <span data-ttu-id="65ca0-120">Name</span><span class="sxs-lookup"><span data-stu-id="65ca0-120">Name</span></span>       | <span data-ttu-id="65ca0-121">Typ</span><span class="sxs-lookup"><span data-stu-id="65ca0-121">Type</span></span> | <span data-ttu-id="65ca0-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65ca0-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="65ca0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65ca0-123">Authorization</span></span>  | <span data-ttu-id="65ca0-124">string</span><span class="sxs-lookup"><span data-stu-id="65ca0-124">string</span></span>  | <span data-ttu-id="65ca0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="65ca0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65ca0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65ca0-127">Request body</span></span>
<span data-ttu-id="65ca0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="65ca0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65ca0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="65ca0-129">Response</span></span>

<span data-ttu-id="65ca0-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die Binärdaten des Bilds oder der Datei im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65ca0-130">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="65ca0-131">Hinweis: Bilder werden nicht direkt in einem Browser gerendert, da zum Abrufen eine Autorisierung erforderlich ist, ebenso wie für den Rest des Seiteninhalts.</span><span class="sxs-lookup"><span data-stu-id="65ca0-131">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="65ca0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="65ca0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65ca0-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65ca0-133">Request</span></span>
<span data-ttu-id="65ca0-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65ca0-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="65ca0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="65ca0-135">Response</span></span>
<span data-ttu-id="65ca0-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="65ca0-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
