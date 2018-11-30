---
title: Erstellen von identityProvider
description: Erstellen einer neuen IdentityProvider durch Angeben von Anzeigename, IdentityProvider Typ, Client-ID und clientgeheimnis.
ms.openlocfilehash: 8786cbf6676567a0c6aaef5bf497f50cff1ce9a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062691"
---
# <a name="create-identityprovider"></a><span data-ttu-id="bf211-103">Erstellen von identityProvider</span><span class="sxs-lookup"><span data-stu-id="bf211-103">Create identityProvider</span></span>

> <span data-ttu-id="bf211-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bf211-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf211-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bf211-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf211-106">Erstellen einer neuen [IdentityProvider](../resources/identityprovider.md) durch Angeben von Anzeigename, IdentityProvider Typ, Client-ID und clientgeheimnis.</span><span class="sxs-lookup"><span data-stu-id="bf211-106">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf211-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bf211-107">Permissions</span></span>

<span data-ttu-id="bf211-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf211-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf211-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bf211-110">Permission type</span></span>      | <span data-ttu-id="bf211-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bf211-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf211-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bf211-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf211-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf211-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="bf211-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bf211-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bf211-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf211-115">Not supported.</span></span>|
|<span data-ttu-id="bf211-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bf211-116">Application</span></span>|<span data-ttu-id="bf211-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf211-117">Not supported.</span></span>|

<span data-ttu-id="bf211-118">Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="bf211-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="bf211-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf211-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="bf211-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bf211-120">Request headers</span></span>

|<span data-ttu-id="bf211-121">Name</span><span class="sxs-lookup"><span data-stu-id="bf211-121">Name</span></span>|<span data-ttu-id="bf211-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf211-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="bf211-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf211-123">Authorization</span></span>|<span data-ttu-id="bf211-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bf211-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bf211-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf211-126">Content-Type</span></span>|<span data-ttu-id="bf211-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="bf211-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf211-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bf211-129">Request body</span></span>

<span data-ttu-id="bf211-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [IdentityProvider](../resources/identityprovider.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bf211-130">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="bf211-131">Alle in der folgenden Tabelle aufgeführten Eigenschaften sind erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bf211-131">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="bf211-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bf211-132">Property</span></span>|<span data-ttu-id="bf211-133">Typ</span><span class="sxs-lookup"><span data-stu-id="bf211-133">Type</span></span>|<span data-ttu-id="bf211-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf211-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf211-135">clientId</span><span class="sxs-lookup"><span data-stu-id="bf211-135">clientId</span></span>|<span data-ttu-id="bf211-136">String</span><span class="sxs-lookup"><span data-stu-id="bf211-136">String</span></span>|<span data-ttu-id="bf211-137">Die Client-ID für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="bf211-137">The client ID for the application.</span></span> <span data-ttu-id="bf211-138">Dies ist die Client-ID abgerufen wird, wenn die Anwendung mit dem Identitätsanbieter registrieren.</span><span class="sxs-lookup"><span data-stu-id="bf211-138">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="bf211-139">clientSecret</span><span class="sxs-lookup"><span data-stu-id="bf211-139">clientSecret</span></span>|<span data-ttu-id="bf211-140">String</span><span class="sxs-lookup"><span data-stu-id="bf211-140">String</span></span>|<span data-ttu-id="bf211-141">Der geheime Clientschlüssel für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="bf211-141">The client secret for the application.</span></span> <span data-ttu-id="bf211-142">Dies ist der geheime Clientschlüssel erhalten Sie, wenn die Anwendung mit dem Identitätsanbieter registrieren.</span><span class="sxs-lookup"><span data-stu-id="bf211-142">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="bf211-143">name</span><span class="sxs-lookup"><span data-stu-id="bf211-143">name</span></span>|<span data-ttu-id="bf211-144">String</span><span class="sxs-lookup"><span data-stu-id="bf211-144">String</span></span>|<span data-ttu-id="bf211-145">Der Anzeigename des Identitätsanbieters.</span><span class="sxs-lookup"><span data-stu-id="bf211-145">The display name of the identity provider.</span></span>|
|<span data-ttu-id="bf211-146">Typ</span><span class="sxs-lookup"><span data-stu-id="bf211-146">type</span></span>|<span data-ttu-id="bf211-147">String</span><span class="sxs-lookup"><span data-stu-id="bf211-147">String</span></span>|<span data-ttu-id="bf211-148">Der Typ der Identität Anbieter.</span><span class="sxs-lookup"><span data-stu-id="bf211-148">The identity provider type.</span></span> <span data-ttu-id="bf211-149">Es muss eine der folgenden Werte sein:</span><span class="sxs-lookup"><span data-stu-id="bf211-149">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="bf211-150">Microsoft</span><span class="sxs-lookup"><span data-stu-id="bf211-150">Microsoft</span></span><li/><span data-ttu-id="bf211-151">Google</span><span class="sxs-lookup"><span data-stu-id="bf211-151">Google</span></span><li/><span data-ttu-id="bf211-152">Amazon</span><span class="sxs-lookup"><span data-stu-id="bf211-152">Amazon</span></span><li/><span data-ttu-id="bf211-153">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="bf211-153">LinkedIn</span></span><li/><span data-ttu-id="bf211-154">Facebook</span><span class="sxs-lookup"><span data-stu-id="bf211-154">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="bf211-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf211-155">Response</span></span>

<span data-ttu-id="bf211-156">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [IdentityProvider](../resources/identityprovider.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bf211-156">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="bf211-157">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf211-157">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="bf211-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bf211-158">Example</span></span>

<span data-ttu-id="bf211-159">Das folgende Beispiel erstellt eine **IdentityProvider**.</span><span class="sxs-lookup"><span data-stu-id="bf211-159">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="bf211-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf211-160">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}-->
```http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a><span data-ttu-id="bf211-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf211-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
