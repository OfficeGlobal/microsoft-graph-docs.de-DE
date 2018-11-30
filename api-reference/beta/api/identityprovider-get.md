---
title: Abrufen von identityProvider
description: Abrufen der Eigenschaften einer vorhandenen IdentityProvider.
ms.openlocfilehash: 238e222c820e62685fa7c9e7ca50f5efb33693cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061154"
---
# <a name="get-identityprovider"></a><span data-ttu-id="2abe0-103">Abrufen von identityProvider</span><span class="sxs-lookup"><span data-stu-id="2abe0-103">Get identityProvider</span></span>

> <span data-ttu-id="2abe0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2abe0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2abe0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2abe0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2abe0-106">Abrufen der Eigenschaften einer vorhandenen [IdentityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="2abe0-106">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2abe0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2abe0-107">Permissions</span></span>

<span data-ttu-id="2abe0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2abe0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2abe0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2abe0-110">Permission type</span></span>      | <span data-ttu-id="2abe0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2abe0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2abe0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2abe0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2abe0-113">IdentityProvider.Read.All IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2abe0-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="2abe0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2abe0-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="2abe0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2abe0-115">Not supported.</span></span>|
|<span data-ttu-id="2abe0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2abe0-116">Application</span></span>|<span data-ttu-id="2abe0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2abe0-117">Not supported.</span></span>|

<span data-ttu-id="2abe0-118">Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="2abe0-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="2abe0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2abe0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2abe0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2abe0-120">Request headers</span></span>

|<span data-ttu-id="2abe0-121">Name</span><span class="sxs-lookup"><span data-stu-id="2abe0-121">Name</span></span>|<span data-ttu-id="2abe0-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2abe0-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="2abe0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2abe0-123">Authorization</span></span>|<span data-ttu-id="2abe0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2abe0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2abe0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2abe0-126">Request body</span></span>

<span data-ttu-id="2abe0-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2abe0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2abe0-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2abe0-128">Response</span></span>

<span data-ttu-id="2abe0-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eine JSON-Darstellung der [IdentityProvider](../resources/identityprovider.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2abe0-129">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2abe0-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2abe0-130">Example</span></span>

<span data-ttu-id="2abe0-131">Im folgende Beispiel werden einer bestimmten **IdentityProvider**abgerufen.</span><span class="sxs-lookup"><span data-stu-id="2abe0-131">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="2abe0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2abe0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="2abe0-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2abe0-133">Response</span></span>

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