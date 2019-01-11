---
title: 'OrgContact: GetMemberGroups'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
localization_priority: Normal
ms.openlocfilehash: 77ec78708a7f1647133e85ae521417cf358996b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836050"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="7aa38-104">OrgContact: GetMemberGroups</span><span class="sxs-lookup"><span data-stu-id="7aa38-104">orgContact: getMemberGroups</span></span>

> <span data-ttu-id="7aa38-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7aa38-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7aa38-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7aa38-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aa38-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7aa38-107">Permissions</span></span>
<span data-ttu-id="7aa38-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aa38-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa38-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7aa38-110">Permission type</span></span>      | <span data-ttu-id="7aa38-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7aa38-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aa38-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7aa38-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7aa38-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7aa38-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7aa38-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7aa38-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aa38-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7aa38-115">Not supported.</span></span>    |
|<span data-ttu-id="7aa38-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7aa38-116">Application</span></span> | <span data-ttu-id="7aa38-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa38-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aa38-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7aa38-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="7aa38-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7aa38-119">Request headers</span></span>
| <span data-ttu-id="7aa38-120">Name</span><span class="sxs-lookup"><span data-stu-id="7aa38-120">Name</span></span>       | <span data-ttu-id="7aa38-121">Typ</span><span class="sxs-lookup"><span data-stu-id="7aa38-121">Type</span></span> | <span data-ttu-id="7aa38-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7aa38-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7aa38-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aa38-123">Authorization</span></span>  | <span data-ttu-id="7aa38-124">string</span><span class="sxs-lookup"><span data-stu-id="7aa38-124">string</span></span>  | <span data-ttu-id="7aa38-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7aa38-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aa38-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7aa38-127">Request body</span></span>
<span data-ttu-id="7aa38-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="7aa38-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7aa38-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="7aa38-129">Parameter</span></span>    | <span data-ttu-id="7aa38-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7aa38-130">Type</span></span>   |<span data-ttu-id="7aa38-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7aa38-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7aa38-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="7aa38-132">securityEnabledOnly</span></span>|<span data-ttu-id="7aa38-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7aa38-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="7aa38-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7aa38-134">Response</span></span>

<span data-ttu-id="7aa38-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7aa38-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aa38-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7aa38-136">Example</span></span>
<span data-ttu-id="7aa38-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="7aa38-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7aa38-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7aa38-138">Request</span></span>
<span data-ttu-id="7aa38-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7aa38-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="7aa38-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="7aa38-140">Response</span></span>
<span data-ttu-id="7aa38-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7aa38-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
