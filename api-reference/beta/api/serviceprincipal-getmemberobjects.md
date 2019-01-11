---
title: 'ServicePrincipal: GetMemberObjects'
description: Rufen Sie die Liste der Gruppen und Directory Rollen, denen dieser Dienst principal ein Mitglied ist.  Diese Überprüfung ist transitiv.
localization_priority: Normal
ms.openlocfilehash: 46c23e18d2484b3dff38ed8791f203e823c4cc9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842119"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="5084d-104">ServicePrincipal: GetMemberObjects</span><span class="sxs-lookup"><span data-stu-id="5084d-104">servicePrincipal: getMemberObjects</span></span>

> <span data-ttu-id="5084d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5084d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5084d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5084d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5084d-107">Rufen Sie die Liste der Gruppen und Directory Rollen, denen dieser Dienst principal ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="5084d-107">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="5084d-108">Diese Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="5084d-108">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5084d-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5084d-109">Permissions</span></span>
<span data-ttu-id="5084d-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5084d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5084d-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5084d-112">Permission type</span></span>      | <span data-ttu-id="5084d-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5084d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5084d-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5084d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5084d-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5084d-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5084d-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5084d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5084d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5084d-117">Not supported.</span></span>    |
|<span data-ttu-id="5084d-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5084d-118">Application</span></span> | <span data-ttu-id="5084d-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5084d-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5084d-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5084d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="5084d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5084d-121">Request headers</span></span>
| <span data-ttu-id="5084d-122">Name</span><span class="sxs-lookup"><span data-stu-id="5084d-122">Name</span></span>       | <span data-ttu-id="5084d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="5084d-123">Type</span></span> | <span data-ttu-id="5084d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5084d-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5084d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5084d-125">Authorization</span></span>  | <span data-ttu-id="5084d-126">string</span><span class="sxs-lookup"><span data-stu-id="5084d-126">string</span></span>  | <span data-ttu-id="5084d-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5084d-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5084d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5084d-129">Request body</span></span>
<span data-ttu-id="5084d-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="5084d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5084d-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="5084d-131">Parameter</span></span>    | <span data-ttu-id="5084d-132">Typ</span><span class="sxs-lookup"><span data-stu-id="5084d-132">Type</span></span>   |<span data-ttu-id="5084d-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5084d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5084d-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="5084d-134">securityEnabledOnly</span></span>|<span data-ttu-id="5084d-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5084d-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="5084d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5084d-136">Response</span></span>

<span data-ttu-id="5084d-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5084d-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5084d-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5084d-138">Example</span></span>
<span data-ttu-id="5084d-139">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5084d-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5084d-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5084d-140">Request</span></span>
<span data-ttu-id="5084d-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5084d-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="5084d-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="5084d-142">Response</span></span>
<span data-ttu-id="5084d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5084d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
