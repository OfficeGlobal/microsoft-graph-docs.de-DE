---
title: Besitzer auflisten
description: Abrufen einer Liste von DirectoryObject-Objekten.
ms.openlocfilehash: 2db43b62d1d30813ed80e6d612e5c0d2770e283d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058701"
---
# <a name="list-owners"></a><span data-ttu-id="e2488-103">Besitzer auflisten</span><span class="sxs-lookup"><span data-stu-id="e2488-103">List owners</span></span>

> <span data-ttu-id="e2488-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e2488-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2488-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2488-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2488-106">Abrufen einer Liste von DirectoryObject-Objekten.</span><span class="sxs-lookup"><span data-stu-id="e2488-106">Retrieve a list of directoryObject objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2488-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e2488-107">Permissions</span></span>
<span data-ttu-id="e2488-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2488-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2488-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2488-110">Permission type</span></span>      | <span data-ttu-id="e2488-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2488-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2488-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2488-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2488-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2488-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e2488-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2488-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2488-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2488-115">Not supported.</span></span>    |
|<span data-ttu-id="e2488-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2488-116">Application</span></span> | <span data-ttu-id="e2488-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2488-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2488-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2488-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2488-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e2488-119">Optional query parameters</span></span>
<span data-ttu-id="e2488-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e2488-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2488-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2488-121">Request headers</span></span>
| <span data-ttu-id="e2488-122">Name</span><span class="sxs-lookup"><span data-stu-id="e2488-122">Name</span></span>       | <span data-ttu-id="e2488-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e2488-123">Type</span></span> | <span data-ttu-id="e2488-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2488-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e2488-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2488-125">Authorization</span></span>  | <span data-ttu-id="e2488-126">string</span><span class="sxs-lookup"><span data-stu-id="e2488-126">string</span></span>  | <span data-ttu-id="e2488-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e2488-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e2488-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2488-129">Request body</span></span>
<span data-ttu-id="e2488-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e2488-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2488-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2488-131">Response</span></span>

<span data-ttu-id="e2488-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2488-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2488-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2488-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2488-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2488-134">Request</span></span>
<span data-ttu-id="e2488-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2488-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
##### <a name="response"></a><span data-ttu-id="e2488-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2488-136">Response</span></span>
<span data-ttu-id="e2488-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2488-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->