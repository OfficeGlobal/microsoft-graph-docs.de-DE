---
title: Erstellen von identityProvider
description: Erstellen einer neuen IdentityProvider durch Angeben von Anzeigename, IdentityProvider Typ, Client-ID und clientgeheimnis.
localization_priority: Normal
ms.openlocfilehash: c0b005d729510fa68d9edd8bfea7b85687543cf2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514649"
---
# <a name="create-identityprovider"></a><span data-ttu-id="59251-103">Erstellen von identityProvider</span><span class="sxs-lookup"><span data-stu-id="59251-103">Create identityProvider</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59251-104">Erstellen einer neuen [IdentityProvider](../resources/identityprovider.md) durch Angeben von Anzeigename, IdentityProvider Typ, Client-ID und clientgeheimnis.</span><span class="sxs-lookup"><span data-stu-id="59251-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="59251-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="59251-105">Permissions</span></span>

<span data-ttu-id="59251-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59251-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59251-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="59251-108">Permission type</span></span>      | <span data-ttu-id="59251-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="59251-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59251-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="59251-110">Delegated (work or school account)</span></span>|<span data-ttu-id="59251-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59251-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="59251-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="59251-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="59251-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59251-113">Not supported.</span></span>|
|<span data-ttu-id="59251-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="59251-114">Application</span></span>|<span data-ttu-id="59251-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59251-115">Not supported.</span></span>|

<span data-ttu-id="59251-116">Das Konto arbeiten oder Schule muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="59251-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="59251-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59251-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="59251-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="59251-118">Request headers</span></span>

|<span data-ttu-id="59251-119">Name</span><span class="sxs-lookup"><span data-stu-id="59251-119">Name</span></span>|<span data-ttu-id="59251-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59251-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="59251-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="59251-121">Authorization</span></span>|<span data-ttu-id="59251-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="59251-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="59251-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59251-124">Content-Type</span></span>|<span data-ttu-id="59251-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="59251-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59251-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="59251-127">Request body</span></span>

<span data-ttu-id="59251-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [IdentityProvider](../resources/identityprovider.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="59251-128">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) object.</span></span> <span data-ttu-id="59251-129">Alle in der folgenden Tabelle aufgeführten Eigenschaften sind erforderlich.</span><span class="sxs-lookup"><span data-stu-id="59251-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="59251-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="59251-130">Property</span></span>|<span data-ttu-id="59251-131">Typ</span><span class="sxs-lookup"><span data-stu-id="59251-131">Type</span></span>|<span data-ttu-id="59251-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59251-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59251-133">clientId</span><span class="sxs-lookup"><span data-stu-id="59251-133">clientId</span></span>|<span data-ttu-id="59251-134">String</span><span class="sxs-lookup"><span data-stu-id="59251-134">String</span></span>|<span data-ttu-id="59251-135">Die Client-ID für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="59251-135">The client ID for the application.</span></span> <span data-ttu-id="59251-136">Dies ist die Client-ID abgerufen wird, wenn die Anwendung mit dem Identitätsanbieter registrieren.</span><span class="sxs-lookup"><span data-stu-id="59251-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="59251-137">client_secret</span><span class="sxs-lookup"><span data-stu-id="59251-137">clientSecret</span></span>|<span data-ttu-id="59251-138">String</span><span class="sxs-lookup"><span data-stu-id="59251-138">String</span></span>|<span data-ttu-id="59251-139">Der geheime Clientschlüssel für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="59251-139">The client secret for the application.</span></span> <span data-ttu-id="59251-140">Dies ist der geheime Clientschlüssel erhalten Sie, wenn die Anwendung mit dem Identitätsanbieter registrieren.</span><span class="sxs-lookup"><span data-stu-id="59251-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="59251-141">name</span><span class="sxs-lookup"><span data-stu-id="59251-141">name</span></span>|<span data-ttu-id="59251-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="59251-142">String</span></span>|<span data-ttu-id="59251-143">Der Anzeigename des Identitätsanbieters.</span><span class="sxs-lookup"><span data-stu-id="59251-143">The display name of the identity provider.</span></span>|
|<span data-ttu-id="59251-144">type</span><span class="sxs-lookup"><span data-stu-id="59251-144">type</span></span>|<span data-ttu-id="59251-145">String</span><span class="sxs-lookup"><span data-stu-id="59251-145">String</span></span>|<span data-ttu-id="59251-146">Der Typ der Identität Anbieter.</span><span class="sxs-lookup"><span data-stu-id="59251-146">The identity provider type.</span></span> <span data-ttu-id="59251-147">Es muss eine der folgenden Werte sein:</span><span class="sxs-lookup"><span data-stu-id="59251-147">It must be one of the following values:</span></span> <ul><li/><span data-ttu-id="59251-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="59251-148">Microsoft</span></span><li/><span data-ttu-id="59251-149">Google</span><span class="sxs-lookup"><span data-stu-id="59251-149">Google</span></span><li/><span data-ttu-id="59251-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="59251-150">Amazon</span></span><li/><span data-ttu-id="59251-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="59251-151">LinkedIn</span></span><li/><span data-ttu-id="59251-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="59251-152">Facebook</span></span></ul>|

## <a name="response"></a><span data-ttu-id="59251-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="59251-153">Response</span></span>

<span data-ttu-id="59251-154">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [IdentityProvider](../resources/identityprovider.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="59251-154">If successful, this method returns `201 Created` response code and [identityProvider](../resources/identityprovider.md) object in the response body.</span></span> <span data-ttu-id="59251-155">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="59251-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="59251-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59251-156">Example</span></span>

<span data-ttu-id="59251-157">Das folgende Beispiel erstellt eine **IdentityProvider**.</span><span class="sxs-lookup"><span data-stu-id="59251-157">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="59251-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59251-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="59251-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="59251-159">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-post-identityproviders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
