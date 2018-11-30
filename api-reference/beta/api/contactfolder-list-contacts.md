---
title: Kontakte auflisten
description: Rufen Sie alle Kontakte im Postfach des angemeldeten Benutzers (.../me/contacts) oder aus der angegebenen Kontaktordner.
ms.openlocfilehash: e15080c9a4d5b0f8e388cc9556ded1ac90ce2823
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059637"
---
# <a name="list-contacts"></a><span data-ttu-id="18afd-103">Kontakte auflisten</span><span class="sxs-lookup"><span data-stu-id="18afd-103">List contacts</span></span>

> <span data-ttu-id="18afd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="18afd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18afd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18afd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18afd-106">Rufen Sie alle Kontakte im Postfach des angemeldeten Benutzers (.../me/contacts) oder aus der angegebenen Kontaktordner.</span><span class="sxs-lookup"><span data-stu-id="18afd-106">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="18afd-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="18afd-107">Permissions</span></span>
<span data-ttu-id="18afd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18afd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18afd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="18afd-110">Permission type</span></span>      | <span data-ttu-id="18afd-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="18afd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18afd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="18afd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18afd-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18afd-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="18afd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="18afd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18afd-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18afd-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="18afd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="18afd-116">Application</span></span> | <span data-ttu-id="18afd-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18afd-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="18afd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="18afd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="18afd-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="18afd-119">Optional query parameters</span></span>
<span data-ttu-id="18afd-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="18afd-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="18afd-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="18afd-121">Request headers</span></span>
| <span data-ttu-id="18afd-122">Name</span><span class="sxs-lookup"><span data-stu-id="18afd-122">Name</span></span>       | <span data-ttu-id="18afd-123">Typ</span><span class="sxs-lookup"><span data-stu-id="18afd-123">Type</span></span> | <span data-ttu-id="18afd-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18afd-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="18afd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="18afd-125">Authorization</span></span>  | <span data-ttu-id="18afd-126">string</span><span class="sxs-lookup"><span data-stu-id="18afd-126">string</span></span>  | <span data-ttu-id="18afd-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="18afd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18afd-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="18afd-129">Request body</span></span>
<span data-ttu-id="18afd-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="18afd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18afd-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="18afd-131">Response</span></span>

<span data-ttu-id="18afd-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contact](../resources/contact.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18afd-132">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18afd-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="18afd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18afd-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="18afd-134">Request</span></span>
<span data-ttu-id="18afd-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="18afd-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="18afd-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="18afd-136">Response</span></span>
<span data-ttu-id="18afd-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="18afd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
