---
title: childFolders auflisten
description: 'Rufen Sie die Ordner-Auflistung, unter dem angegebenen Ordner. Sie können die `.../me/MailFolders` Verknüpfung zum Abrufen der obersten Ebene '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9d54828b97bb82c9ce0ee9eceeee86a4aa975c3d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512549"
---
# <a name="list-childfolders"></a><span data-ttu-id="2634b-104">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="2634b-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2634b-p102">Dient zum Abrufen der Ordnersammlung unter dem angegebenen Ordner. Sie können die `.../me/MailFolders`-Verknüpfung zum Abrufen der Ordnersammlung auf oberster Ebene und zum Navigieren zu einem anderen Ordner verwenden.</span><span class="sxs-lookup"><span data-stu-id="2634b-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="2634b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2634b-107">Permissions</span></span>
<span data-ttu-id="2634b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2634b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2634b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2634b-110">Permission type</span></span>      | <span data-ttu-id="2634b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2634b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2634b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2634b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2634b-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2634b-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2634b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2634b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2634b-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2634b-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2634b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2634b-116">Application</span></span> | <span data-ttu-id="2634b-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2634b-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2634b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2634b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2634b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2634b-119">Optional query parameters</span></span>
<span data-ttu-id="2634b-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2634b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2634b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2634b-121">Request headers</span></span>
| <span data-ttu-id="2634b-122">Name</span><span class="sxs-lookup"><span data-stu-id="2634b-122">Name</span></span>       | <span data-ttu-id="2634b-123">Typ</span><span class="sxs-lookup"><span data-stu-id="2634b-123">Type</span></span> | <span data-ttu-id="2634b-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2634b-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2634b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2634b-125">Authorization</span></span>  | <span data-ttu-id="2634b-126">string</span><span class="sxs-lookup"><span data-stu-id="2634b-126">string</span></span>  | <span data-ttu-id="2634b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2634b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2634b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2634b-129">Request body</span></span>
<span data-ttu-id="2634b-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2634b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2634b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2634b-131">Response</span></span>
<span data-ttu-id="2634b-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [MailFolder](../resources/mailfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2634b-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="2634b-133">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="2634b-133">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="2634b-134">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="2634b-134">Request 1</span></span>
<span data-ttu-id="2634b-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2634b-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

#### <a name="response-1"></a><span data-ttu-id="2634b-136">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="2634b-136">Response 1</span></span>
<span data-ttu-id="2634b-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2634b-137">The following is an example of the response.</span></span>
><span data-ttu-id="2634b-138">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="2634b-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2634b-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2634b-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
        "id": "AAMkAGVmMDEzA",
        "displayName": "Internal Screens",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 2,
        "totalItemCount": 2,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzB",
        "displayName": "Project Falcon",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 5,
        "totalItemCount": 5,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzMA",
        "displayName": "Finder",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 4,
        "unreadItemCount": 0,
        "totalItemCount": 0,
        "wellKnownName": "searchfolders"
    }
  ]
}
```

## <a name="example-2"></a><span data-ttu-id="2634b-140">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="2634b-140">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="2634b-141">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="2634b-141">Request 2</span></span>
<span data-ttu-id="2634b-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2634b-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response-2"></a><span data-ttu-id="2634b-143">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="2634b-143">Response 2</span></span>
<span data-ttu-id="2634b-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2634b-144">The following is an example of the response.</span></span>
><span data-ttu-id="2634b-145">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="2634b-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2634b-146">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2634b-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
        "id": "AAMkAGVmMDEzA",
        "displayName": "Internal Screens",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 2,
        "totalItemCount": 2,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzB",
        "displayName": "Project Falcon",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 5,
        "totalItemCount": 5,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzMA",
        "displayName": "Finder",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 4,
        "unreadItemCount": 0,
        "totalItemCount": 0,
        "wellKnownName": "searchfolders"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
