---
title: Kontakte auflisten
description: Dient zum Abrufen einer Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers (`.../me/contacts`) oder aus dem angegebenen Kontaktordner.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bc7cc37eaefbd84e9fea8d4cbb1e888b5c445d1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912477"
---
# <a name="list-contacts"></a><span data-ttu-id="9806b-103">Kontakte auflisten</span><span class="sxs-lookup"><span data-stu-id="9806b-103">List contacts</span></span>

<span data-ttu-id="9806b-104">Mit dieser API können Sie eine Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers (`.../me/contacts`) oder dem jeweils angegebenen Kontaktordner abrufen.</span><span class="sxs-lookup"><span data-stu-id="9806b-104">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="9806b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9806b-105">Permissions</span></span>
<span data-ttu-id="9806b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9806b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9806b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9806b-108">Permission type</span></span>      | <span data-ttu-id="9806b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9806b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9806b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9806b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9806b-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9806b-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9806b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9806b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9806b-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9806b-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9806b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9806b-114">Application</span></span> | <span data-ttu-id="9806b-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9806b-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9806b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9806b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9806b-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9806b-117">Optional query parameters</span></span>
<span data-ttu-id="9806b-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9806b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9806b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9806b-119">Request headers</span></span>
| <span data-ttu-id="9806b-120">Name</span><span class="sxs-lookup"><span data-stu-id="9806b-120">Name</span></span>       | <span data-ttu-id="9806b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9806b-121">Type</span></span> | <span data-ttu-id="9806b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9806b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9806b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9806b-123">Authorization</span></span>  | <span data-ttu-id="9806b-124">string</span><span class="sxs-lookup"><span data-stu-id="9806b-124">string</span></span>  | <span data-ttu-id="9806b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9806b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9806b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9806b-127">Request body</span></span>
<span data-ttu-id="9806b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9806b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9806b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9806b-129">Response</span></span>

<span data-ttu-id="9806b-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contact](../resources/contact.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9806b-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9806b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9806b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9806b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9806b-132">Request</span></span>
<span data-ttu-id="9806b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9806b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="9806b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9806b-134">Response</span></span>
<span data-ttu-id="9806b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9806b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "birthday": "datetime-value",
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
