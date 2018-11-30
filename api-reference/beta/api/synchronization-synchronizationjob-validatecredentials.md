---
title: 'SynchronizationJob: ValidateCredentials'
description: Überprüfen Sie, dass die Anmeldeinformationen im Mandanten gültig sind.
ms.openlocfilehash: b4f488787474158172800fe23d7d0ae78ef6a366
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059738"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="3ae1e-103">SynchronizationJob: ValidateCredentials</span><span class="sxs-lookup"><span data-stu-id="3ae1e-103">synchronizationJob: validateCredentials</span></span>

> <span data-ttu-id="3ae1e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ae1e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ae1e-106">Überprüfen Sie, dass die Anmeldeinformationen im Mandanten gültig sind.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-106">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ae1e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3ae1e-107">Permissions</span></span>
<span data-ttu-id="3ae1e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ae1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ae1e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ae1e-110">Permission type</span></span>                        | <span data-ttu-id="3ae1e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ae1e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ae1e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ae1e-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="3ae1e-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ae1e-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3ae1e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ae1e-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3ae1e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ae1e-115">Not supported.</span></span> |
|<span data-ttu-id="3ae1e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ae1e-116">Application</span></span>                            |<span data-ttu-id="3ae1e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ae1e-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="3ae1e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ae1e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="3ae1e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ae1e-119">Request headers</span></span>
| <span data-ttu-id="3ae1e-120">Name</span><span class="sxs-lookup"><span data-stu-id="3ae1e-120">Name</span></span>       | <span data-ttu-id="3ae1e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ae1e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3ae1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ae1e-122">Authorization</span></span>  | <span data-ttu-id="3ae1e-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3ae1e-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ae1e-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ae1e-124">Request body</span></span>
<span data-ttu-id="3ae1e-125">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ae1e-126">Parameter</span><span class="sxs-lookup"><span data-stu-id="3ae1e-126">Parameter</span></span>    | <span data-ttu-id="3ae1e-127">Typ</span><span class="sxs-lookup"><span data-stu-id="3ae1e-127">Type</span></span>   |<span data-ttu-id="3ae1e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ae1e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ae1e-129">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="3ae1e-129">useSavedCredentials</span></span>|<span data-ttu-id="3ae1e-130">Boolesch</span><span class="sxs-lookup"><span data-stu-id="3ae1e-130">Boolean</span></span>|<span data-ttu-id="3ae1e-131">Wenn `true`, die `credentials` Parameter wird ignoriert, und die zuvor gespeicherten Anmeldeinformationen (falls vorhanden), werden stattdessen überprüft werden.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-131">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="3ae1e-132">Anmeldeinformationen</span><span class="sxs-lookup"><span data-stu-id="3ae1e-132">credentials</span></span>|<span data-ttu-id="3ae1e-133">[SynchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3ae1e-133">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="3ae1e-134">Die Anmeldeinformationen zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-134">Credentials to validate.</span></span> <span data-ttu-id="3ae1e-135">Ignoriert, wenn die `useSavedCredentials` Parameter ist `true`.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-135">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="3ae1e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ae1e-136">Response</span></span>
<span data-ttu-id="3ae1e-137">Wenn die Validierung erfolgreich ist, gibt diese Methode einen `204, No Content` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-137">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="3ae1e-138">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-138">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ae1e-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ae1e-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ae1e-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ae1e-140">Request</span></span>
<span data-ttu-id="3ae1e-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-141">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3ae1e-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ae1e-142">Response</span></span>
<span data-ttu-id="3ae1e-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3ae1e-143">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->