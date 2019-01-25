---
title: Liste programControls
description: In Azure AD Access Feature überprüft, eine Liste aller der ProgramControl-Objekte in allen Programmen im Mandanten.
localization_priority: Normal
ms.openlocfilehash: 52361e3878445d4f739fd0cd33817d5b254ddc03
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525059"
---
# <a name="list-programcontrols"></a><span data-ttu-id="9ba27-103">Liste programControls</span><span class="sxs-lookup"><span data-stu-id="9ba27-103">List programControls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ba27-104">Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature in allen Programmen im Mandanten Listen Sie aller [ProgramControl](../resources/programcontrol.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9ba27-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ba27-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9ba27-105">Permissions</span></span>
<span data-ttu-id="9ba27-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ba27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ba27-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ba27-108">Permission type</span></span>                        | <span data-ttu-id="9ba27-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ba27-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ba27-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ba27-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ba27-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="9ba27-111"></span></span>  <span data-ttu-id="9ba27-112">Der angemeldeten Benutzer muss auch in ein Verzeichnis-Rolle sein, die diese zum Lesen von einem Programm zulässt.</span><span class="sxs-lookup"><span data-stu-id="9ba27-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="9ba27-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ba27-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ba27-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ba27-114">Not supported.</span></span> |
|<span data-ttu-id="9ba27-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ba27-115">Application</span></span>                            | <span data-ttu-id="9ba27-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ba27-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ba27-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ba27-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="9ba27-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ba27-118">Request headers</span></span>
| <span data-ttu-id="9ba27-119">Name</span><span class="sxs-lookup"><span data-stu-id="9ba27-119">Name</span></span>         | <span data-ttu-id="9ba27-120">Typ</span><span class="sxs-lookup"><span data-stu-id="9ba27-120">Type</span></span>        | <span data-ttu-id="9ba27-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ba27-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9ba27-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ba27-122">Authorization</span></span> | <span data-ttu-id="9ba27-123">string</span><span class="sxs-lookup"><span data-stu-id="9ba27-123">string</span></span> | <span data-ttu-id="9ba27-124">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="9ba27-124">Bearer \{token\}.</span></span> <span data-ttu-id="9ba27-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9ba27-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ba27-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ba27-126">Request body</span></span>
<span data-ttu-id="9ba27-127">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="9ba27-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="9ba27-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ba27-128">Response</span></span>
<span data-ttu-id="9ba27-129">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [ProgramControl](../resources/programcontrol.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9ba27-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ba27-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ba27-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ba27-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ba27-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="9ba27-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ba27-132">Response</span></span>
><span data-ttu-id="9ba27-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9ba27-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{

    "value": [
        {
            "id": "f6abf8ef-a05e-4788-adc9-5af909c400af",
            "controlId": "bc81d51d-be53-4606-a8c2-f90a2beb5f40",
            "programId": "673a7379-9c38-4f01-bd9d-4fda7260b807",
            "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "guest user review",
            "status": "Completed",
            "createdDateTime": "2017-09-20T20:18:05.1318394Z"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="9ba27-135">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="9ba27-135">See also</span></span>

| <span data-ttu-id="9ba27-136">Methode</span><span class="sxs-lookup"><span data-stu-id="9ba27-136">Method</span></span>           | <span data-ttu-id="9ba27-137">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9ba27-137">Return Type</span></span>    |<span data-ttu-id="9ba27-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ba27-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ba27-139">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="9ba27-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="9ba27-140">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9ba27-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="9ba27-141">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="9ba27-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
