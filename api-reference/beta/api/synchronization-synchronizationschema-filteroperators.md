---
title: 'SynchronizationSchema: FilterOperators'
description: Alle in den Gültigkeitsbereichen Filtern unterstützte Operatoren aufgelistet.
ms.openlocfilehash: 968abf6584868b2b0b5e664c59f14eebc780f151
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061329"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="35249-103">SynchronizationSchema: FilterOperators</span><span class="sxs-lookup"><span data-stu-id="35249-103">synchronizationSchema: filterOperators</span></span>

> <span data-ttu-id="35249-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="35249-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35249-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35249-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35249-106">Alle in den [Gültigkeitsbereichen Filter](../resources/synchronization-filter.md)unterstützte Operatoren aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="35249-106">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35249-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="35249-107">Permissions</span></span>
<span data-ttu-id="35249-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35249-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35249-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35249-110">Permission type</span></span>                        | <span data-ttu-id="35249-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35249-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="35249-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35249-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="35249-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35249-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="35249-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35249-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="35249-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35249-115">Not supported.</span></span>|
|<span data-ttu-id="35249-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35249-116">Application</span></span>                            |<span data-ttu-id="35249-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35249-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="35249-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35249-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="35249-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="35249-119">Request headers</span></span>

| <span data-ttu-id="35249-120">Name</span><span class="sxs-lookup"><span data-stu-id="35249-120">Name</span></span>           | <span data-ttu-id="35249-121">Typ</span><span class="sxs-lookup"><span data-stu-id="35249-121">Type</span></span>    | <span data-ttu-id="35249-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35249-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="35249-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35249-123">Authorization</span></span>  | <span data-ttu-id="35249-124">string</span><span class="sxs-lookup"><span data-stu-id="35249-124">string</span></span>  | <span data-ttu-id="35249-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="35249-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35249-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35249-127">Request body</span></span>

<span data-ttu-id="35249-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="35249-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35249-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="35249-129">Response</span></span>

<span data-ttu-id="35249-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200, OK` Antwortcode und ein [FilterOperatorSchema](../resources/synchronization-filteroperatorschema.md) -Auflistungsobjekt in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="35249-130">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35249-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="35249-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="35249-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35249-132">Request</span></span>
<span data-ttu-id="35249-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="35249-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="35249-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="35249-134">Response</span></span>
<span data-ttu-id="35249-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="35249-135">The following is an example of a response.</span></span>

><span data-ttu-id="35249-136">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="35249-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="35249-137">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35249-137">All the properties will be returned in an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->