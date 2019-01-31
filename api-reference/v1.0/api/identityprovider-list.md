---
title: Auflisten von Identitätsanbietern
description: Abrufen aller Identitätsanbieter
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 06cf62ef006348b46b38f78b50dae95267921489
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649403"
---
# <a name="list-identityproviders"></a><span data-ttu-id="e7b18-103">Auflisten von Identitätsanbietern</span><span class="sxs-lookup"><span data-stu-id="e7b18-103">List identityProviders</span></span>

<span data-ttu-id="e7b18-104">Abrufen aller [Identitätsanbietern](../resources/identityprovider.md) in Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="e7b18-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7b18-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e7b18-105">Permissions</span></span>

<span data-ttu-id="e7b18-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7b18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7b18-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e7b18-108">Permission type</span></span>      | <span data-ttu-id="e7b18-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e7b18-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7b18-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e7b18-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e7b18-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7b18-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e7b18-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e7b18-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e7b18-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7b18-113">Not supported.</span></span>|
|<span data-ttu-id="e7b18-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e7b18-114">Application</span></span>|<span data-ttu-id="e7b18-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7b18-115">Not supported.</span></span>|

<span data-ttu-id="e7b18-116">Das Geschäfts-, Schul- oder Unikonto muss ein globaler Administrator des Mandanten sein.</span><span class="sxs-lookup"><span data-stu-id="e7b18-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="e7b18-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7b18-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="e7b18-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e7b18-118">Request headers</span></span>

|<span data-ttu-id="e7b18-119">Name</span><span class="sxs-lookup"><span data-stu-id="e7b18-119">Name</span></span>|<span data-ttu-id="e7b18-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7b18-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e7b18-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7b18-121">Authorization</span></span>|<span data-ttu-id="e7b18-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e7b18-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7b18-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e7b18-124">Request body</span></span>

<span data-ttu-id="e7b18-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e7b18-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7b18-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7b18-126">Response</span></span>

<span data-ttu-id="e7b18-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Auflistung von [Identitätsanbietern](../resources/identityProvider.md) in JSON-Darstellung im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7b18-127">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/identityProvider.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7b18-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7b18-128">Example</span></span>

<span data-ttu-id="e7b18-129">Im folgenden Beispiel werden alle **Identitätsanbieter** abgerufen.</span><span class="sxs-lookup"><span data-stu-id="e7b18-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="e7b18-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7b18-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list-identityproviders"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders
```

##### <a name="response"></a><span data-ttu-id="e7b18-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7b18-131">Response</span></span>

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
