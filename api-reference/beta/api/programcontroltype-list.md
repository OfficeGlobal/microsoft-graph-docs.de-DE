---
title: Liste programControlTypes
description: Öffnen Sie in Azure AD Bewertungen Feature, Sie alle ProgramControlType Objekte auflisten.
localization_priority: Normal
ms.openlocfilehash: 00983cadf4bd1e0cf136c594f06ac3ee6fbb1de5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515692"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="b34b1-103">Liste programControlTypes</span><span class="sxs-lookup"><span data-stu-id="b34b1-103">List programControlTypes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b34b1-104">Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature Listen Sie aller [ProgramControlType](../resources/programcontroltype.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b34b1-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b34b1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b34b1-105">Permissions</span></span>
<span data-ttu-id="b34b1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b34b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b34b1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b34b1-108">Permission type</span></span>                        | <span data-ttu-id="b34b1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b34b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b34b1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b34b1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b34b1-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="b34b1-111"></span></span>  <span data-ttu-id="b34b1-112">Der angemeldeten Benutzer muss auch in ein Verzeichnis-Rolle sein, die diese zum Lesen von einem Programm zulässt.</span><span class="sxs-lookup"><span data-stu-id="b34b1-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="b34b1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b34b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b34b1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b34b1-114">Not supported.</span></span> |
|<span data-ttu-id="b34b1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b34b1-115">Application</span></span>                            | <span data-ttu-id="b34b1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b34b1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b34b1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b34b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="b34b1-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b34b1-118">Request headers</span></span>
| <span data-ttu-id="b34b1-119">Name</span><span class="sxs-lookup"><span data-stu-id="b34b1-119">Name</span></span>         | <span data-ttu-id="b34b1-120">Typ</span><span class="sxs-lookup"><span data-stu-id="b34b1-120">Type</span></span>        | <span data-ttu-id="b34b1-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b34b1-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b34b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b34b1-122">Authorization</span></span> | <span data-ttu-id="b34b1-123">string</span><span class="sxs-lookup"><span data-stu-id="b34b1-123">string</span></span> | <span data-ttu-id="b34b1-124">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="b34b1-124">Bearer \{token\}.</span></span> <span data-ttu-id="b34b1-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b34b1-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b34b1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b34b1-126">Request body</span></span>
<span data-ttu-id="b34b1-127">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="b34b1-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="b34b1-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b34b1-128">Response</span></span>
<span data-ttu-id="b34b1-129">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [ProgramControlType](../resources/programcontroltype.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b34b1-129">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b34b1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b34b1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b34b1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b34b1-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="b34b1-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b34b1-132">Response</span></span>
><span data-ttu-id="b34b1-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b34b1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControlType",
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

## <a name="see-also"></a><span data-ttu-id="b34b1-135">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="b34b1-135">See also</span></span>

| <span data-ttu-id="b34b1-136">Methode</span><span class="sxs-lookup"><span data-stu-id="b34b1-136">Method</span></span>           | <span data-ttu-id="b34b1-137">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b34b1-137">Return Type</span></span>    |<span data-ttu-id="b34b1-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b34b1-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b34b1-139">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="b34b1-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="b34b1-140">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b34b1-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="b34b1-141">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="b34b1-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
