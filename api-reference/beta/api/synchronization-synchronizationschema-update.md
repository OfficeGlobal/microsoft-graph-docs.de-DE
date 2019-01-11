---
title: SynchronizationSchema aktualisieren
description: Aktualisieren Sie das Synchronisierungsschema für einen bestimmten Auftrag oder eine Vorlage. Diese Methode ersetzt das aktuelle Schema vollständig mit demjenigen, der in der Anforderung bereitgestellt. Um das Schema einer Vorlage zu aktualisieren, stellen Sie den Anruf auf das Application-Objekt. Sie müssen den Besitzer der Anwendung sein.
localization_priority: Normal
ms.openlocfilehash: d4f3f3540fe0d304b4edc3a5fcaec7b3366dbb0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826138"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="0b0cc-106">SynchronizationSchema aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0b0cc-106">Update synchronizationSchema</span></span>

> <span data-ttu-id="0b0cc-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b0cc-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b0cc-109">Aktualisieren Sie das Synchronisierungsschema für einen bestimmten Auftrag oder eine Vorlage.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-109">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="0b0cc-110">Diese Methode ersetzt das aktuelle Schema vollständig mit demjenigen, der in der Anforderung bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-110">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="0b0cc-111">Um das Schema einer Vorlage zu aktualisieren, stellen Sie den Anruf auf das Application-Objekt.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-111">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="0b0cc-112">Sie müssen den Besitzer der Anwendung sein.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-112">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b0cc-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0b0cc-113">Permissions</span></span>
<span data-ttu-id="0b0cc-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b0cc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b0cc-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b0cc-116">Permission type</span></span>                        | <span data-ttu-id="0b0cc-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b0cc-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b0cc-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b0cc-118">Delegated (work or school account)</span></span>     |<span data-ttu-id="0b0cc-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b0cc-119">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0b0cc-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b0cc-120">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0b0cc-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b0cc-121">Not supported.</span></span>|
|<span data-ttu-id="0b0cc-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b0cc-122">Application</span></span>                            |<span data-ttu-id="0b0cc-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b0cc-123">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="0b0cc-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b0cc-124">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="0b0cc-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b0cc-125">Request headers</span></span>

| <span data-ttu-id="0b0cc-126">Name</span><span class="sxs-lookup"><span data-stu-id="0b0cc-126">Name</span></span>           | <span data-ttu-id="0b0cc-127">Typ</span><span class="sxs-lookup"><span data-stu-id="0b0cc-127">Type</span></span>    | <span data-ttu-id="0b0cc-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b0cc-128">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0b0cc-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b0cc-129">Authorization</span></span>  | <span data-ttu-id="0b0cc-130">string</span><span class="sxs-lookup"><span data-stu-id="0b0cc-130">string</span></span>  | <span data-ttu-id="0b0cc-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b0cc-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b0cc-133">Request body</span></span>

<span data-ttu-id="0b0cc-134">Geben Sie im Textkörper Anforderung das [SynchronizationSchema](../resources/synchronization-synchronizationschema.md) -Objekt, um das vorhandene Schema zu ersetzen.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-134">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="0b0cc-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b0cc-135">Response</span></span>

<span data-ttu-id="0b0cc-136">Bei erfolgreicher gibt eine `204 No Content` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-136">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="0b0cc-137">Es gibt keine Suchzeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b0cc-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b0cc-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0b0cc-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b0cc-139">Request</span></span>
<span data-ttu-id="0b0cc-140">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-140">The following is an example of a request.</span></span>

><span data-ttu-id="0b0cc-141">**Hinweis:** Das hier gezeigte Request-Objekt wird zur besseren Lesbarkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-141">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="0b0cc-142">Geben Sie alle Eigenschaften in eine tatsächliche aufrufen.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-142">Supply all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0b0cc-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b0cc-143">Response</span></span>
<span data-ttu-id="0b0cc-144">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="0b0cc-144">The following is an example of a response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
