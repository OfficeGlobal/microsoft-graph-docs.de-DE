---
title: 'OrgContact: Get-Manager'
description: Abrufen der Vorgesetzte des Kontakts
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96833e9b38b2d988a3843e097a11fe38a247c0b6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524856"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="f4e79-103">OrgContact: Get-Manager</span><span class="sxs-lookup"><span data-stu-id="f4e79-103">orgContact: Get manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4e79-104">Abrufen der Vorgesetzte des Kontakts</span><span class="sxs-lookup"><span data-stu-id="f4e79-104">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="f4e79-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f4e79-105">Permissions</span></span>
<span data-ttu-id="f4e79-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4e79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4e79-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f4e79-108">Permission type</span></span>      | <span data-ttu-id="f4e79-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f4e79-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4e79-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f4e79-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f4e79-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4e79-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f4e79-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f4e79-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4e79-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f4e79-113">Not supported.</span></span>    |
|<span data-ttu-id="f4e79-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f4e79-114">Application</span></span> | <span data-ttu-id="f4e79-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4e79-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4e79-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4e79-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4e79-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f4e79-117">Optional query parameters</span></span>
<span data-ttu-id="f4e79-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f4e79-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4e79-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f4e79-119">Request headers</span></span>
| <span data-ttu-id="f4e79-120">Name</span><span class="sxs-lookup"><span data-stu-id="f4e79-120">Name</span></span>       | <span data-ttu-id="f4e79-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f4e79-121">Type</span></span> | <span data-ttu-id="f4e79-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4e79-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f4e79-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4e79-123">Authorization</span></span>  | <span data-ttu-id="f4e79-124">string</span><span class="sxs-lookup"><span data-stu-id="f4e79-124">string</span></span>  | <span data-ttu-id="f4e79-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f4e79-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4e79-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f4e79-127">Request body</span></span>
<span data-ttu-id="f4e79-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f4e79-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4e79-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4e79-129">Response</span></span>

<span data-ttu-id="f4e79-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4e79-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f4e79-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f4e79-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f4e79-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f4e79-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="f4e79-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f4e79-133">Response</span></span>

<span data-ttu-id="f4e79-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f4e79-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-get-manager.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
