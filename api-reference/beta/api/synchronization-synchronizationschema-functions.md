---
title: 'SynchronizationSchema: Funktionen'
description: Listen Sie alle Funktionen, die derzeit in der AttributeMappingSource unterstützt.
localization_priority: Normal
ms.openlocfilehash: 5dc7734e9d747ac1e832aebb7d9c7355c2fbb52f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841007"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="f3130-103">SynchronizationSchema: Funktionen</span><span class="sxs-lookup"><span data-stu-id="f3130-103">synchronizationSchema: functions</span></span>

> <span data-ttu-id="f3130-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f3130-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3130-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3130-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3130-106">Listen Sie alle Funktionen, die derzeit in der [AttributeMappingSource](../resources/synchronization-attributemappingsource.md)unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3130-106">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f3130-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f3130-107">Permissions</span></span>
<span data-ttu-id="f3130-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3130-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3130-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3130-110">Permission type</span></span>                        | <span data-ttu-id="f3130-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3130-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3130-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3130-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="f3130-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3130-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f3130-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3130-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f3130-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3130-115">Not supported.</span></span>|
|<span data-ttu-id="f3130-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3130-116">Application</span></span>                            |<span data-ttu-id="f3130-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3130-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f3130-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3130-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="f3130-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3130-119">Request headers</span></span>

| <span data-ttu-id="f3130-120">Name</span><span class="sxs-lookup"><span data-stu-id="f3130-120">Name</span></span>           | <span data-ttu-id="f3130-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f3130-121">Type</span></span>    | <span data-ttu-id="f3130-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3130-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f3130-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3130-123">Authorization</span></span>  | <span data-ttu-id="f3130-124">string</span><span class="sxs-lookup"><span data-stu-id="f3130-124">string</span></span>  | <span data-ttu-id="f3130-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f3130-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3130-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3130-127">Request body</span></span>

<span data-ttu-id="f3130-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f3130-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3130-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3130-129">Response</span></span>

<span data-ttu-id="f3130-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AttributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) .</span><span class="sxs-lookup"><span data-stu-id="f3130-130">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3130-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3130-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f3130-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3130-132">Request</span></span>
<span data-ttu-id="f3130-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3130-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```

##### <a name="response"></a><span data-ttu-id="f3130-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3130-134">Response</span></span>
<span data-ttu-id="f3130-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="f3130-135">The following is an example of a response.</span></span>

><span data-ttu-id="f3130-136">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="f3130-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f3130-137">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3130-137">All the properties will be returned in an actual call.</span></span>

<!--
{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#functions",
    "value": [
        {
            "name": "Append",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "suffix",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "DefaultDomain",
            "parameters": []
        },
        {
            "name": "AppRoleAssignments",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "FormatDateTime",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "inputFormat",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "outputFormat",
                    "required": true,
                    "type": "String"
                }
            ]
        }
    ]
}
```

<!--
Below is the full response, which had to be redacted above as Markdown Scanner tool trips over "type" values containing 
non-string type names like "Integer" or "Boolean"

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#functions",
    "value": [
        {
            "name": "Append",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "suffix",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "DefaultDomain",
            "parameters": []
        },
        {
            "name": "AppRoleAssignments",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "FormatDateTime",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "inputFormat",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "outputFormat",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "IsNothing",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "Boolean"
                }
            ]
        },
        {
            "name": "Join",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "separator",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": true,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Prepend",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "prefix",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Mid",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "start",
                    "required": true,
                    "type": "Integer"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "length",
                    "required": true,
                    "type": "Integer"
                }
            ]
        },
        {
            "name": "Not",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "Boolean"
                }
            ]
        },
        {
            "name": "Replace",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Find",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "RegularExpression",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "RegularExpressionGroupName",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Replacement",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "ReplacementPropertyName",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Template",
                    "required": false,
                    "type": "String"
                }
            ]
        },
        {
            "name": "SingleAppRoleAssignment",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Split",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "delimiter",
                    "required": false,
                    "type": "String"
                }
            ]
        },
        {
            "name": "StripSpaces",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Switch",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "defaultValue",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": true,
                    "name": "switchValue",
                    "required": false,
                    "type": "String"
                }
            ]
        }
    ]
}

-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: functions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
