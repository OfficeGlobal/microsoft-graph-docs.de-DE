---
title: Abrufen eines Identitätsanbieters
description: Abrufen der Eigenschaften eines vorhandenen Identitätsanbieters.
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc06d4f8dcab8bf07d2dc0a9ff8130b305b8217c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649409"
---
# <a name="get-identityprovider"></a><span data-ttu-id="e05fa-103">Abrufen eines Identitätsanbieters</span><span class="sxs-lookup"><span data-stu-id="e05fa-103">Get identityProvider</span></span>

<span data-ttu-id="e05fa-104">Abrufen der Eigenschaften eines vorhandenen [Identitätsanbieters](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="e05fa-104">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e05fa-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e05fa-105">Permissions</span></span>

<span data-ttu-id="e05fa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e05fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e05fa-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e05fa-108">Permission type</span></span>      | <span data-ttu-id="e05fa-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e05fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e05fa-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e05fa-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e05fa-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e05fa-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e05fa-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e05fa-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e05fa-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e05fa-113">Not supported.</span></span>|
|<span data-ttu-id="e05fa-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e05fa-114">Application</span></span>|<span data-ttu-id="e05fa-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e05fa-115">Not supported.</span></span>|

<span data-ttu-id="e05fa-116">Das Geschäfts-, Schul- oder Unikonto muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="e05fa-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e05fa-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e05fa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e05fa-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e05fa-118">Request headers</span></span>

|<span data-ttu-id="e05fa-119">Name</span><span class="sxs-lookup"><span data-stu-id="e05fa-119">Name</span></span>|<span data-ttu-id="e05fa-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e05fa-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e05fa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e05fa-121">Authorization</span></span>|<span data-ttu-id="e05fa-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e05fa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e05fa-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e05fa-124">Request body</span></span>

<span data-ttu-id="e05fa-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e05fa-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e05fa-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="e05fa-126">Response</span></span>

<span data-ttu-id="e05fa-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine JSON-Darstellung des [Identitätsanbieters](../resources/identityProvider.md) im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e05fa-127">If successful, this method returns a `200 OK` response code and collection of [workbookPivotTable](../resources/identityProvider.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e05fa-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e05fa-128">Example</span></span>

<span data-ttu-id="e05fa-129">Im folgenden Beispiel wird ein bestimmter **Identitätsanbieter** abgerufen.</span><span class="sxs-lookup"><span data-stu-id="e05fa-129">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e05fa-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e05fa-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-identityprovider"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="e05fa-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e05fa-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
