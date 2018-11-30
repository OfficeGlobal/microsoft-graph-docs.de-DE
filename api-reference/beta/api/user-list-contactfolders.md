---
title: contactFolders auflisten
description: Rufen Sie die Kontakt Ordner im Postfach des angemeldeten Benutzers.
ms.openlocfilehash: 08f763d8bc1e9a05c047f194e2847d76c385e587
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062220"
---
# <a name="list-contactfolders"></a><span data-ttu-id="e2e2f-103">contactFolders auflisten</span><span class="sxs-lookup"><span data-stu-id="e2e2f-103">List contactFolders</span></span>

> <span data-ttu-id="e2e2f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e2e2f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2e2f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2e2f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2e2f-106">Rufen Sie die Kontakt Ordner im Postfach des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e2e2f-106">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2e2f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e2e2f-107">Permissions</span></span>
<span data-ttu-id="e2e2f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2e2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2e2f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2e2f-110">Permission type</span></span>      | <span data-ttu-id="e2e2f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2e2f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2e2f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2e2f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e2e2f-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2e2f-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e2e2f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2e2f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2e2f-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2e2f-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e2e2f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2e2f-116">Application</span></span> | <span data-ttu-id="e2e2f-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2e2f-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2e2f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2e2f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2e2f-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e2e2f-119">Optional query parameters</span></span>
<span data-ttu-id="e2e2f-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e2e2f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e2e2f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2e2f-121">Request headers</span></span>
| <span data-ttu-id="e2e2f-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e2e2f-122">Header</span></span>       | <span data-ttu-id="e2e2f-123">Wert</span><span class="sxs-lookup"><span data-stu-id="e2e2f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e2e2f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2e2f-124">Authorization</span></span>  | <span data-ttu-id="e2e2f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e2e2f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e2e2f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2e2f-127">Content-Type</span></span>   | <span data-ttu-id="e2e2f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e2e2f-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e2e2f-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2e2f-129">Request body</span></span>
<span data-ttu-id="e2e2f-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e2e2f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2e2f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2e2f-131">Response</span></span>

<span data-ttu-id="e2e2f-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ContactFolder](../resources/contactfolder.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2e2f-132">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2e2f-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2e2f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2e2f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2e2f-134">Request</span></span>
<span data-ttu-id="e2e2f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2e2f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="e2e2f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2e2f-136">Response</span></span>
<span data-ttu-id="e2e2f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2e2f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
