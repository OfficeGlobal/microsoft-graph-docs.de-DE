---
title: Abrufen von Gruppenrichtlinien
description: Rufen Sie die Eigenschaften einer Richtlinie ab.
localization_priority: Normal
ms.openlocfilehash: c2ef94c48e2b55f39cc812b9c2e3479a3352a6e6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526739"
---
# <a name="get-policy"></a><span data-ttu-id="6a3b2-103">Abrufen von Gruppenrichtlinien</span><span class="sxs-lookup"><span data-stu-id="6a3b2-103">Get Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a3b2-104">Rufen Sie die Eigenschaften einer [Richtlinie](../resources/policy.md)ab.</span><span class="sxs-lookup"><span data-stu-id="6a3b2-104">Retrieve the properties of a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a3b2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6a3b2-105">Permissions</span></span>
<span data-ttu-id="6a3b2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a3b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a3b2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a3b2-108">Permission type</span></span>      | <span data-ttu-id="6a3b2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a3b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a3b2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a3b2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6a3b2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a3b2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a3b2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a3b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a3b2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a3b2-113">Not supported.</span></span>    |
|<span data-ttu-id="6a3b2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a3b2-114">Application</span></span> | <span data-ttu-id="6a3b2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a3b2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a3b2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a3b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6a3b2-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a3b2-117">Request headers</span></span>
| <span data-ttu-id="6a3b2-118">Name</span><span class="sxs-lookup"><span data-stu-id="6a3b2-118">Name</span></span>       | <span data-ttu-id="6a3b2-119">Typ</span><span class="sxs-lookup"><span data-stu-id="6a3b2-119">Type</span></span> | <span data-ttu-id="6a3b2-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a3b2-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6a3b2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a3b2-121">Authorization</span></span>  | <span data-ttu-id="6a3b2-122">string</span><span class="sxs-lookup"><span data-stu-id="6a3b2-122">string</span></span>  | <span data-ttu-id="6a3b2-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a3b2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a3b2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a3b2-125">Request body</span></span>
<span data-ttu-id="6a3b2-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6a3b2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a3b2-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a3b2-127">Response</span></span>

<span data-ttu-id="6a3b2-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und [Sie ein Gruppenrichtlinienobjekt in der Antworttext](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="6a3b2-128">If successful, this method returns `200 OK` response code and a [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="6a3b2-129">Wenn Unsucccessful...</span><span class="sxs-lookup"><span data-stu-id="6a3b2-129">If unsucccessful...</span></span>

## <a name="example"></a><span data-ttu-id="6a3b2-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a3b2-130">Example</span></span>
<span data-ttu-id="6a3b2-131">Das folgende Beispiel ruft eine bestimmte Richtlinie ab.</span><span class="sxs-lookup"><span data-stu-id="6a3b2-131">The following example retrieves a specific policy.</span></span>

##### <a name="request"></a><span data-ttu-id="6a3b2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a3b2-132">Request</span></span>
<span data-ttu-id="6a3b2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a3b2-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="6a3b2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a3b2-134">Response</span></span>
<span data-ttu-id="6a3b2-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a3b2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
    "id":"id-value",
    "alternativeIdentifier":null,
    "definition":["policy-definition"],
    "displayName":"name-value",
    "isOrganizationDefault":boolean-value,
    "keyCredentials":[key-credentials],
    "type":"type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
