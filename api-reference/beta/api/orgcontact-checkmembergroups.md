---
title: 'OrgContact: CheckMemberGroups'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ef9345a1879789a3f96a3eb6b2bbe4d636c75ddc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523785"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="8fb77-104">OrgContact: CheckMemberGroups</span><span class="sxs-lookup"><span data-stu-id="8fb77-104">orgContact: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="8fb77-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8fb77-105">Permissions</span></span>
<span data-ttu-id="8fb77-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fb77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fb77-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8fb77-108">Permission type</span></span>      | <span data-ttu-id="8fb77-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8fb77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fb77-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8fb77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8fb77-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8fb77-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8fb77-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8fb77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fb77-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8fb77-113">Not supported.</span></span>    |
|<span data-ttu-id="8fb77-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8fb77-114">Application</span></span> | <span data-ttu-id="8fb77-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fb77-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fb77-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fb77-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="8fb77-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8fb77-117">Request headers</span></span>
| <span data-ttu-id="8fb77-118">Name</span><span class="sxs-lookup"><span data-stu-id="8fb77-118">Name</span></span>       | <span data-ttu-id="8fb77-119">Typ</span><span class="sxs-lookup"><span data-stu-id="8fb77-119">Type</span></span> | <span data-ttu-id="8fb77-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fb77-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8fb77-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fb77-121">Authorization</span></span>  | <span data-ttu-id="8fb77-122">string</span><span class="sxs-lookup"><span data-stu-id="8fb77-122">string</span></span>  | <span data-ttu-id="8fb77-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8fb77-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fb77-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8fb77-125">Request body</span></span>
<span data-ttu-id="8fb77-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="8fb77-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8fb77-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="8fb77-127">Parameter</span></span>    | <span data-ttu-id="8fb77-128">Typ</span><span class="sxs-lookup"><span data-stu-id="8fb77-128">Type</span></span>   |<span data-ttu-id="8fb77-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fb77-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fb77-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="8fb77-130">groupIds</span></span>|<span data-ttu-id="8fb77-131">String</span><span class="sxs-lookup"><span data-stu-id="8fb77-131">String</span></span>||

## <a name="response"></a><span data-ttu-id="8fb77-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fb77-132">Response</span></span>

<span data-ttu-id="8fb77-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8fb77-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fb77-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8fb77-134">Example</span></span>
<span data-ttu-id="8fb77-135">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8fb77-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8fb77-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fb77-136">Request</span></span>
<span data-ttu-id="8fb77-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8fb77-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="8fb77-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fb77-138">Response</span></span>
<span data-ttu-id="8fb77-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8fb77-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
