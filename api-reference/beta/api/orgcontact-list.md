---
title: Liste orgContacts
description: Die Liste der Organisationseinheit Kontakte für diese Organisation abgerufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 53cfa75edeb1994cabc1f363dab79455b90ce921
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915074"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="b6b37-103">Liste orgContacts</span><span class="sxs-lookup"><span data-stu-id="b6b37-103">List orgContacts</span></span>

> <span data-ttu-id="b6b37-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b6b37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6b37-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6b37-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6b37-106">Die Liste der Organisationseinheit Kontakte für diese Organisation abgerufen.</span><span class="sxs-lookup"><span data-stu-id="b6b37-106">Retrieve the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6b37-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b6b37-107">Permissions</span></span>
<span data-ttu-id="b6b37-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6b37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6b37-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6b37-110">Permission type</span></span>      | <span data-ttu-id="b6b37-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6b37-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6b37-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6b37-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b6b37-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6b37-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b6b37-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6b37-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6b37-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6b37-115">Not supported.</span></span>    |
|<span data-ttu-id="b6b37-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6b37-116">Application</span></span> | <span data-ttu-id="b6b37-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6b37-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6b37-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6b37-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6b37-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b6b37-119">Optional query parameters</span></span>
<span data-ttu-id="b6b37-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b6b37-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6b37-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6b37-121">Request headers</span></span>
| <span data-ttu-id="b6b37-122">Name</span><span class="sxs-lookup"><span data-stu-id="b6b37-122">Name</span></span>       | <span data-ttu-id="b6b37-123">Typ</span><span class="sxs-lookup"><span data-stu-id="b6b37-123">Type</span></span> | <span data-ttu-id="b6b37-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6b37-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b6b37-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6b37-125">Authorization</span></span>  | <span data-ttu-id="b6b37-126">string</span><span class="sxs-lookup"><span data-stu-id="b6b37-126">string</span></span>  | <span data-ttu-id="b6b37-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b6b37-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6b37-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b6b37-129">Request body</span></span>
<span data-ttu-id="b6b37-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b6b37-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6b37-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6b37-131">Response</span></span>

<span data-ttu-id="b6b37-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [OrgContact](../resources/orgcontact.md) .</span><span class="sxs-lookup"><span data-stu-id="b6b37-132">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6b37-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b6b37-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6b37-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6b37-134">Request</span></span>
<span data-ttu-id="b6b37-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b6b37-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts
```
##### <a name="response"></a><span data-ttu-id="b6b37-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6b37-136">Response</span></span>
<span data-ttu-id="b6b37-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6b37-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
    {
      "addresses":[
          {
            "city": "string",
            "countryOrRegion": "string",
            "officeLocation": "string",
            "postalCode": "string",
            "state": "string",
            "street": "string"
          }
      ],
      "companyName": "companyName-value",
      "department": "department-value",
      "displayName": "displayName-value",
      "phones":[
          {
            "type": "string",
            "number": "string"
          }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
