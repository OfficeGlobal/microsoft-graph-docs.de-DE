---
title: IdentityProvider löschen
description: Löschen einer vorhandenen IdentityProvider.
localization_priority: Normal
ms.openlocfilehash: 35689037d4f6a564ee3e1e40d18401ef793ef474
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808295"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="874d4-103">IdentityProvider löschen</span><span class="sxs-lookup"><span data-stu-id="874d4-103">Delete identityProvider</span></span>

> <span data-ttu-id="874d4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="874d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="874d4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="874d4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="874d4-106">Löschen einer vorhandenen [IdentityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="874d4-106">Delete an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="874d4-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="874d4-107">Permissions</span></span>

<span data-ttu-id="874d4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="874d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="874d4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="874d4-110">Permission type</span></span>      | <span data-ttu-id="874d4-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="874d4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="874d4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="874d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="874d4-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="874d4-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="874d4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="874d4-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="874d4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="874d4-115">Not supported.</span></span>|
|<span data-ttu-id="874d4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="874d4-116">Application</span></span>|<span data-ttu-id="874d4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="874d4-117">Not supported.</span></span>|

<span data-ttu-id="874d4-118">Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="874d4-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="874d4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="874d4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="874d4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="874d4-120">Request headers</span></span>

|<span data-ttu-id="874d4-121">Name</span><span class="sxs-lookup"><span data-stu-id="874d4-121">Name</span></span>|<span data-ttu-id="874d4-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="874d4-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="874d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="874d4-123">Authorization</span></span>|<span data-ttu-id="874d4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="874d4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="874d4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="874d4-126">Request body</span></span>

<span data-ttu-id="874d4-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="874d4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="874d4-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="874d4-128">Response</span></span>

<span data-ttu-id="874d4-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="874d4-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="874d4-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="874d4-130">Example</span></span>

<span data-ttu-id="874d4-131">Im folgende Beispiel wird ein **IdentityProvider**gelöscht.</span><span class="sxs-lookup"><span data-stu-id="874d4-131">The following example deletes an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="874d4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="874d4-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="874d4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="874d4-133">Response</span></span>

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
