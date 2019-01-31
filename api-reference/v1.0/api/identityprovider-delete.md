---
title: Löschen eines Identitätsanbieters
description: Löschen eines vorhandenen Identitätsanbieters.
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a09018011e87da383371ba41b1a046ddeb9002b5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649407"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="8dd18-103">Löschen eines Identitätsanbieters</span><span class="sxs-lookup"><span data-stu-id="8dd18-103">Delete identityProvider</span></span>

<span data-ttu-id="8dd18-104">Löschen eines vorhandenen [Identitätsanbieters](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="8dd18-104">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8dd18-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8dd18-105">Permissions</span></span>

<span data-ttu-id="8dd18-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dd18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dd18-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8dd18-108">Permission type</span></span>      | <span data-ttu-id="8dd18-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8dd18-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dd18-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8dd18-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8dd18-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd18-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="8dd18-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8dd18-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8dd18-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8dd18-113">Not supported.</span></span>|
|<span data-ttu-id="8dd18-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8dd18-114">Application</span></span>|<span data-ttu-id="8dd18-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8dd18-115">Not supported.</span></span>|

<span data-ttu-id="8dd18-116">Das Geschäfts-, Schul- oder Unikonto muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="8dd18-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="8dd18-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8dd18-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8dd18-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8dd18-118">Request headers</span></span>

|<span data-ttu-id="8dd18-119">Name</span><span class="sxs-lookup"><span data-stu-id="8dd18-119">Name</span></span>|<span data-ttu-id="8dd18-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8dd18-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8dd18-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dd18-121">Authorization</span></span>|<span data-ttu-id="8dd18-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8dd18-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dd18-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8dd18-124">Request body</span></span>

<span data-ttu-id="8dd18-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8dd18-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dd18-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="8dd18-126">Response</span></span>

<span data-ttu-id="8dd18-127">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8dd18-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8dd18-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8dd18-128">Example</span></span>

<span data-ttu-id="8dd18-129">Im folgenden Beispiel wird ein **Identitätsanbieter** gelöscht.</span><span class="sxs-lookup"><span data-stu-id="8dd18-129">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="8dd18-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8dd18-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="8dd18-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="8dd18-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
