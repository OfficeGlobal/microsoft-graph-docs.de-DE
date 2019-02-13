---
title: childFolders auflisten
description: 'Rufen Sie die Ordner-Auflistung, unter dem angegebenen Ordner. Sie können die `.../me/MailFolders` Verknüpfung zum Abrufen der obersten Ebene '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 96dec9ca1ba6dbd8e50e8eb978756a98657d2c9d
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967235"
---
# <a name="list-childfolders"></a><span data-ttu-id="b25ed-104">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="b25ed-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b25ed-p102">Dient zum Abrufen der Ordnersammlung unter dem angegebenen Ordner. Sie können die `.../me/MailFolders`-Verknüpfung zum Abrufen der Ordnersammlung auf oberster Ebene und zum Navigieren zu einem anderen Ordner verwenden.</span><span class="sxs-lookup"><span data-stu-id="b25ed-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b25ed-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b25ed-107">Permissions</span></span>

<span data-ttu-id="b25ed-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b25ed-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b25ed-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b25ed-110">Permission type</span></span>                        | <span data-ttu-id="b25ed-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b25ed-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="b25ed-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b25ed-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b25ed-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b25ed-113">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="b25ed-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b25ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b25ed-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b25ed-115">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="b25ed-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b25ed-116">Application</span></span>                            | <span data-ttu-id="b25ed-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b25ed-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="b25ed-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b25ed-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b25ed-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b25ed-119">Optional query parameters</span></span>

<span data-ttu-id="b25ed-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b25ed-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b25ed-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b25ed-121">Request headers</span></span>

| <span data-ttu-id="b25ed-122">Name</span><span class="sxs-lookup"><span data-stu-id="b25ed-122">Name</span></span>          | <span data-ttu-id="b25ed-123">Typ</span><span class="sxs-lookup"><span data-stu-id="b25ed-123">Type</span></span>   | <span data-ttu-id="b25ed-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b25ed-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="b25ed-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b25ed-125">Authorization</span></span> | <span data-ttu-id="b25ed-126">string</span><span class="sxs-lookup"><span data-stu-id="b25ed-126">string</span></span> | <span data-ttu-id="b25ed-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b25ed-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b25ed-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b25ed-129">Request body</span></span>

<span data-ttu-id="b25ed-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b25ed-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b25ed-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b25ed-131">Response</span></span>

<span data-ttu-id="b25ed-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [MailFolder](../resources/mailfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b25ed-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b25ed-133">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b25ed-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="b25ed-134">In Beispiel 1: Liste e-Mail-Ordner</span><span class="sxs-lookup"><span data-stu-id="b25ed-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="b25ed-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b25ed-135">Request</span></span>

<span data-ttu-id="b25ed-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b25ed-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="b25ed-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="b25ed-137">Response</span></span>

<span data-ttu-id="b25ed-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b25ed-138">The following is an example of the response.</span></span>

> <span data-ttu-id="b25ed-139">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="b25ed-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b25ed-140">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b25ed-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="b25ed-141">Beispiel 2: Liste Mail Suchordner</span><span class="sxs-lookup"><span data-stu-id="b25ed-141">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="b25ed-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b25ed-142">Request</span></span>

<span data-ttu-id="b25ed-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b25ed-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="b25ed-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b25ed-144">Response</span></span>

<span data-ttu-id="b25ed-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b25ed-145">The following is an example of the response.</span></span>

> <span data-ttu-id="b25ed-146">**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden.</span><span class="sxs-lookup"><span data-stu-id="b25ed-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b25ed-147">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b25ed-147">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMz",
      "displayName": "Get MyAnalytics",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 6,
      "totalItemCount": 6,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'MyAnalytics')"
    },
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMy",
      "displayName": "Action Required",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 4,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'ACTION REQUIRED')"
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
