---
title: 'SynchronizationSchema: FilterOperators'
description: Alle in den Gültigkeitsbereichen Filtern unterstützte Operatoren aufgelistet.
localization_priority: Normal
ms.openlocfilehash: 68e0c9f583e92989213d1442aee1610b1495bae0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641708"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="fbcef-103">SynchronizationSchema: FilterOperators</span><span class="sxs-lookup"><span data-stu-id="fbcef-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbcef-104">Alle in den [Gültigkeitsbereichen Filter](../resources/synchronization-filter.md)unterstützte Operatoren aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="fbcef-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fbcef-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fbcef-105">Permissions</span></span>
<span data-ttu-id="fbcef-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbcef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbcef-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fbcef-108">Permission type</span></span>                        | <span data-ttu-id="fbcef-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fbcef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbcef-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fbcef-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="fbcef-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbcef-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="fbcef-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fbcef-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="fbcef-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbcef-113">Not supported.</span></span>|
|<span data-ttu-id="fbcef-114">Application</span><span class="sxs-lookup"><span data-stu-id="fbcef-114">Application</span></span>                            |<span data-ttu-id="fbcef-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbcef-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fbcef-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbcef-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="fbcef-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fbcef-117">Request headers</span></span>

| <span data-ttu-id="fbcef-118">Name</span><span class="sxs-lookup"><span data-stu-id="fbcef-118">Name</span></span>           | <span data-ttu-id="fbcef-119">Typ</span><span class="sxs-lookup"><span data-stu-id="fbcef-119">Type</span></span>    | <span data-ttu-id="fbcef-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fbcef-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="fbcef-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fbcef-121">Authorization</span></span>  | <span data-ttu-id="fbcef-122">string</span><span class="sxs-lookup"><span data-stu-id="fbcef-122">string</span></span>  | <span data-ttu-id="fbcef-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fbcef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbcef-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fbcef-125">Request body</span></span>

<span data-ttu-id="fbcef-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fbcef-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbcef-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbcef-127">Response</span></span>

<span data-ttu-id="fbcef-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200, OK` Antwortcode und ein [FilterOperatorSchema](../resources/synchronization-filteroperatorschema.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fbcef-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbcef-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fbcef-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fbcef-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbcef-130">Request</span></span>
<span data-ttu-id="fbcef-131">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fbcef-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="fbcef-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbcef-132">Response</span></span>
<span data-ttu-id="fbcef-133">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="fbcef-133">The following is an example of a response.</span></span>

><span data-ttu-id="fbcef-134">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="fbcef-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fbcef-135">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fbcef-135">All the properties will be returned in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.filterOperatorSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "name": "EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "String",
                "Integer"
            ]
        }
    ]
}
```
<!--
Below is the full response, which had to be redacted above as Markdown Scanner tool trips over "type" values containing 
non-string type names like "Integer" or "Boolean"

{
    "value": [
        {
            "name": "EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "IS FALSE",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "IS NOT NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String",
                "Binary",
                "Boolean"
            ]
        },
        {
            "name": "IS NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String",
                "Binary",
                "Boolean"
            ]
        },
        {
            "name": "IS TRUE",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "NOT EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "NOT REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        }
    ]
}
-->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-filteroperators.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
