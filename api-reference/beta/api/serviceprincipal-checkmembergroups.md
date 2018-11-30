---
title: 'ServicePrincipal: CheckMemberGroups'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
ms.openlocfilehash: bf16206e9029ddcf687738c3a7db5a0a27a43903
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057899"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="349ba-104">ServicePrincipal: CheckMemberGroups</span><span class="sxs-lookup"><span data-stu-id="349ba-104">servicePrincipal: checkMemberGroups</span></span>

> <span data-ttu-id="349ba-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="349ba-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="349ba-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="349ba-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="349ba-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="349ba-107">Permissions</span></span>
<span data-ttu-id="349ba-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="349ba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="349ba-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="349ba-110">Permission type</span></span>      | <span data-ttu-id="349ba-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="349ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="349ba-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="349ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="349ba-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="349ba-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="349ba-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="349ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="349ba-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="349ba-115">Not supported.</span></span>    |
|<span data-ttu-id="349ba-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="349ba-116">Application</span></span> | <span data-ttu-id="349ba-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="349ba-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="349ba-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="349ba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="349ba-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="349ba-119">Request headers</span></span>
| <span data-ttu-id="349ba-120">Name</span><span class="sxs-lookup"><span data-stu-id="349ba-120">Name</span></span>       | <span data-ttu-id="349ba-121">Typ</span><span class="sxs-lookup"><span data-stu-id="349ba-121">Type</span></span> | <span data-ttu-id="349ba-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="349ba-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="349ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="349ba-123">Authorization</span></span>  | <span data-ttu-id="349ba-124">string</span><span class="sxs-lookup"><span data-stu-id="349ba-124">string</span></span>  | <span data-ttu-id="349ba-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="349ba-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="349ba-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="349ba-127">Request body</span></span>
<span data-ttu-id="349ba-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="349ba-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="349ba-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="349ba-129">Parameter</span></span>    | <span data-ttu-id="349ba-130">Typ</span><span class="sxs-lookup"><span data-stu-id="349ba-130">Type</span></span>   |<span data-ttu-id="349ba-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="349ba-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="349ba-132">groupIds</span><span class="sxs-lookup"><span data-stu-id="349ba-132">groupIds</span></span>|<span data-ttu-id="349ba-133">String</span><span class="sxs-lookup"><span data-stu-id="349ba-133">String</span></span>||

## <a name="response"></a><span data-ttu-id="349ba-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="349ba-134">Response</span></span>

<span data-ttu-id="349ba-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="349ba-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="349ba-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="349ba-136">Example</span></span>
<span data-ttu-id="349ba-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="349ba-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="349ba-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="349ba-138">Request</span></span>
<span data-ttu-id="349ba-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="349ba-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="349ba-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="349ba-140">Response</span></span>
<span data-ttu-id="349ba-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="349ba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->