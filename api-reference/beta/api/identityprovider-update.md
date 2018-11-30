---
title: IdentityProvider aktualisieren
description: Aktualisieren von Eigenschaften in einer vorhandenen IdentityProvider.
ms.openlocfilehash: b89b0f50ef2f62625a1707c3e77c32865adaec67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060841"
---
# <a name="update-identityprovider"></a><span data-ttu-id="49da2-103">IdentityProvider aktualisieren</span><span class="sxs-lookup"><span data-stu-id="49da2-103">Update identityProvider</span></span>

> <span data-ttu-id="49da2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="49da2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49da2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49da2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49da2-106">Aktualisieren von Eigenschaften in einer vorhandenen [IdentityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="49da2-106">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="49da2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="49da2-107">Permissions</span></span>

<span data-ttu-id="49da2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49da2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49da2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49da2-110">Permission type</span></span>      | <span data-ttu-id="49da2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49da2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49da2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49da2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49da2-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49da2-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="49da2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49da2-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="49da2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49da2-115">Not supported.</span></span>|
|<span data-ttu-id="49da2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49da2-116">Application</span></span>|<span data-ttu-id="49da2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49da2-117">Not supported.</span></span>|

<span data-ttu-id="49da2-118">Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="49da2-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="49da2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49da2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="49da2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49da2-120">Request headers</span></span>

|<span data-ttu-id="49da2-121">Name</span><span class="sxs-lookup"><span data-stu-id="49da2-121">Name</span></span>|<span data-ttu-id="49da2-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49da2-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="49da2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49da2-123">Authorization</span></span>|<span data-ttu-id="49da2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49da2-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="49da2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49da2-126">Content-Type</span></span>|<span data-ttu-id="49da2-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="49da2-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49da2-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49da2-129">Request body</span></span>

<span data-ttu-id="49da2-130">Geben Sie im Textkörper Anforderung ein JSON-Objekt mit einer oder mehrerer Eigenschaften, die aktualisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="49da2-130">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="49da2-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49da2-131">Property</span></span>|<span data-ttu-id="49da2-132">Typ</span><span class="sxs-lookup"><span data-stu-id="49da2-132">Type</span></span>|<span data-ttu-id="49da2-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49da2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49da2-134">clientId</span><span class="sxs-lookup"><span data-stu-id="49da2-134">clientId</span></span>|<span data-ttu-id="49da2-135">String</span><span class="sxs-lookup"><span data-stu-id="49da2-135">String</span></span>|<span data-ttu-id="49da2-136">Die Client-ID für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="49da2-136">The client ID for the application.</span></span> <span data-ttu-id="49da2-137">Dies ist die Client-ID abgerufen wird, wenn die Anwendung mit dem Identitätsanbieter registrieren.</span><span class="sxs-lookup"><span data-stu-id="49da2-137">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="49da2-138">clientSecret</span><span class="sxs-lookup"><span data-stu-id="49da2-138">clientSecret</span></span>|<span data-ttu-id="49da2-139">String</span><span class="sxs-lookup"><span data-stu-id="49da2-139">String</span></span>|<span data-ttu-id="49da2-140">Der geheime Clientschlüssel für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="49da2-140">The client secret for the application.</span></span> <span data-ttu-id="49da2-141">Dies ist der geheime Clientschlüssel erhalten Sie, wenn die Anwendung mit dem Identitätsanbieter registrieren.</span><span class="sxs-lookup"><span data-stu-id="49da2-141">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="49da2-142">name</span><span class="sxs-lookup"><span data-stu-id="49da2-142">name</span></span>|<span data-ttu-id="49da2-143">String</span><span class="sxs-lookup"><span data-stu-id="49da2-143">String</span></span>|<span data-ttu-id="49da2-144">Der Anzeigename des Identitätsanbieters.</span><span class="sxs-lookup"><span data-stu-id="49da2-144">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="49da2-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="49da2-145">Response</span></span>

<span data-ttu-id="49da2-146">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49da2-146">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="49da2-147">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49da2-147">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="49da2-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49da2-148">Example</span></span>

<span data-ttu-id="49da2-149">Im folgenden Beispiel wird die Definition der Gültigkeitsdauer von token **IdentityProvider** aktualisiert und platziert es als Standard Organisation.</span><span class="sxs-lookup"><span data-stu-id="49da2-149">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="49da2-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49da2-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```

##### <a name="response"></a><span data-ttu-id="49da2-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="49da2-151">Response</span></span>

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