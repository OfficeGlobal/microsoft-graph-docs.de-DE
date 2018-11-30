---
title: childFolders auflisten
description: Mit dieser API können Sie eine Sammlung von untergeordneten Ordnern im jeweils angegebenen Kontaktordner abrufen.
ms.openlocfilehash: 7d379e81229ee8efd4c12718147a99ed13ebdb93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061230"
---
# <a name="list-childfolders"></a><span data-ttu-id="a95dc-103">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="a95dc-103">List childFolders</span></span>

> <span data-ttu-id="a95dc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a95dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a95dc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a95dc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a95dc-106">Mit dieser API können Sie eine Sammlung von untergeordneten Ordnern im jeweils angegebenen Kontaktordner abrufen.</span><span class="sxs-lookup"><span data-stu-id="a95dc-106">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a95dc-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a95dc-107">Permissions</span></span>
<span data-ttu-id="a95dc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a95dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a95dc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a95dc-110">Permission type</span></span>      | <span data-ttu-id="a95dc-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a95dc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a95dc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a95dc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a95dc-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a95dc-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a95dc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a95dc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a95dc-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a95dc-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a95dc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a95dc-116">Application</span></span> | <span data-ttu-id="a95dc-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a95dc-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a95dc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a95dc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a95dc-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a95dc-119">Optional query parameters</span></span>
<span data-ttu-id="a95dc-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a95dc-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a95dc-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a95dc-121">Request headers</span></span>
| <span data-ttu-id="a95dc-122">Name</span><span class="sxs-lookup"><span data-stu-id="a95dc-122">Name</span></span>       | <span data-ttu-id="a95dc-123">Typ</span><span class="sxs-lookup"><span data-stu-id="a95dc-123">Type</span></span> | <span data-ttu-id="a95dc-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a95dc-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a95dc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a95dc-125">Authorization</span></span>  | <span data-ttu-id="a95dc-126">string</span><span class="sxs-lookup"><span data-stu-id="a95dc-126">string</span></span>  | <span data-ttu-id="a95dc-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a95dc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a95dc-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a95dc-129">Request body</span></span>
<span data-ttu-id="a95dc-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a95dc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a95dc-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a95dc-131">Response</span></span>

<span data-ttu-id="a95dc-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ContactFolder](../resources/contactfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a95dc-132">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a95dc-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a95dc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a95dc-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a95dc-134">Request</span></span>
<span data-ttu-id="a95dc-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a95dc-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="a95dc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a95dc-136">Response</span></span>
<span data-ttu-id="a95dc-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a95dc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
