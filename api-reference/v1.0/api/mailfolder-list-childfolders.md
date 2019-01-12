---
title: childFolders auflisten
description: 'Rufen Sie die Ordner-Auflistung, unter dem angegebenen Ordner. Sie können die `.../me/MailFolders` Verknüpfung zum Abrufen der obersten Ebene '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 3fec593d1d1b29e84f43e46d4bee7ef8f4aa61d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935402"
---
# <a name="list-childfolders"></a><span data-ttu-id="9d109-104">childFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="9d109-104">List childFolders</span></span>

<span data-ttu-id="9d109-p102">Dient zum Abrufen der Ordnersammlung unter dem angegebenen Ordner. Sie können die `.../me/MailFolders`-Verknüpfung zum Abrufen der Ordnersammlung auf oberster Ebene und zum Navigieren zu einem anderen Ordner verwenden.</span><span class="sxs-lookup"><span data-stu-id="9d109-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d109-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9d109-107">Permissions</span></span>
<span data-ttu-id="9d109-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d109-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d109-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d109-110">Permission type</span></span>      | <span data-ttu-id="9d109-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d109-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d109-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d109-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d109-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d109-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9d109-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d109-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d109-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d109-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9d109-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d109-116">Application</span></span> | <span data-ttu-id="9d109-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d109-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d109-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d109-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d109-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9d109-119">Optional query parameters</span></span>
<span data-ttu-id="9d109-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9d109-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9d109-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d109-121">Request headers</span></span>
| <span data-ttu-id="9d109-122">Name</span><span class="sxs-lookup"><span data-stu-id="9d109-122">Name</span></span>       | <span data-ttu-id="9d109-123">Typ</span><span class="sxs-lookup"><span data-stu-id="9d109-123">Type</span></span> | <span data-ttu-id="9d109-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d109-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9d109-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d109-125">Authorization</span></span>  | <span data-ttu-id="9d109-126">string</span><span class="sxs-lookup"><span data-stu-id="9d109-126">string</span></span>  | <span data-ttu-id="9d109-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9d109-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d109-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d109-129">Request body</span></span>
<span data-ttu-id="9d109-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9d109-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d109-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d109-131">Response</span></span>

<span data-ttu-id="9d109-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [MailFolder](../resources/mailfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d109-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d109-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d109-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d109-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d109-134">Request</span></span>
<span data-ttu-id="9d109-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d109-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="9d109-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d109-136">Response</span></span>
<span data-ttu-id="9d109-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d109-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
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
