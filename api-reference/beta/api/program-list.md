---
title: Programme auflisten
description: Zugriff auf in Azure AD Bewertungen Feature, listet alle Programmobjekte.
localization_priority: Normal
ms.openlocfilehash: 71073f2469087e92b43823e89881406fb17a666b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526977"
---
# <a name="list-programs"></a><span data-ttu-id="4ccc7-103">Programme auflisten</span><span class="sxs-lookup"><span data-stu-id="4ccc7-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ccc7-104">Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature Listen Sie aller [Programm](../resources/program.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="4ccc7-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ccc7-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4ccc7-105">Permissions</span></span>
<span data-ttu-id="4ccc7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ccc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ccc7-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ccc7-108">Permission type</span></span>                        | <span data-ttu-id="4ccc7-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ccc7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ccc7-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ccc7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ccc7-111">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="4ccc7-111"></span></span>  <span data-ttu-id="4ccc7-112">Der angemeldeten Benutzer muss auch in ein Verzeichnis-Rolle sein, die diese zum Lesen von einem Programm zulässt.</span><span class="sxs-lookup"><span data-stu-id="4ccc7-112">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="4ccc7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ccc7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ccc7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ccc7-114">Not supported.</span></span> |
|<span data-ttu-id="4ccc7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ccc7-115">Application</span></span>                            | <span data-ttu-id="4ccc7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ccc7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ccc7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ccc7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="4ccc7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ccc7-118">Request headers</span></span>
| <span data-ttu-id="4ccc7-119">Name</span><span class="sxs-lookup"><span data-stu-id="4ccc7-119">Name</span></span>         | <span data-ttu-id="4ccc7-120">Typ</span><span class="sxs-lookup"><span data-stu-id="4ccc7-120">Type</span></span>        | <span data-ttu-id="4ccc7-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ccc7-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4ccc7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ccc7-122">Authorization</span></span> | <span data-ttu-id="4ccc7-123">string</span><span class="sxs-lookup"><span data-stu-id="4ccc7-123">string</span></span> | <span data-ttu-id="4ccc7-124">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="4ccc7-124">Bearer \{token\}.</span></span> <span data-ttu-id="4ccc7-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4ccc7-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ccc7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ccc7-126">Request body</span></span>
<span data-ttu-id="4ccc7-127">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="4ccc7-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="4ccc7-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ccc7-128">Response</span></span>
<span data-ttu-id="4ccc7-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200, OK` Antwortcode und ein Array von Objekten im Antworttext [Programm](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="4ccc7-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ccc7-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ccc7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ccc7-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ccc7-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="4ccc7-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ccc7-132">Response</span></span>
><span data-ttu-id="4ccc7-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4ccc7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
            "displayName": "testprogram3",
            "description": "test description"
        },
        {
            "id": "b4afdd74-b6cf-4239-9b08-dde9a91d18d2",
            "displayName": "Default Program",
            "description": "Built-in program to start managing access reviews"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="4ccc7-135">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="4ccc7-135">See also</span></span>

| <span data-ttu-id="4ccc7-136">Methode</span><span class="sxs-lookup"><span data-stu-id="4ccc7-136">Method</span></span>           | <span data-ttu-id="4ccc7-137">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4ccc7-137">Return Type</span></span>    |<span data-ttu-id="4ccc7-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ccc7-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ccc7-139">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="4ccc7-139">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="4ccc7-140">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4ccc7-140">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="4ccc7-141">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="4ccc7-141">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
