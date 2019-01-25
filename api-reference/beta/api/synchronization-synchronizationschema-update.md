---
title: SynchronizationSchema aktualisieren
description: Aktualisieren Sie das Synchronisierungsschema für einen bestimmten Auftrag oder eine Vorlage. Diese Methode ersetzt das aktuelle Schema vollständig mit demjenigen, der in der Anforderung bereitgestellt. Um das Schema einer Vorlage zu aktualisieren, stellen Sie den Anruf auf das Application-Objekt. Sie müssen den Besitzer der Anwendung sein.
localization_priority: Normal
ms.openlocfilehash: 13ee7d996b0e02834b77cd222380747c02d7fcc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525549"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="2cc61-106">SynchronizationSchema aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2cc61-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cc61-107">Aktualisieren Sie das Synchronisierungsschema für einen bestimmten Auftrag oder eine Vorlage.</span><span class="sxs-lookup"><span data-stu-id="2cc61-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="2cc61-108">Diese Methode ersetzt das aktuelle Schema vollständig mit demjenigen, der in der Anforderung bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="2cc61-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="2cc61-109">Um das Schema einer Vorlage zu aktualisieren, stellen Sie den Anruf auf das Application-Objekt.</span><span class="sxs-lookup"><span data-stu-id="2cc61-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="2cc61-110">Sie müssen den Besitzer der Anwendung sein.</span><span class="sxs-lookup"><span data-stu-id="2cc61-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cc61-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2cc61-111">Permissions</span></span>
<span data-ttu-id="2cc61-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cc61-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cc61-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2cc61-114">Permission type</span></span>                        | <span data-ttu-id="2cc61-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2cc61-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cc61-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2cc61-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="2cc61-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc61-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2cc61-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2cc61-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2cc61-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2cc61-119">Not supported.</span></span>|
|<span data-ttu-id="2cc61-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2cc61-120">Application</span></span>                            |<span data-ttu-id="2cc61-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2cc61-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="2cc61-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2cc61-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="2cc61-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2cc61-123">Request headers</span></span>

| <span data-ttu-id="2cc61-124">Name</span><span class="sxs-lookup"><span data-stu-id="2cc61-124">Name</span></span>           | <span data-ttu-id="2cc61-125">Typ</span><span class="sxs-lookup"><span data-stu-id="2cc61-125">Type</span></span>    | <span data-ttu-id="2cc61-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2cc61-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="2cc61-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cc61-127">Authorization</span></span>  | <span data-ttu-id="2cc61-128">string</span><span class="sxs-lookup"><span data-stu-id="2cc61-128">string</span></span>  | <span data-ttu-id="2cc61-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2cc61-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cc61-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2cc61-131">Request body</span></span>

<span data-ttu-id="2cc61-132">Geben Sie im Textkörper Anforderung das [SynchronizationSchema](../resources/synchronization-synchronizationschema.md) -Objekt, um das vorhandene Schema zu ersetzen.</span><span class="sxs-lookup"><span data-stu-id="2cc61-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="2cc61-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2cc61-133">Response</span></span>

<span data-ttu-id="2cc61-134">Bei erfolgreicher gibt eine `204 No Content` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="2cc61-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="2cc61-135">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2cc61-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cc61-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2cc61-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2cc61-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2cc61-137">Request</span></span>
<span data-ttu-id="2cc61-138">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2cc61-138">The following is an example of a request.</span></span>

><span data-ttu-id="2cc61-139">**Hinweis:** Das hier gezeigte Request-Objekt wird zur besseren Lesbarkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="2cc61-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="2cc61-140">Geben Sie alle Eigenschaften in eine tatsächliche aufrufen.</span><span class="sxs-lookup"><span data-stu-id="2cc61-140">Supply all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema

{
    "directories": [
        {
            "name": "Azure Active Directory",
            "objects": [
                {
                    "name": "User",
                    "attributes": [
                        {
                            "name": "userPrincipalName",
                            "type": "string"
                        }
                    ]
                },
            ]
        },
        {
            "name": "Salesforce",
        }
    ],
    "synchronizationRules":[
        {
            "name": "USER_TO_USER",
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "Salesforce",
            "objectMappings": [
                {
                    "sourceObjectName": "User",
                    "targetObjectName": "User",
                    "attributeMappings": [
                        {
                            "source": {},
                            "targetAttributeName": "userName"
                        },
                    ]
                },
            ]
        },
    ]
}

```

##### <a name="response"></a><span data-ttu-id="2cc61-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2cc61-141">Response</span></span>
<span data-ttu-id="2cc61-142">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="2cc61-142">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
