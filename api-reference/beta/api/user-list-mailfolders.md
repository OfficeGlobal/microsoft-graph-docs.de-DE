---
title: mailFolders auflisten
description: Rufen Sie die e-Mail-Ordner im Postfach des angemeldeten Benutzers.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cb2d9e50776d88676cd6c2fdde39d9de89a635c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990299"
---
# <a name="list-mailfolders"></a><span data-ttu-id="afe24-103">mailFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="afe24-103">List mailFolders</span></span>

> <span data-ttu-id="afe24-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="afe24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afe24-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="afe24-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="afe24-106">Rufen Sie die e-Mail-Ordner im Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="afe24-106">Get all the mail folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="afe24-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="afe24-107">Permissions</span></span>
<span data-ttu-id="afe24-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afe24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afe24-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="afe24-110">Permission type</span></span>      | <span data-ttu-id="afe24-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="afe24-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afe24-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="afe24-112">Delegated (work or school account)</span></span> | <span data-ttu-id="afe24-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="afe24-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="afe24-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="afe24-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afe24-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="afe24-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="afe24-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="afe24-116">Application</span></span> | <span data-ttu-id="afe24-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="afe24-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="afe24-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="afe24-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="afe24-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="afe24-119">Optional query parameters</span></span>
<span data-ttu-id="afe24-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="afe24-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="afe24-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="afe24-121">Request headers</span></span>
| <span data-ttu-id="afe24-122">Header</span><span class="sxs-lookup"><span data-stu-id="afe24-122">Header</span></span>       | <span data-ttu-id="afe24-123">Wert</span><span class="sxs-lookup"><span data-stu-id="afe24-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="afe24-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="afe24-124">Authorization</span></span>  | <span data-ttu-id="afe24-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="afe24-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="afe24-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="afe24-127">Content-Type</span></span>   | <span data-ttu-id="afe24-128">application/json</span><span class="sxs-lookup"><span data-stu-id="afe24-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="afe24-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="afe24-129">Request body</span></span>
<span data-ttu-id="afe24-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="afe24-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afe24-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="afe24-131">Response</span></span>

<span data-ttu-id="afe24-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [MailFolder](../resources/mailfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afe24-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="afe24-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="afe24-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="afe24-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="afe24-134">Request</span></span>
<span data-ttu-id="afe24-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="afe24-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="afe24-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="afe24-136">Response</span></span>
<span data-ttu-id="afe24-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="afe24-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
