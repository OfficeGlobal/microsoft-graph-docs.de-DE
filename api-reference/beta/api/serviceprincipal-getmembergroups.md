---
title: 'ServicePrincipal: GetMemberGroups'
description: Rufen Sie die Liste der Gruppen, bei denen diese Dienstprinzipal ein Mitglied ist.  Die Überprüfung ist transitiv.
ms.openlocfilehash: 3ea35e86269f370a3f4fc500555ae04705c038fc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058414"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="ae7be-104">ServicePrincipal: GetMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ae7be-104">servicePrincipal: getMemberGroups</span></span>

> <span data-ttu-id="ae7be-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ae7be-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae7be-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae7be-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae7be-107">Rufen Sie die Liste der Gruppen, bei denen diese Dienstprinzipal ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="ae7be-107">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="ae7be-108">Die Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="ae7be-108">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae7be-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae7be-109">Permissions</span></span>
<span data-ttu-id="ae7be-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae7be-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ae7be-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae7be-112">Permission type</span></span>      | <span data-ttu-id="ae7be-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae7be-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae7be-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae7be-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ae7be-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae7be-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae7be-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae7be-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae7be-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae7be-117">Not supported.</span></span>    |
|<span data-ttu-id="ae7be-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae7be-118">Application</span></span> | <span data-ttu-id="ae7be-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae7be-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae7be-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae7be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="ae7be-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae7be-121">Request headers</span></span>
| <span data-ttu-id="ae7be-122">Name</span><span class="sxs-lookup"><span data-stu-id="ae7be-122">Name</span></span>       | <span data-ttu-id="ae7be-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ae7be-123">Type</span></span> | <span data-ttu-id="ae7be-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae7be-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ae7be-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae7be-125">Authorization</span></span>  | <span data-ttu-id="ae7be-126">string</span><span class="sxs-lookup"><span data-stu-id="ae7be-126">string</span></span>  | <span data-ttu-id="ae7be-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae7be-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae7be-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae7be-129">Request body</span></span>
<span data-ttu-id="ae7be-130">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="ae7be-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ae7be-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="ae7be-131">Parameter</span></span>    | <span data-ttu-id="ae7be-132">Typ</span><span class="sxs-lookup"><span data-stu-id="ae7be-132">Type</span></span>   |<span data-ttu-id="ae7be-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae7be-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae7be-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ae7be-134">securityEnabledOnly</span></span>|<span data-ttu-id="ae7be-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ae7be-135">Boolean</span></span>|<span data-ttu-id="ae7be-p106">Festgelegt auf **false**. Die Option, dass nur Gruppen mit aktivierter Sicherheit zurückgegeben werden, wird nur für Benutzer unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae7be-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="ae7be-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae7be-138">Response</span></span>

<span data-ttu-id="ae7be-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae7be-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae7be-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae7be-140">Example</span></span>
<span data-ttu-id="ae7be-141">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ae7be-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae7be-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae7be-142">Request</span></span>
<span data-ttu-id="ae7be-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae7be-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="ae7be-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae7be-144">Response</span></span>
<span data-ttu-id="ae7be-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae7be-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->