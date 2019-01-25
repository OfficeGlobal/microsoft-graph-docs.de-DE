---
title: 'SynchronizationJob: ValidateCredentials'
description: Überprüfen Sie, dass die Anmeldeinformationen im Mandanten gültig sind.
localization_priority: Normal
ms.openlocfilehash: 122d673e89f15697b2fdeefbcefb516cf9ad89ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519003"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="7d556-103">SynchronizationJob: ValidateCredentials</span><span class="sxs-lookup"><span data-stu-id="7d556-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d556-104">Überprüfen Sie, dass die Anmeldeinformationen im Mandanten gültig sind.</span><span class="sxs-lookup"><span data-stu-id="7d556-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d556-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7d556-105">Permissions</span></span>
<span data-ttu-id="7d556-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d556-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d556-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7d556-108">Permission type</span></span>                        | <span data-ttu-id="7d556-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7d556-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d556-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7d556-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="7d556-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d556-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7d556-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7d556-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7d556-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d556-113">Not supported.</span></span> |
|<span data-ttu-id="7d556-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7d556-114">Application</span></span>                            |<span data-ttu-id="7d556-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d556-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="7d556-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d556-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="7d556-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7d556-117">Request headers</span></span>
| <span data-ttu-id="7d556-118">Name</span><span class="sxs-lookup"><span data-stu-id="7d556-118">Name</span></span>       | <span data-ttu-id="7d556-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d556-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d556-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d556-120">Authorization</span></span>  | <span data-ttu-id="7d556-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7d556-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d556-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7d556-122">Request body</span></span>
<span data-ttu-id="7d556-123">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="7d556-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7d556-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="7d556-124">Parameter</span></span>    | <span data-ttu-id="7d556-125">Typ</span><span class="sxs-lookup"><span data-stu-id="7d556-125">Type</span></span>   |<span data-ttu-id="7d556-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d556-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d556-127">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="7d556-127">useSavedCredentials</span></span>|<span data-ttu-id="7d556-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7d556-128">Boolean</span></span>|<span data-ttu-id="7d556-129">Wenn `true`, die `credentials` Parameter wird ignoriert, und die zuvor gespeicherten Anmeldeinformationen (falls vorhanden), werden stattdessen überprüft werden.</span><span class="sxs-lookup"><span data-stu-id="7d556-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="7d556-130">Credentials</span><span class="sxs-lookup"><span data-stu-id="7d556-130">credentials</span></span>|<span data-ttu-id="7d556-131">[SynchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7d556-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="7d556-132">Die Anmeldeinformationen zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="7d556-132">Credentials to validate.</span></span> <span data-ttu-id="7d556-133">Ignoriert, wenn die `useSavedCredentials` Parameter ist `true`.</span><span class="sxs-lookup"><span data-stu-id="7d556-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="7d556-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d556-134">Response</span></span>
<span data-ttu-id="7d556-135">Wenn die Validierung erfolgreich ist, gibt diese Methode einen `204, No Content` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="7d556-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="7d556-136">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7d556-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d556-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7d556-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7d556-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d556-138">Request</span></span>
<span data-ttu-id="7d556-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7d556-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_validatecredentials"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials
Content-type: application/json
Content-length: 218

{ 
    credentials: [ 
        { key: "UserName", value: "user@domain.com" },
        { key: "Password", value: "password-value" }
    ]
}
```

##### <a name="response"></a><span data-ttu-id="7d556-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d556-140">Response</span></span>
<span data-ttu-id="7d556-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7d556-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
