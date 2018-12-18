---
title: Mitglieder auflisten
description: Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.
author: lleonard-msft
ms.openlocfilehash: 8bd0f67d6ca565dac6dfae501f5bc5c829f4db3b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359101"
---
# <a name="list-members"></a><span data-ttu-id="81b5c-104">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="81b5c-104">List members</span></span>

> <span data-ttu-id="81b5c-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="81b5c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81b5c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81b5c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81b5c-p103">Dient zum Abrufen einer Liste der Benutzer, die der Verzeichnisrolle zugeordnet sind.  Nur Benutzer können einer Verzeichnisrolle zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="81b5c-p103">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="81b5c-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="81b5c-109">Permissions</span></span>
<span data-ttu-id="81b5c-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81b5c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="81b5c-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="81b5c-112">Permission type</span></span>      | <span data-ttu-id="81b5c-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="81b5c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81b5c-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="81b5c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="81b5c-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81b5c-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81b5c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="81b5c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81b5c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="81b5c-117">Not supported.</span></span>    |
|<span data-ttu-id="81b5c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="81b5c-118">Application</span></span> | <span data-ttu-id="81b5c-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81b5c-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81b5c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="81b5c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="81b5c-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="81b5c-121">Optional query parameters</span></span>
<span data-ttu-id="81b5c-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="81b5c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="81b5c-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="81b5c-123">Request headers</span></span>
| <span data-ttu-id="81b5c-124">Name</span><span class="sxs-lookup"><span data-stu-id="81b5c-124">Name</span></span>       | <span data-ttu-id="81b5c-125">Typ</span><span class="sxs-lookup"><span data-stu-id="81b5c-125">Type</span></span> | <span data-ttu-id="81b5c-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81b5c-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="81b5c-127">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="81b5c-127">Authorization</span></span>  | <span data-ttu-id="81b5c-128">string</span><span class="sxs-lookup"><span data-stu-id="81b5c-128">string</span></span>  | <span data-ttu-id="81b5c-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="81b5c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81b5c-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="81b5c-131">Request body</span></span>
<span data-ttu-id="81b5c-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="81b5c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81b5c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="81b5c-133">Response</span></span>

<span data-ttu-id="81b5c-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81b5c-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="81b5c-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="81b5c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81b5c-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="81b5c-136">Request</span></span>
<span data-ttu-id="81b5c-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="81b5c-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="81b5c-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="81b5c-138">Response</span></span>
<span data-ttu-id="81b5c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81b5c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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