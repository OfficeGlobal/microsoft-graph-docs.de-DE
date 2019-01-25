---
title: IdentityProvider aktualisieren
description: Aktualisieren von Eigenschaften in einer vorhandenen IdentityProvider.
localization_priority: Normal
ms.openlocfilehash: d98bc5d0bd7a8f165f33c89548a69805039cdf07
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525745"
---
# <a name="update-identityprovider"></a><span data-ttu-id="49326-103">IdentityProvider aktualisieren</span><span class="sxs-lookup"><span data-stu-id="49326-103">Update identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49326-104">Aktualisieren von Eigenschaften in einer vorhandenen [IdentityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="49326-104">Update properties in an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="49326-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="49326-105">Permissions</span></span>

<span data-ttu-id="49326-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49326-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49326-108">Permission type</span></span>      | <span data-ttu-id="49326-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49326-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49326-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49326-110">Delegated (work or school account)</span></span>|<span data-ttu-id="49326-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49326-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="49326-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49326-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="49326-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49326-113">Not supported.</span></span>|
|<span data-ttu-id="49326-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49326-114">Application</span></span>|<span data-ttu-id="49326-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49326-115">Not supported.</span></span>|

<span data-ttu-id="49326-116">Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="49326-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="49326-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49326-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="49326-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49326-118">Request headers</span></span>

|<span data-ttu-id="49326-119">Name</span><span class="sxs-lookup"><span data-stu-id="49326-119">Name</span></span>|<span data-ttu-id="49326-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49326-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="49326-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="49326-121">Authorization</span></span>|<span data-ttu-id="49326-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49326-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="49326-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49326-124">Content-Type</span></span>|<span data-ttu-id="49326-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="49326-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49326-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49326-127">Request body</span></span>

<span data-ttu-id="49326-128">Geben Sie im Textkörper Anforderung ein JSON-Objekt mit einer oder mehrerer Eigenschaften, die aktualisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="49326-128">In the request body, provide a JSON object with one or more properties that need to be updated.</span></span>

|<span data-ttu-id="49326-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49326-129">Property</span></span>|<span data-ttu-id="49326-130">Typ</span><span class="sxs-lookup"><span data-stu-id="49326-130">Type</span></span>|<span data-ttu-id="49326-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49326-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49326-132">clientId</span><span class="sxs-lookup"><span data-stu-id="49326-132">clientId</span></span>|<span data-ttu-id="49326-133">String</span><span class="sxs-lookup"><span data-stu-id="49326-133">String</span></span>|<span data-ttu-id="49326-134">Die Client-ID für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="49326-134">The client ID for the application.</span></span> <span data-ttu-id="49326-135">Dies ist die Client-ID abgerufen wird, wenn die Anwendung mit dem Identitätsanbieter registrieren.</span><span class="sxs-lookup"><span data-stu-id="49326-135">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="49326-136">client_secret</span><span class="sxs-lookup"><span data-stu-id="49326-136">clientSecret</span></span>|<span data-ttu-id="49326-137">String</span><span class="sxs-lookup"><span data-stu-id="49326-137">String</span></span>|<span data-ttu-id="49326-138">Der geheime Clientschlüssel für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="49326-138">The client secret for the application.</span></span> <span data-ttu-id="49326-139">Dies ist der geheime Clientschlüssel erhalten Sie, wenn die Anwendung mit dem Identitätsanbieter registrieren.</span><span class="sxs-lookup"><span data-stu-id="49326-139">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="49326-140">name</span><span class="sxs-lookup"><span data-stu-id="49326-140">name</span></span>|<span data-ttu-id="49326-141">String</span><span class="sxs-lookup"><span data-stu-id="49326-141">String</span></span>|<span data-ttu-id="49326-142">Der Anzeigename des Identitätsanbieters.</span><span class="sxs-lookup"><span data-stu-id="49326-142">The display name of the identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="49326-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="49326-143">Response</span></span>

<span data-ttu-id="49326-144">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49326-144">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="49326-145">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49326-145">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="49326-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49326-146">Example</span></span>

<span data-ttu-id="49326-147">Im folgenden Beispiel wird die Definition der Gültigkeitsdauer von token **IdentityProvider** aktualisiert und platziert es als Standard Organisation.</span><span class="sxs-lookup"><span data-stu-id="49326-147">The following example updates the definition of the token lifetime **identityProvider** and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="49326-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49326-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="49326-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="49326-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
