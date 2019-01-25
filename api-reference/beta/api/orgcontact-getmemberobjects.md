---
title: 'OrgContact: GetMemberObjects'
description: Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema Berechtigungen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab9d516fe4200a188defe026fdf44ac183bb5909
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523750"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="c1c29-104">OrgContact: GetMemberObjects</span><span class="sxs-lookup"><span data-stu-id="c1c29-104">orgContact: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="c1c29-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c1c29-105">Permissions</span></span>
<span data-ttu-id="c1c29-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1c29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1c29-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1c29-108">Permission type</span></span>      | <span data-ttu-id="c1c29-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1c29-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1c29-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1c29-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1c29-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c1c29-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c1c29-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1c29-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1c29-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1c29-113">Not supported.</span></span>    |
|<span data-ttu-id="c1c29-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1c29-114">Application</span></span> | <span data-ttu-id="c1c29-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1c29-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1c29-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1c29-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="c1c29-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1c29-117">Request headers</span></span>
| <span data-ttu-id="c1c29-118">Name</span><span class="sxs-lookup"><span data-stu-id="c1c29-118">Name</span></span>       | <span data-ttu-id="c1c29-119">Typ</span><span class="sxs-lookup"><span data-stu-id="c1c29-119">Type</span></span> | <span data-ttu-id="c1c29-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1c29-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c1c29-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1c29-121">Authorization</span></span>  | <span data-ttu-id="c1c29-122">string</span><span class="sxs-lookup"><span data-stu-id="c1c29-122">string</span></span>  | <span data-ttu-id="c1c29-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c1c29-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1c29-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1c29-125">Request body</span></span>
<span data-ttu-id="c1c29-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="c1c29-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1c29-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="c1c29-127">Parameter</span></span>    | <span data-ttu-id="c1c29-128">Typ</span><span class="sxs-lookup"><span data-stu-id="c1c29-128">Type</span></span>   |<span data-ttu-id="c1c29-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1c29-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1c29-130">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="c1c29-130">securityEnabledOnly</span></span>|<span data-ttu-id="c1c29-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c1c29-131">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="c1c29-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1c29-132">Response</span></span>

<span data-ttu-id="c1c29-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1c29-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1c29-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1c29-134">Example</span></span>
<span data-ttu-id="c1c29-135">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c1c29-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c1c29-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1c29-136">Request</span></span>
<span data-ttu-id="c1c29-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1c29-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="c1c29-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1c29-138">Response</span></span>
<span data-ttu-id="c1c29-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1c29-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-getmemberobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
