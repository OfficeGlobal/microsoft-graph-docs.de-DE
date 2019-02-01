---
title: Erstellen eines Identitätsanbieters
description: Erstellen eines neuen Identitätsanbieters.
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a33354c35903fedc3efedb84e9f2ed7bc20c9506
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649413"
---
# <a name="create-identityprovider"></a><span data-ttu-id="32660-103">Erstellen eines Identitätsanbieters</span><span class="sxs-lookup"><span data-stu-id="32660-103">Create identityProvider</span></span>

<span data-ttu-id="32660-104">Erstellen Sie einen neuen [Identitätsanbieter](../resources/identityprovider.md), indem Sie den Anzeigenamen, den Typ des Identitätsanbieters, die Client-ID sowie den geheimen Clientschlüssel angeben.</span><span class="sxs-lookup"><span data-stu-id="32660-104">Create a new [identityProvider](../resources/identityprovider.md) by specifying display name, identityProvider type, client ID, and client secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="32660-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="32660-105">Permissions</span></span>

<span data-ttu-id="32660-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32660-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32660-108">Permission type</span></span>      | <span data-ttu-id="32660-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32660-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32660-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32660-110">Delegated (work or school account)</span></span>|<span data-ttu-id="32660-111">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32660-111">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="32660-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32660-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="32660-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32660-113">Not supported.</span></span>|
|<span data-ttu-id="32660-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32660-114">Application</span></span>|<span data-ttu-id="32660-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32660-115">Not supported.</span></span>|

<span data-ttu-id="32660-116">Das Geschäfts-, Schul- oder Unikonto muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="32660-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="32660-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32660-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="32660-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32660-118">Request headers</span></span>

|<span data-ttu-id="32660-119">Name</span><span class="sxs-lookup"><span data-stu-id="32660-119">Name</span></span>|<span data-ttu-id="32660-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32660-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="32660-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32660-121">Authorization</span></span>|<span data-ttu-id="32660-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="32660-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="32660-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32660-124">Content-Type</span></span>|<span data-ttu-id="32660-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="32660-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32660-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32660-127">Request body</span></span>

<span data-ttu-id="32660-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [identityProvider](../resources/identityProvider.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="32660-128">In the request body, supply a JSON representation of a [team](../resources/identityProvider.md) object.</span></span> <span data-ttu-id="32660-129">Alle in der folgenden Tabelle aufgeführten Eigenschaften sind erforderlich.</span><span class="sxs-lookup"><span data-stu-id="32660-129">All the properties listed in the following table are required.</span></span>

|<span data-ttu-id="32660-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32660-130">Property</span></span>|<span data-ttu-id="32660-131">Typ</span><span class="sxs-lookup"><span data-stu-id="32660-131">Type</span></span>|<span data-ttu-id="32660-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32660-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32660-133">clientId</span><span class="sxs-lookup"><span data-stu-id="32660-133">clientId</span></span>|<span data-ttu-id="32660-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32660-134">String</span></span>|<span data-ttu-id="32660-135">Die Client-ID für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="32660-135">The client ID created for your application.</span></span> <span data-ttu-id="32660-136">Dies ist die Client-ID, die Sie beim Registrieren der Anwendung beim Identitätsanbieter erhalten.</span><span class="sxs-lookup"><span data-stu-id="32660-136">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="32660-137">clientSecret</span><span class="sxs-lookup"><span data-stu-id="32660-137">client_secret</span></span>|<span data-ttu-id="32660-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32660-138">String</span></span>|<span data-ttu-id="32660-139">Der geheime Clientschlüssel für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="32660-139">The client secret created for your application.</span></span> <span data-ttu-id="32660-140">Dies ist der geheime Clientschlüssel, den Sie beim Registrieren der Anwendung beim Identitätsanbieter erhalten.</span><span class="sxs-lookup"><span data-stu-id="32660-140">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="32660-141">name</span><span class="sxs-lookup"><span data-stu-id="32660-141">name</span></span>|<span data-ttu-id="32660-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32660-142">String</span></span>|<span data-ttu-id="32660-143">Der Anzeigename des Identitätsanbieters.</span><span class="sxs-lookup"><span data-stu-id="32660-143">The unique name of the identity provider.</span></span>|
|<span data-ttu-id="32660-144">type</span><span class="sxs-lookup"><span data-stu-id="32660-144">type</span></span>|<span data-ttu-id="32660-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="32660-145">String</span></span>|<span data-ttu-id="32660-146">Der Typ des Identitätsanbieters.</span><span class="sxs-lookup"><span data-stu-id="32660-146">The identity provider type.</span></span> <span data-ttu-id="32660-147">Der Typ muss einer der folgenden Werte für B2C-Szenarien sein:</span><span class="sxs-lookup"><span data-stu-id="32660-147">It must be one of the following values for B2C Scenarios:</span></span> <ul><li/><span data-ttu-id="32660-148">Microsoft</span><span class="sxs-lookup"><span data-stu-id="32660-148">Microsoft</span></span><li/><span data-ttu-id="32660-149">Google</span><span class="sxs-lookup"><span data-stu-id="32660-149">Google</span></span><li/><span data-ttu-id="32660-150">Amazon</span><span class="sxs-lookup"><span data-stu-id="32660-150">Amazon</span></span><li/><span data-ttu-id="32660-151">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="32660-151">LinkedIn</span></span><li/><span data-ttu-id="32660-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="32660-152">Facebook</span></span><li/><span data-ttu-id="32660-153">GitHub</span><span class="sxs-lookup"><span data-stu-id="32660-153">GitHub</span></span><li/><span data-ttu-id="32660-154">Twitter</span><span class="sxs-lookup"><span data-stu-id="32660-154">Twitter</span></span><li/><span data-ttu-id="32660-155">Weibo</span><span class="sxs-lookup"><span data-stu-id="32660-155">Weibo</span></span><li/><span data-ttu-id="32660-156">QQ</span><span class="sxs-lookup"><span data-stu-id="32660-156">QQ</span></span><li/><span data-ttu-id="32660-157">WeChat</span><span class="sxs-lookup"><span data-stu-id="32660-157">WeChat</span></span></ul><span data-ttu-id="32660-158">Für B2B kann er nur Google sein.</span><span class="sxs-lookup"><span data-stu-id="32660-158">For B2B it can only be Google</span></span>|

## <a name="response"></a><span data-ttu-id="32660-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="32660-159">Response</span></span>

<span data-ttu-id="32660-160">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [identityProvider](../resources/identityProvider.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32660-160">If successful, this method returns a `201 Created` response code and [Contract](../resources/identityProvider.md) object in the response body.</span></span> <span data-ttu-id="32660-161">Wenn die Methode nicht erfolgreich ist, wird ein `4xx`-Fehler mit bestimmten Details zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32660-161">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="32660-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32660-162">Example</span></span>

<span data-ttu-id="32660-163">Im folgenden Beispiel wird ein **Identitätsanbieter** erstellt.</span><span class="sxs-lookup"><span data-stu-id="32660-163">The following example creates an **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="32660-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32660-164">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/identityProviders
Content-type: application/json

{
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

##### <a name="response"></a><span data-ttu-id="32660-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="32660-165">Response</span></span>

<!-- { "blockType": "ignored" } -->
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


