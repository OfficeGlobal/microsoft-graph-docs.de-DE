---
title: Mitglieder auflisten
description: Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ad27b5d4a56bee9e149b9f6de87271a86e9945e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970808"
---
# <a name="list-members"></a><span data-ttu-id="d23a4-104">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="d23a4-104">List members</span></span>

> <span data-ttu-id="d23a4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d23a4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d23a4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d23a4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d23a4-p103">Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="d23a4-p103">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="d23a4-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d23a4-109">Permissions</span></span>
<span data-ttu-id="d23a4-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d23a4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d23a4-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d23a4-112">Permission type</span></span>      | <span data-ttu-id="d23a4-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d23a4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d23a4-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d23a4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d23a4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d23a4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d23a4-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d23a4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d23a4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d23a4-117">Not supported.</span></span>    |
|<span data-ttu-id="d23a4-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d23a4-118">Application</span></span> | <span data-ttu-id="d23a4-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d23a4-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d23a4-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d23a4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d23a4-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d23a4-121">Optional query parameters</span></span>
<span data-ttu-id="d23a4-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d23a4-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d23a4-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d23a4-123">Request headers</span></span>
| <span data-ttu-id="d23a4-124">Name</span><span class="sxs-lookup"><span data-stu-id="d23a4-124">Name</span></span>       | <span data-ttu-id="d23a4-125">Typ</span><span class="sxs-lookup"><span data-stu-id="d23a4-125">Type</span></span> | <span data-ttu-id="d23a4-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d23a4-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d23a4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d23a4-127">Authorization</span></span>  | <span data-ttu-id="d23a4-128">string</span><span class="sxs-lookup"><span data-stu-id="d23a4-128">string</span></span>  | <span data-ttu-id="d23a4-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d23a4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d23a4-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d23a4-131">Request body</span></span>
<span data-ttu-id="d23a4-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d23a4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d23a4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d23a4-133">Response</span></span>

<span data-ttu-id="d23a4-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d23a4-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d23a4-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d23a4-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d23a4-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d23a4-136">Request</span></span>
<span data-ttu-id="d23a4-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d23a4-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="d23a4-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="d23a4-138">Response</span></span>
<span data-ttu-id="d23a4-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d23a4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
