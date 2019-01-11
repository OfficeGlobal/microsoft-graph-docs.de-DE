---
title: Liste identityProviders
description: Rufen Sie alle IdentityProviders im Verzeichnis ab.
localization_priority: Normal
ms.openlocfilehash: 43442a0bf354816c8c104d57d9720940d83bc0d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837967"
---
# <a name="list-identityproviders"></a><span data-ttu-id="9f700-103">Liste identityProviders</span><span class="sxs-lookup"><span data-stu-id="9f700-103">List identityProviders</span></span>

> <span data-ttu-id="9f700-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9f700-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f700-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f700-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f700-106">Rufen Sie alle [IdentityProviders](../resources/identityprovider.md) im Verzeichnis ab.</span><span class="sxs-lookup"><span data-stu-id="9f700-106">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f700-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f700-107">Permissions</span></span>

<span data-ttu-id="9f700-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f700-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f700-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f700-110">Permission type</span></span>      | <span data-ttu-id="9f700-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f700-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f700-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f700-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f700-113">IdentityProvider.Read.All IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f700-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="9f700-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f700-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9f700-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f700-115">Not supported.</span></span>|
|<span data-ttu-id="9f700-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f700-116">Application</span></span>|<span data-ttu-id="9f700-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f700-117">Not supported.</span></span>|

<span data-ttu-id="9f700-118">Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="9f700-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f700-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f700-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="9f700-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f700-120">Request headers</span></span>

|<span data-ttu-id="9f700-121">Name</span><span class="sxs-lookup"><span data-stu-id="9f700-121">Name</span></span>|<span data-ttu-id="9f700-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f700-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9f700-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f700-123">Authorization</span></span>|<span data-ttu-id="9f700-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f700-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f700-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f700-126">Request body</span></span>

<span data-ttu-id="9f700-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9f700-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f700-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f700-128">Response</span></span>

<span data-ttu-id="9f700-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und eine Auflistung von [IdentityProviders](../resources/identityprovider.md) im JSON-Darstellung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9f700-129">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f700-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f700-130">Example</span></span>

<span data-ttu-id="9f700-131">Im folgende Beispiel werden alle **IdentityProvider**abgerufen.</span><span class="sxs-lookup"><span data-stu-id="9f700-131">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="9f700-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f700-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="9f700-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f700-133">Response</span></span>

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
