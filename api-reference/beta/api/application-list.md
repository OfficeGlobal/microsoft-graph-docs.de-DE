---
title: Liste applications
description: Abrufen der Liste der Programme in dieser Organisation.
author: lleonard-msft
ms.openlocfilehash: 138a9e6d238fde44d5b5c47781bbd93cb2b73f98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336694"
---
# <a name="list-applications"></a><span data-ttu-id="23a35-103">Liste applications</span><span class="sxs-lookup"><span data-stu-id="23a35-103">List applications</span></span>

> <span data-ttu-id="23a35-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23a35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23a35-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23a35-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23a35-106">Abrufen der Liste der Programme in dieser Organisation.</span><span class="sxs-lookup"><span data-stu-id="23a35-106">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="23a35-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="23a35-107">Permissions</span></span>
<span data-ttu-id="23a35-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23a35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="23a35-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23a35-110">Permission type</span></span>      | <span data-ttu-id="23a35-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23a35-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23a35-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23a35-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23a35-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23a35-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="23a35-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23a35-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23a35-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23a35-115">Not supported.</span></span>    |
|<span data-ttu-id="23a35-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23a35-116">Application</span></span> | <span data-ttu-id="23a35-117">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="23a35-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23a35-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23a35-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23a35-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="23a35-119">Optional query parameters</span></span>
<span data-ttu-id="23a35-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="23a35-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23a35-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23a35-121">Request headers</span></span>
| <span data-ttu-id="23a35-122">Name</span><span class="sxs-lookup"><span data-stu-id="23a35-122">Name</span></span>       | <span data-ttu-id="23a35-123">Typ</span><span class="sxs-lookup"><span data-stu-id="23a35-123">Type</span></span> | <span data-ttu-id="23a35-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23a35-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23a35-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="23a35-125">Authorization</span></span>  | <span data-ttu-id="23a35-126">string</span><span class="sxs-lookup"><span data-stu-id="23a35-126">string</span></span>  | <span data-ttu-id="23a35-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23a35-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="23a35-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23a35-129">Request body</span></span>
<span data-ttu-id="23a35-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="23a35-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23a35-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="23a35-131">Response</span></span>

<span data-ttu-id="23a35-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [Anwendung](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="23a35-132">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23a35-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23a35-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23a35-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23a35-134">Request</span></span>
<span data-ttu-id="23a35-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23a35-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications
```
##### <a name="response"></a><span data-ttu-id="23a35-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="23a35-136">Response</span></span>
<span data-ttu-id="23a35-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23a35-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
