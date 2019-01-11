---
title: Liste businessFlowTemplates
description: Öffnen Sie in Azure AD Bewertungen Feature, Sie alle BusinessFlowTemplate Objekte auflisten.
localization_priority: Normal
ms.openlocfilehash: 021a3c939c6642caf5200b5e9cc4e47b390019b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829498"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="3e491-103">Liste businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="3e491-103">List businessFlowTemplates</span></span>

> <span data-ttu-id="3e491-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3e491-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e491-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3e491-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e491-106">Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature Listen Sie aller [BusinessFlowTemplate](../resources/businessflowtemplate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="3e491-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e491-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3e491-107">Permissions</span></span>
<span data-ttu-id="3e491-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e491-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e491-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3e491-110">Permission type</span></span>                        | <span data-ttu-id="3e491-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3e491-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e491-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3e491-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e491-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="3e491-113"></span></span>  <span data-ttu-id="3e491-114">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Lesen von einer Überprüfung Zugriff zulässt.</span><span class="sxs-lookup"><span data-stu-id="3e491-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="3e491-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3e491-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e491-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e491-116">Not supported.</span></span> |
|<span data-ttu-id="3e491-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3e491-117">Application</span></span>                            | <span data-ttu-id="3e491-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3e491-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e491-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e491-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="3e491-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3e491-120">Request headers</span></span>
| <span data-ttu-id="3e491-121">Name</span><span class="sxs-lookup"><span data-stu-id="3e491-121">Name</span></span>         | <span data-ttu-id="3e491-122">Typ</span><span class="sxs-lookup"><span data-stu-id="3e491-122">Type</span></span>        | <span data-ttu-id="3e491-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e491-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3e491-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e491-124">Authorization</span></span> | <span data-ttu-id="3e491-125">string</span><span class="sxs-lookup"><span data-stu-id="3e491-125">string</span></span> | <span data-ttu-id="3e491-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="3e491-126">Bearer \{token\}.</span></span> <span data-ttu-id="3e491-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3e491-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e491-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3e491-128">Request body</span></span>
<span data-ttu-id="3e491-129">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="3e491-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="3e491-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e491-130">Response</span></span>
<span data-ttu-id="3e491-131">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [BusinessFlowTemplate](../resources/businessflowtemplate.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3e491-131">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e491-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3e491-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e491-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3e491-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="3e491-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3e491-134">Response</span></span>
><span data-ttu-id="3e491-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3e491-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlowTemplate",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Office 365 Groups' membership"
        } 
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="3e491-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="3e491-137">See also</span></span>

| <span data-ttu-id="3e491-138">Methode</span><span class="sxs-lookup"><span data-stu-id="3e491-138">Method</span></span>           | <span data-ttu-id="3e491-139">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3e491-139">Return Type</span></span>    |<span data-ttu-id="3e491-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3e491-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3e491-141">Erstellen von accessReview</span><span class="sxs-lookup"><span data-stu-id="3e491-141">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="3e491-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="3e491-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="3e491-143">Erstellen Sie eine neue AccessReview.</span><span class="sxs-lookup"><span data-stu-id="3e491-143">Create a new accessReview.</span></span> |




<!-- {
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
