---
title: Abrufen von synchronizationSchema
description: Rufen Sie das Schema für einen bestimmten Synchronisierungsauftrag oder eine Vorlage.
ms.openlocfilehash: 93624a334c928b6402851ebc566e6e29e341ca1b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059736"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="79142-103">Abrufen von synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="79142-103">Get synchronizationSchema</span></span>

> <span data-ttu-id="79142-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="79142-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79142-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79142-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79142-106">Rufen Sie das Schema für einen bestimmten Synchronisierungsauftrag oder eine Vorlage.</span><span class="sxs-lookup"><span data-stu-id="79142-106">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="79142-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="79142-107">Permissions</span></span>
<span data-ttu-id="79142-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79142-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79142-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="79142-110">Permission type</span></span>                        | <span data-ttu-id="79142-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="79142-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="79142-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="79142-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="79142-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79142-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="79142-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="79142-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="79142-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79142-115">Not supported.</span></span> |
|<span data-ttu-id="79142-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="79142-116">Application</span></span>                            |<span data-ttu-id="79142-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="79142-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="79142-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="79142-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="79142-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="79142-119">Request headers</span></span>

| <span data-ttu-id="79142-120">Name</span><span class="sxs-lookup"><span data-stu-id="79142-120">Name</span></span>           | <span data-ttu-id="79142-121">Typ</span><span class="sxs-lookup"><span data-stu-id="79142-121">Type</span></span>    | <span data-ttu-id="79142-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79142-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="79142-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79142-123">Authorization</span></span>  | <span data-ttu-id="79142-124">string</span><span class="sxs-lookup"><span data-stu-id="79142-124">string</span></span>  | <span data-ttu-id="79142-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="79142-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79142-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="79142-127">Request body</span></span>

<span data-ttu-id="79142-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="79142-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79142-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="79142-129">Response</span></span>

<span data-ttu-id="79142-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [SynchronizationSchema](../resources/synchronization-synchronizationschema.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="79142-130">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79142-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="79142-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="79142-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="79142-132">Request</span></span>
<span data-ttu-id="79142-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="79142-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="79142-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="79142-134">Response</span></span>
<span data-ttu-id="79142-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="79142-135">The following is an example of a response.</span></span>

><span data-ttu-id="79142-136">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="79142-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="79142-137">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="79142-137">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

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
                }
            ]
        },
        {
            "name": "Salesforce",
            "objects": [{}]
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
                        {}
                    ]
                },
                {}
            ]
        },
        {}
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->