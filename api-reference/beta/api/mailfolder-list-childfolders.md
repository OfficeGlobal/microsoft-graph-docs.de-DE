---
title: childFolders auflisten
description: 'Rufen Sie die Ordner-Auflistung, unter dem angegebenen Ordner. Sie können die `.../me/MailFolders` Verknüpfung zum Abrufen der obersten Ebene '
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 3af208919b1f733e913d8ac374bb72608d8fa1aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837436"
---
# <a name="list-childfolders"></a><span data-ttu-id="208e1-104">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="208e1-104">List childFolders</span></span>

> <span data-ttu-id="208e1-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="208e1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="208e1-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="208e1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="208e1-p103">Dient zum Abrufen der Ordnersammlung unter dem angegebenen Ordner. Sie können die `.../me/MailFolders`-Verknüpfung zum Abrufen der Ordnersammlung auf oberster Ebene und zum Navigieren zu einem anderen Ordner verwenden.</span><span class="sxs-lookup"><span data-stu-id="208e1-p103">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="208e1-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="208e1-109">Permissions</span></span>
<span data-ttu-id="208e1-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="208e1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="208e1-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="208e1-112">Permission type</span></span>      | <span data-ttu-id="208e1-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="208e1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="208e1-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="208e1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="208e1-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="208e1-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="208e1-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="208e1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="208e1-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="208e1-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="208e1-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="208e1-118">Application</span></span> | <span data-ttu-id="208e1-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="208e1-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="208e1-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="208e1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="208e1-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="208e1-121">Optional query parameters</span></span>
<span data-ttu-id="208e1-122">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="208e1-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="208e1-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="208e1-123">Request headers</span></span>
| <span data-ttu-id="208e1-124">Name</span><span class="sxs-lookup"><span data-stu-id="208e1-124">Name</span></span>       | <span data-ttu-id="208e1-125">Typ</span><span class="sxs-lookup"><span data-stu-id="208e1-125">Type</span></span> | <span data-ttu-id="208e1-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="208e1-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="208e1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="208e1-127">Authorization</span></span>  | <span data-ttu-id="208e1-128">string</span><span class="sxs-lookup"><span data-stu-id="208e1-128">string</span></span>  | <span data-ttu-id="208e1-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="208e1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="208e1-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="208e1-131">Request body</span></span>
<span data-ttu-id="208e1-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="208e1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="208e1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="208e1-133">Response</span></span>
<span data-ttu-id="208e1-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [MailFolder](../resources/mailfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="208e1-134">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="208e1-135">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="208e1-135">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="208e1-136">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="208e1-136">Request 1</span></span>
<span data-ttu-id="208e1-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="208e1-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

#### <a name="response-1"></a><span data-ttu-id="208e1-138">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="208e1-138">Response 1</span></span>
<span data-ttu-id="208e1-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="208e1-139">The following is an example of the response.</span></span>
><span data-ttu-id="208e1-140">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="208e1-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="208e1-141">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="208e1-141">All the properties will be returned from an actual call.</span></span>

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

## <a name="example-2"></a><span data-ttu-id="208e1-142">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="208e1-142">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="208e1-143">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="208e1-143">Request 2</span></span>
<span data-ttu-id="208e1-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="208e1-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response-2"></a><span data-ttu-id="208e1-145">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="208e1-145">Response 2</span></span>
<span data-ttu-id="208e1-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="208e1-146">The following is an example of the response.</span></span>
><span data-ttu-id="208e1-147">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="208e1-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="208e1-148">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="208e1-148">All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
