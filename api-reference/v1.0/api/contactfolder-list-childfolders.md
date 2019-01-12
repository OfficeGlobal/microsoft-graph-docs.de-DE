---
title: childFolders auflisten
description: Mit dieser API können Sie eine Sammlung von untergeordneten Ordnern im jeweils angegebenen Kontaktordner abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3d0f6d14249e488333954b3a45c3bed0f6eaf93a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987797"
---
# <a name="list-childfolders"></a><span data-ttu-id="4ddfe-103">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="4ddfe-103">List childFolders</span></span>

<span data-ttu-id="4ddfe-104">Mit dieser API können Sie eine Sammlung von untergeordneten Ordnern im jeweils angegebenen Kontaktordner abrufen.</span><span class="sxs-lookup"><span data-stu-id="4ddfe-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ddfe-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4ddfe-105">Permissions</span></span>
<span data-ttu-id="4ddfe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ddfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ddfe-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ddfe-108">Permission type</span></span>      | <span data-ttu-id="4ddfe-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ddfe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ddfe-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ddfe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4ddfe-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ddfe-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4ddfe-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ddfe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ddfe-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ddfe-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4ddfe-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ddfe-114">Application</span></span> | <span data-ttu-id="4ddfe-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ddfe-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ddfe-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ddfe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ddfe-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4ddfe-117">Optional query parameters</span></span>
<span data-ttu-id="4ddfe-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4ddfe-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4ddfe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ddfe-119">Request headers</span></span>
| <span data-ttu-id="4ddfe-120">Name</span><span class="sxs-lookup"><span data-stu-id="4ddfe-120">Name</span></span>       | <span data-ttu-id="4ddfe-121">Typ</span><span class="sxs-lookup"><span data-stu-id="4ddfe-121">Type</span></span> | <span data-ttu-id="4ddfe-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ddfe-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4ddfe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ddfe-123">Authorization</span></span>  | <span data-ttu-id="4ddfe-124">string</span><span class="sxs-lookup"><span data-stu-id="4ddfe-124">string</span></span>  | <span data-ttu-id="4ddfe-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4ddfe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ddfe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ddfe-127">Request body</span></span>
<span data-ttu-id="4ddfe-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4ddfe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ddfe-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ddfe-129">Response</span></span>

<span data-ttu-id="4ddfe-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ContactFolder](../resources/contactfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ddfe-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ddfe-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ddfe-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ddfe-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ddfe-132">Request</span></span>
<span data-ttu-id="4ddfe-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ddfe-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="4ddfe-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ddfe-134">Response</span></span>
<span data-ttu-id="4ddfe-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ddfe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
