---
title: Liste identityProviders
description: Rufen Sie alle IdentityProviders im Verzeichnis ab.
ms.openlocfilehash: fd5662690b644bc7a34587a5bdfc519188a3d4ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064287"
---
# <a name="list-identityproviders"></a><span data-ttu-id="5b1bd-103">Liste identityProviders</span><span class="sxs-lookup"><span data-stu-id="5b1bd-103">List identityProviders</span></span>

> <span data-ttu-id="5b1bd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b1bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b1bd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b1bd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b1bd-106">Rufen Sie alle [IdentityProviders](../resources/identityprovider.md) im Verzeichnis ab.</span><span class="sxs-lookup"><span data-stu-id="5b1bd-106">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b1bd-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5b1bd-107">Permissions</span></span>

<span data-ttu-id="5b1bd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b1bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b1bd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b1bd-110">Permission type</span></span>      | <span data-ttu-id="5b1bd-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b1bd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b1bd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b1bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b1bd-113">IdentityProvider.Read.All IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b1bd-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="5b1bd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b1bd-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5b1bd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b1bd-115">Not supported.</span></span>|
|<span data-ttu-id="5b1bd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b1bd-116">Application</span></span>|<span data-ttu-id="5b1bd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b1bd-117">Not supported.</span></span>|

<span data-ttu-id="5b1bd-118">Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="5b1bd-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="5b1bd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b1bd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="5b1bd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b1bd-120">Request headers</span></span>

|<span data-ttu-id="5b1bd-121">Name</span><span class="sxs-lookup"><span data-stu-id="5b1bd-121">Name</span></span>|<span data-ttu-id="5b1bd-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b1bd-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5b1bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b1bd-123">Authorization</span></span>|<span data-ttu-id="5b1bd-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b1bd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b1bd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b1bd-126">Request body</span></span>

<span data-ttu-id="5b1bd-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5b1bd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b1bd-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b1bd-128">Response</span></span>

<span data-ttu-id="5b1bd-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eine Auflistung von [IdentityProviders](../resources/identityprovider.md) im JSON-Darstellung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5b1bd-129">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b1bd-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b1bd-130">Example</span></span>

<span data-ttu-id="5b1bd-131">Im folgende Beispiel werden alle **IdentityProvider**abgerufen.</span><span class="sxs-lookup"><span data-stu-id="5b1bd-131">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="5b1bd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b1bd-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="5b1bd-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b1bd-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->