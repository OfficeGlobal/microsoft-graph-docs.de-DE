---
title: 'SynchronizationSchema: ParseExpression'
description: '(.. / resources/synchronization_attributemappingsource.md) Objekt. '
localization_priority: Normal
ms.openlocfilehash: 27545333c6ff7b3c9ffde3e1c59abd09465db1c2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522966"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="b110d-103">SynchronizationSchema: ParseExpression</span><span class="sxs-lookup"><span data-stu-id="b110d-103">synchronizationSchema: parseExpression</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b110d-104">Analysieren einer gegebenen Zeichenfolgenausdruck in einem [AttributeMappingSource | (... / resources/synchronization_attributemappingsource.md) Objekt.</span><span class="sxs-lookup"><span data-stu-id="b110d-104">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="b110d-105">Weitere Informationen zu Ausdrücken finden Sie unter [Writing Ausdrücke für Attribut Zuordnungen in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="b110d-105">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="b110d-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b110d-106">Permissions</span></span>
<span data-ttu-id="b110d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b110d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b110d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b110d-109">Permission type</span></span>                        | <span data-ttu-id="b110d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b110d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b110d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b110d-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="b110d-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b110d-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b110d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b110d-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b110d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b110d-114">Not supported.</span></span>|
|<span data-ttu-id="b110d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b110d-115">Application</span></span>                            |<span data-ttu-id="b110d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b110d-116">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="b110d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b110d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="b110d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b110d-118">Request headers</span></span>
| <span data-ttu-id="b110d-119">Name</span><span class="sxs-lookup"><span data-stu-id="b110d-119">Name</span></span>       | <span data-ttu-id="b110d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b110d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b110d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b110d-121">Authorization</span></span>  | <span data-ttu-id="b110d-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b110d-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b110d-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b110d-123">Request body</span></span>
<span data-ttu-id="b110d-124">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b110d-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b110d-125">Parameter</span><span class="sxs-lookup"><span data-stu-id="b110d-125">Parameter</span></span>    | <span data-ttu-id="b110d-126">Typ</span><span class="sxs-lookup"><span data-stu-id="b110d-126">Type</span></span>   |<span data-ttu-id="b110d-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b110d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b110d-128">Ausdruck</span><span class="sxs-lookup"><span data-stu-id="b110d-128">expression</span></span>               |<span data-ttu-id="b110d-129">String</span><span class="sxs-lookup"><span data-stu-id="b110d-129">String</span></span>               |<span data-ttu-id="b110d-130">Ausdruck zu analysieren.</span><span class="sxs-lookup"><span data-stu-id="b110d-130">Expression to parse.</span></span>|
|<span data-ttu-id="b110d-131">testInputObject</span><span class="sxs-lookup"><span data-stu-id="b110d-131">testInputObject</span></span>          |[<span data-ttu-id="b110d-132">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="b110d-132">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="b110d-133">Testen Sie Datenobjekt für gegen Ausdruck ausgewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b110d-133">Test data object to evaluate expression against.</span></span> <span data-ttu-id="b110d-134">Optional.</span><span class="sxs-lookup"><span data-stu-id="b110d-134">Optional.</span></span>|
|<span data-ttu-id="b110d-135">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="b110d-135">targetAttributeDefinition</span></span>|[<span data-ttu-id="b110d-136">Attributdefinition</span><span class="sxs-lookup"><span data-stu-id="b110d-136">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="b110d-137">Definition des Attributs, das dieser Ausdruck zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="b110d-137">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="b110d-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="b110d-138">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="b110d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b110d-139">Response</span></span>
<span data-ttu-id="b110d-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [ParseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b110d-140">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b110d-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b110d-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b110d-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b110d-142">Request</span></span>
<span data-ttu-id="b110d-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b110d-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_parseexpression"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
Content-type: application/json

{
    "expression":"Replace([preferredLanguage], \"-\", , , \"_\", ,  )",
    "targetAttributeDefinition":null,
    "testInputObject": {
        definition: null,
        properties:[
            { key: "objectId", value : "66E4A8CC-1B7B-435E-95F8-F06CEA133828" },
            { key: "IsSoftDeleted", value: "false"},
            { key: "accountEnabled", value: "true"},
            { key: "streetAddress", value: "1 Redmond Way"},
            { key: "city", value: "Redmond"},
            { key: "state", value: "WA"},
            { key: "postalCode", value: "98052"},
            { key: "country", value: "USA"},
            { key: "department", value: "Sales"},
            { key: "displayName", value: "John Smith"},
            { key: "extensionAttribute1", value: "Sample 1"},
            { key: "extensionAttribute2", value: "Sample 2"},
            { key: "extensionAttribute3", value: "Sample 3"},
            { key: "extensionAttribute4", value: "Sample 4"},
            { key: "extensionAttribute5", value: "Sample 5"},
            { key: "extensionAttribute6", value: "Sample 6"},
            { key: "extensionAttribute7", value: "Sample 1"},
            { key: "extensionAttribute8", value: "Sample 1"},
            { key: "extensionAttribute9", value: "Sample 1"},
            { key: "extensionAttribute10", value: "Sample 1"},
            { key: "extensionAttribute11", value: "Sample 1"},
            { key: "extensionAttribute12", value: "Sample 1"},
            { key: "extensionAttribute13", value: "Sample 1"},
            { key: "extensionAttribute14", value: "Sample 1"},
            { key: "extensionAttribute15", value: "Sample 1"},
            { key: "givenName", value: "John"},
            { key: "jobTitle", value: "Finance manager"},
            { key: "mail", value: "johns@contoso.com"},
            { key: "mailNickname", value: "johns"},
            { key: "manager", value: "maxs@contoso.com"},
            { key: "mobile", value: "425-555-0010"},
            { key: "onPremisesSecurityIdentifier", value: "66E4A8CC-1B7B-435E-95F8-F06CEA133828"},
            { key: "passwordProfile.password", value: ""},
            { key: "physicalDeliveryOfficeName", value: "Main Office"},
            { key: "preferredLanguage", value: "EN-US"},
            { key: "proxyAddresses", value: ""},
            { key: "surname", value: "Smith"},
            { key: "telephoneNumber", value: "425-555-0011"},
            { key: "userPrincipalName", value: "johns@contoso.com"},
            { key: "appRoleAssignments", "value@odata.type":"#Collection(String)", value: ["Default Assignment"] }
        ]
    }
}
```

##### <a name="response"></a><span data-ttu-id="b110d-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b110d-144">Response</span></span>
<span data-ttu-id="b110d-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b110d-145">The following is an example of the response.</span></span> 

><span data-ttu-id="b110d-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b110d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.parseExpressionResponse"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "error": null,
    "evaluationSucceeded": true,
    "evaluationResult": [
        "EN_US"
    ],
    "parsedExpression": {
        "expression": "Replace([preferredLanguage], \"-\", , , \"_\", , )",
        "name": "Replace",
        "parameters": [
            {
                "key": "source",
                "value": {
                    "expression": "[preferredLanguage]",
                    "name": "preferredLanguage",
                    "parameters": [],
                    "type": "Attribute"
                }
            },
            {
                "key": "Find",
                "value": {
                    "expression": "\"-\"",
                    "name": "-",
                    "parameters": [],
                    "type": "Constant"
                }
            },
            {
                "key": "Replacement",
                "value": {
                    "expression": "\"_\"",
                    "name": "_",
                    "parameters": [],
                    "type": "Constant"
                }
            }
        ],
        "type": "Function"
    },
    "parsingSucceeded": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-parseexpression.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
