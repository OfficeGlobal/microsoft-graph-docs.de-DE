---
title: 'SynchronizationSchema: ParseExpression'
description: '(.. / resources/synchronization_attributemappingsource.md) Objekt. '
localization_priority: Normal
ms.openlocfilehash: dbde03b9ae85377801ad894c8b8ca22c6baebc85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811025"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="ea285-103">SynchronizationSchema: ParseExpression</span><span class="sxs-lookup"><span data-stu-id="ea285-103">synchronizationSchema: parseExpression</span></span>

> <span data-ttu-id="ea285-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ea285-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea285-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea285-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ea285-106">Analysieren einer gegebenen Zeichenfolgenausdruck in einem [AttributeMappingSource | (... / resources/synchronization_attributemappingsource.md) Objekt.</span><span class="sxs-lookup"><span data-stu-id="ea285-106">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="ea285-107">Weitere Informationen zu Ausdrücken finden Sie unter [Writing Ausdrücke für Attribut Zuordnungen in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="ea285-107">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea285-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ea285-108">Permissions</span></span>
<span data-ttu-id="ea285-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea285-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea285-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ea285-111">Permission type</span></span>                        | <span data-ttu-id="ea285-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ea285-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea285-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ea285-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="ea285-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea285-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ea285-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ea285-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ea285-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea285-116">Not supported.</span></span>|
|<span data-ttu-id="ea285-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ea285-117">Application</span></span>                            |<span data-ttu-id="ea285-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ea285-118">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="ea285-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea285-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="ea285-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ea285-120">Request headers</span></span>
| <span data-ttu-id="ea285-121">Name</span><span class="sxs-lookup"><span data-stu-id="ea285-121">Name</span></span>       | <span data-ttu-id="ea285-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea285-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ea285-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea285-123">Authorization</span></span>  | <span data-ttu-id="ea285-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ea285-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea285-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ea285-125">Request body</span></span>
<span data-ttu-id="ea285-126">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="ea285-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ea285-127">Parameter</span><span class="sxs-lookup"><span data-stu-id="ea285-127">Parameter</span></span>    | <span data-ttu-id="ea285-128">Typ</span><span class="sxs-lookup"><span data-stu-id="ea285-128">Type</span></span>   |<span data-ttu-id="ea285-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea285-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea285-130">Ausdruck</span><span class="sxs-lookup"><span data-stu-id="ea285-130">expression</span></span>               |<span data-ttu-id="ea285-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea285-131">String</span></span>               |<span data-ttu-id="ea285-132">Ausdruck zu analysieren.</span><span class="sxs-lookup"><span data-stu-id="ea285-132">Expression to parse.</span></span>|
|<span data-ttu-id="ea285-133">testInputObject</span><span class="sxs-lookup"><span data-stu-id="ea285-133">testInputObject</span></span>          |[<span data-ttu-id="ea285-134">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="ea285-134">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="ea285-135">Testen Sie Datenobjekt für gegen Ausdruck ausgewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ea285-135">Test data object to evaluate expression against.</span></span> <span data-ttu-id="ea285-136">Optional.</span><span class="sxs-lookup"><span data-stu-id="ea285-136">Optional.</span></span>|
|<span data-ttu-id="ea285-137">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="ea285-137">targetAttributeDefinition</span></span>|[<span data-ttu-id="ea285-138">Attributdefinition</span><span class="sxs-lookup"><span data-stu-id="ea285-138">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="ea285-139">Definition des Attributs, das dieser Ausdruck zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="ea285-139">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="ea285-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="ea285-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="ea285-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea285-141">Response</span></span>
<span data-ttu-id="ea285-142">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [ParseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ea285-142">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea285-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ea285-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ea285-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ea285-144">Request</span></span>
<span data-ttu-id="ea285-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ea285-145">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ea285-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="ea285-146">Response</span></span>
<span data-ttu-id="ea285-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ea285-147">The following is an example of the response.</span></span> 

><span data-ttu-id="ea285-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ea285-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
