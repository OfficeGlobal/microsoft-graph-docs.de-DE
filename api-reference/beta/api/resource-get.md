---
title: Ressource abrufen
description: Mit dieser API können Sie die Binärdateien eines Objekts des Typs resource mit der Eigenschaft „file“ oder der Eigenschaft „image“ abrufen.
localization_priority: Normal
ms.openlocfilehash: 1f8150e0449009eef4d1afe2ce014ae848153382
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841258"
---
# <a name="get-resource"></a><span data-ttu-id="e1ed5-103">Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="e1ed5-103">Get resource</span></span>

> <span data-ttu-id="e1ed5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1ed5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1ed5-106">Mit dieser API können Sie die Binärdateien eines Objekts des Typs [resource](../resources/resource.md) mit der Eigenschaft „file“ oder der Eigenschaft „image“ abrufen.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-106">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1ed5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e1ed5-107">Permissions</span></span>
<span data-ttu-id="e1ed5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1ed5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1ed5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1ed5-110">Permission type</span></span>      | <span data-ttu-id="e1ed5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1ed5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1ed5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1ed5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e1ed5-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ed5-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1ed5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1ed5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1ed5-115">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1ed5-115">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e1ed5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1ed5-116">Application</span></span> | <span data-ttu-id="e1ed5-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ed5-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1ed5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1ed5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="e1ed5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1ed5-119">Request headers</span></span>
| <span data-ttu-id="e1ed5-120">Name</span><span class="sxs-lookup"><span data-stu-id="e1ed5-120">Name</span></span>       | <span data-ttu-id="e1ed5-121">Typ</span><span class="sxs-lookup"><span data-stu-id="e1ed5-121">Type</span></span> | <span data-ttu-id="e1ed5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1ed5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e1ed5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1ed5-123">Authorization</span></span>  | <span data-ttu-id="e1ed5-124">string</span><span class="sxs-lookup"><span data-stu-id="e1ed5-124">string</span></span>  | <span data-ttu-id="e1ed5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1ed5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1ed5-127">Request body</span></span>
<span data-ttu-id="e1ed5-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1ed5-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1ed5-129">Response</span></span>

<span data-ttu-id="e1ed5-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die Binärdaten des Bilds oder der Datei im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-130">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="e1ed5-131">Hinweis: Bilder werden nicht direkt in einem Browser gerendert, da zum Abrufen eine Autorisierung erforderlich ist, ebenso wie für den Rest des Seiteninhalts.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-131">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="e1ed5-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1ed5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1ed5-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1ed5-133">Request</span></span>
<span data-ttu-id="e1ed5-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="e1ed5-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1ed5-135">Response</span></span>
<span data-ttu-id="e1ed5-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e1ed5-136">Here is an example of the response.</span></span>
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
