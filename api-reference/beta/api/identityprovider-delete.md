---
title: IdentityProvider löschen
description: Löschen einer vorhandenen IdentityProvider.
ms.openlocfilehash: ac6f8cafa72b94891a540c05c2d4e5e2f32e23c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057976"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="b1bdf-103">IdentityProvider löschen</span><span class="sxs-lookup"><span data-stu-id="b1bdf-103">Delete identityProvider</span></span>

> <span data-ttu-id="b1bdf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1bdf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1bdf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1bdf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1bdf-106">Löschen einer vorhandenen [IdentityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="b1bdf-106">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b1bdf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b1bdf-107">Permissions</span></span>

<span data-ttu-id="b1bdf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1bdf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1bdf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1bdf-110">Permission type</span></span>      | <span data-ttu-id="b1bdf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1bdf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1bdf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1bdf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1bdf-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1bdf-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b1bdf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1bdf-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b1bdf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1bdf-115">Not supported.</span></span>|
|<span data-ttu-id="b1bdf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1bdf-116">Application</span></span>|<span data-ttu-id="b1bdf-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1bdf-117">Not supported.</span></span>|

<span data-ttu-id="b1bdf-118">Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="b1bdf-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="b1bdf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1bdf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b1bdf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1bdf-120">Request headers</span></span>

|<span data-ttu-id="b1bdf-121">Name</span><span class="sxs-lookup"><span data-stu-id="b1bdf-121">Name</span></span>|<span data-ttu-id="b1bdf-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1bdf-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b1bdf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1bdf-123">Authorization</span></span>|<span data-ttu-id="b1bdf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b1bdf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1bdf-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1bdf-126">Request body</span></span>

<span data-ttu-id="b1bdf-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b1bdf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1bdf-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1bdf-128">Response</span></span>

<span data-ttu-id="b1bdf-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1bdf-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1bdf-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1bdf-130">Example</span></span>

<span data-ttu-id="b1bdf-131">Im folgende Beispiel wird ein **IdentityProvider**gelöscht.</span><span class="sxs-lookup"><span data-stu-id="b1bdf-131">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="b1bdf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1bdf-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="b1bdf-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1bdf-133">Response</span></span>

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