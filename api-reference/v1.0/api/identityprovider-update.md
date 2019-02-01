---
title: Aktualisieren eines Identitätsanbieters
description: Aktualisieren der Eigenschaften eines vorhandenen Identitätsanbieters.
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b3b945163946586e17e16372523a3349306f77ec
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649404"
---
# <a name="update-identityprovider"></a><span data-ttu-id="e030c-103">Aktualisieren eines Identitätsanbieters</span><span class="sxs-lookup"><span data-stu-id="e030c-103">Update identityProvider</span></span>

<span data-ttu-id="e030c-104">Aktualisieren der Eigenschaften eines vorhandenen [Identitätsanbieters](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="e030c-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e030c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e030c-105">Permissions</span></span>

<span data-ttu-id="e030c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e030c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e030c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e030c-108">Permission type</span></span>      | <span data-ttu-id="e030c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e030c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e030c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e030c-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e030c-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e030c-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e030c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e030c-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e030c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e030c-113">Not supported.</span></span>|
|<span data-ttu-id="e030c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e030c-114">Application</span></span>|<span data-ttu-id="e030c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e030c-115">Not supported.</span></span>|

<span data-ttu-id="e030c-116">Das Geschäfts-, Schul- oder Unikonto muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="e030c-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e030c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e030c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e030c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e030c-118">Request headers</span></span>

|<span data-ttu-id="e030c-119">Name</span><span class="sxs-lookup"><span data-stu-id="e030c-119">Name</span></span>|<span data-ttu-id="e030c-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e030c-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e030c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e030c-121">Authorization</span></span>|<span data-ttu-id="e030c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e030c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e030c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e030c-124">Content-Type</span></span>|<span data-ttu-id="e030c-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e030c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e030c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e030c-127">Request body</span></span>

<span data-ttu-id="e030c-128">Geben Sie im Anforderungstext ein JSON-Objekt mit einer oder mehreren Eigenschaften an, die aktualisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="e030c-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="e030c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e030c-129">Property</span></span>|<span data-ttu-id="e030c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e030c-130">Type</span></span>|<span data-ttu-id="e030c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e030c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e030c-132">clientId</span><span class="sxs-lookup"><span data-stu-id="e030c-132">clientId</span></span>|<span data-ttu-id="e030c-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e030c-133">String</span></span>|<span data-ttu-id="e030c-134">Die Client-ID für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="e030c-134">The client ID created for your application.</span></span> <span data-ttu-id="e030c-135">Dies ist die Client-ID, die Sie beim Registrieren der Anwendung beim Identitätsanbieter erhalten.</span><span class="sxs-lookup"><span data-stu-id="e030c-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="e030c-136">clientSecret</span><span class="sxs-lookup"><span data-stu-id="e030c-136">client_secret</span></span>|<span data-ttu-id="e030c-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e030c-137">String</span></span>|<span data-ttu-id="e030c-138">Der geheime Clientschlüssel für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="e030c-138">The client secret created for your application.</span></span> <span data-ttu-id="e030c-139">Dies ist der geheime Clientschlüssel, den Sie beim Registrieren der Anwendung beim Identitätsanbieter erhalten.</span><span class="sxs-lookup"><span data-stu-id="e030c-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="e030c-140">name</span><span class="sxs-lookup"><span data-stu-id="e030c-140">name</span></span>|<span data-ttu-id="e030c-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e030c-141">String</span></span>|<span data-ttu-id="e030c-142">Der Anzeigename des Identitätsanbieters.</span><span class="sxs-lookup"><span data-stu-id="e030c-142">The unique name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="e030c-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="e030c-143">Response</span></span>

<span data-ttu-id="e030c-144">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e030c-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="e030c-145">Wenn die Methode nicht erfolgreich ist, wird ein `4xx`-Fehler mit bestimmten Details zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e030c-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="e030c-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e030c-146">Example</span></span>

<span data-ttu-id="e030c-147">Im folgenden Beispiel wird die Definition der Tokengültigkeitsdauer von **identityProvider** aktualisiert und als Standard in der Organisation festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e030c-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="e030c-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e030c-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update-identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```

##### <a name="response"></a><span data-ttu-id="e030c-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="e030c-149">Response</span></span>

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
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
