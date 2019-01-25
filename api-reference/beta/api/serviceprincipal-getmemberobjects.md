---
title: 'ServicePrincipal: GetMemberObjects'
description: Rufen Sie die Liste der Gruppen und Directory Rollen, denen dieser Dienst principal ein Mitglied ist.  Diese Überprüfung ist transitiv.
localization_priority: Normal
ms.openlocfilehash: a1856e0c359e464078f7689043d1bea493c2bb13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520760"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="4bc5c-104">ServicePrincipal: GetMemberObjects</span><span class="sxs-lookup"><span data-stu-id="4bc5c-104">servicePrincipal: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bc5c-105">Rufen Sie die Liste der Gruppen und Directory Rollen, denen dieser Dienst principal ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="4bc5c-105">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="4bc5c-106">Diese Überprüfung ist transitiv.</span><span class="sxs-lookup"><span data-stu-id="4bc5c-106">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bc5c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4bc5c-107">Permissions</span></span>
<span data-ttu-id="4bc5c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4bc5c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bc5c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4bc5c-110">Permission type</span></span>      | <span data-ttu-id="4bc5c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4bc5c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bc5c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4bc5c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4bc5c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4bc5c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4bc5c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4bc5c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bc5c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4bc5c-115">Not supported.</span></span>    |
|<span data-ttu-id="4bc5c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4bc5c-116">Application</span></span> | <span data-ttu-id="4bc5c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bc5c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bc5c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bc5c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="4bc5c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4bc5c-119">Request headers</span></span>
| <span data-ttu-id="4bc5c-120">Name</span><span class="sxs-lookup"><span data-stu-id="4bc5c-120">Name</span></span>       | <span data-ttu-id="4bc5c-121">Typ</span><span class="sxs-lookup"><span data-stu-id="4bc5c-121">Type</span></span> | <span data-ttu-id="4bc5c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bc5c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4bc5c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bc5c-123">Authorization</span></span>  | <span data-ttu-id="4bc5c-124">string</span><span class="sxs-lookup"><span data-stu-id="4bc5c-124">string</span></span>  | <span data-ttu-id="4bc5c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4bc5c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4bc5c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4bc5c-127">Request body</span></span>
<span data-ttu-id="4bc5c-128">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4bc5c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4bc5c-129">Parameter</span><span class="sxs-lookup"><span data-stu-id="4bc5c-129">Parameter</span></span>    | <span data-ttu-id="4bc5c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4bc5c-130">Type</span></span>   |<span data-ttu-id="4bc5c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4bc5c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bc5c-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4bc5c-132">securityEnabledOnly</span></span>|<span data-ttu-id="4bc5c-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4bc5c-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="4bc5c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bc5c-134">Response</span></span>

<span data-ttu-id="4bc5c-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4bc5c-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bc5c-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4bc5c-136">Example</span></span>
<span data-ttu-id="4bc5c-137">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="4bc5c-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4bc5c-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4bc5c-138">Request</span></span>
<span data-ttu-id="4bc5c-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4bc5c-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4bc5c-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4bc5c-140">Response</span></span>
<span data-ttu-id="4bc5c-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4bc5c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-getmemberobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
