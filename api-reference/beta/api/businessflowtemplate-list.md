---
title: Liste businessFlowTemplates
description: Öffnen Sie in Azure AD Bewertungen Feature, Sie alle BusinessFlowTemplate Objekte auflisten.
localization_priority: Normal
ms.openlocfilehash: 5b1d96330f808600c7f306ca85009bc5948a22f4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525563"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="7b7ff-103">Liste businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="7b7ff-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b7ff-104">Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature Listen Sie aller [BusinessFlowTemplate](../resources/businessflowtemplate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="7b7ff-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7b7ff-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7b7ff-105">Permissions</span></span>
<span data-ttu-id="7b7ff-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b7ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b7ff-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b7ff-108">Permission type</span></span>                        | <span data-ttu-id="7b7ff-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b7ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b7ff-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b7ff-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b7ff-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="7b7ff-111"></span></span>  <span data-ttu-id="7b7ff-112">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Lesen von einer Überprüfung Zugriff zulässt.</span><span class="sxs-lookup"><span data-stu-id="7b7ff-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="7b7ff-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b7ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b7ff-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b7ff-114">Not supported.</span></span> |
|<span data-ttu-id="7b7ff-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b7ff-115">Application</span></span>                            | <span data-ttu-id="7b7ff-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b7ff-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b7ff-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b7ff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="7b7ff-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b7ff-118">Request headers</span></span>
| <span data-ttu-id="7b7ff-119">Name</span><span class="sxs-lookup"><span data-stu-id="7b7ff-119">Name</span></span>         | <span data-ttu-id="7b7ff-120">Typ</span><span class="sxs-lookup"><span data-stu-id="7b7ff-120">Type</span></span>        | <span data-ttu-id="7b7ff-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b7ff-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7b7ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b7ff-122">Authorization</span></span> | <span data-ttu-id="7b7ff-123">string</span><span class="sxs-lookup"><span data-stu-id="7b7ff-123">string</span></span> | <span data-ttu-id="7b7ff-124">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="7b7ff-124">Bearer \{token\}.</span></span> <span data-ttu-id="7b7ff-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7b7ff-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b7ff-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b7ff-126">Request body</span></span>
<span data-ttu-id="7b7ff-127">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="7b7ff-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="7b7ff-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b7ff-128">Response</span></span>
<span data-ttu-id="7b7ff-129">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [BusinessFlowTemplate](../resources/businessflowtemplate.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7b7ff-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b7ff-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b7ff-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b7ff-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b7ff-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_businesFlowTemplate"
}-->
```http
GET https://graph.microsoft.com/beta/businesFlowTemplates
```

##### <a name="response"></a><span data-ttu-id="7b7ff-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b7ff-132">Response</span></span>
><span data-ttu-id="7b7ff-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7b7ff-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7b7ff-135">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7b7ff-135">See also</span></span>

| <span data-ttu-id="7b7ff-136">Methode</span><span class="sxs-lookup"><span data-stu-id="7b7ff-136">Method</span></span>           | <span data-ttu-id="7b7ff-137">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7b7ff-137">Return Type</span></span>    |<span data-ttu-id="7b7ff-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b7ff-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b7ff-139">Erstellen von accessReview</span><span class="sxs-lookup"><span data-stu-id="7b7ff-139">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="7b7ff-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="7b7ff-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="7b7ff-141">Erstellen Sie eine neue AccessReview.</span><span class="sxs-lookup"><span data-stu-id="7b7ff-141">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/businessflowtemplate-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
