---
title: 'OrgContact: Get-Manager'
description: Abrufen der Vorgesetzte des Kontakts
ms.openlocfilehash: 7fe4c61422eb83bb4501fbb521f301ec6f9afaa5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059297"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="8513e-103">OrgContact: Get-Manager</span><span class="sxs-lookup"><span data-stu-id="8513e-103">orgContact: Get manager</span></span>

> <span data-ttu-id="8513e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8513e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8513e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8513e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8513e-106">Abrufen der Vorgesetzte des Kontakts</span><span class="sxs-lookup"><span data-stu-id="8513e-106">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="8513e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8513e-107">Permissions</span></span>
<span data-ttu-id="8513e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8513e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8513e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8513e-110">Permission type</span></span>      | <span data-ttu-id="8513e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8513e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8513e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8513e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8513e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8513e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8513e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8513e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8513e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8513e-115">Not supported.</span></span>    |
|<span data-ttu-id="8513e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8513e-116">Application</span></span> | <span data-ttu-id="8513e-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8513e-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8513e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8513e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8513e-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8513e-119">Optional query parameters</span></span>
<span data-ttu-id="8513e-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8513e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8513e-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8513e-121">Request headers</span></span>
| <span data-ttu-id="8513e-122">Name</span><span class="sxs-lookup"><span data-stu-id="8513e-122">Name</span></span>       | <span data-ttu-id="8513e-123">Typ</span><span class="sxs-lookup"><span data-stu-id="8513e-123">Type</span></span> | <span data-ttu-id="8513e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8513e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8513e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8513e-125">Authorization</span></span>  | <span data-ttu-id="8513e-126">string</span><span class="sxs-lookup"><span data-stu-id="8513e-126">string</span></span>  | <span data-ttu-id="8513e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8513e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8513e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8513e-129">Request body</span></span>
<span data-ttu-id="8513e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8513e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8513e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="8513e-131">Response</span></span>

<span data-ttu-id="8513e-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8513e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8513e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8513e-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8513e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8513e-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="8513e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="8513e-135">Response</span></span>

<span data-ttu-id="8513e-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8513e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
    "businessPhones": [
        "+1 205 555 0108"
    ],
    "displayName": "Diego Siciliani",
    "givenName": "Diego",
    "jobTitle": "CVP Finance",
    "mail": "DiegoS@contoso.com",
    "mobilePhone": null,
    "officeLocation": "14/1108",
    "preferredLanguage": "en-US",
    "surname": "Siciliani",
    "userPrincipalName": "DiegoS@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->