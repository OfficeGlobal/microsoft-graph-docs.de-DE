---
title: Liste programControls
description: In Azure AD Access Feature überprüft, eine Liste aller der ProgramControl-Objekte in allen Programmen im Mandanten.
ms.openlocfilehash: 7e1dcb197a546e3aa823b731a9e7954803b36c2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059134"
---
# <a name="list-programcontrols"></a><span data-ttu-id="0a9b9-103">Liste programControls</span><span class="sxs-lookup"><span data-stu-id="0a9b9-103">List programControls</span></span>

> <span data-ttu-id="0a9b9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a9b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a9b9-106">Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature in allen Programmen im Mandanten Listen Sie aller [ProgramControl](../resources/programcontrol.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a9b9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0a9b9-107">Permissions</span></span>
<span data-ttu-id="0a9b9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a9b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a9b9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a9b9-110">Permission type</span></span>                        | <span data-ttu-id="0a9b9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a9b9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a9b9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a9b9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a9b9-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-113"></span></span>  <span data-ttu-id="0a9b9-114">Der angemeldeten Benutzer muss auch in ein Verzeichnis-Rolle sein, die diese zum Lesen von einem Programm zulässt.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="0a9b9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a9b9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a9b9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a9b9-116">Not supported.</span></span> |
|<span data-ttu-id="0a9b9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a9b9-117">Application</span></span>                            | <span data-ttu-id="0a9b9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a9b9-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a9b9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a9b9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="0a9b9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a9b9-120">Request headers</span></span>
| <span data-ttu-id="0a9b9-121">Name</span><span class="sxs-lookup"><span data-stu-id="0a9b9-121">Name</span></span>         | <span data-ttu-id="0a9b9-122">Typ</span><span class="sxs-lookup"><span data-stu-id="0a9b9-122">Type</span></span>        | <span data-ttu-id="0a9b9-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a9b9-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0a9b9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a9b9-124">Authorization</span></span> | <span data-ttu-id="0a9b9-125">string</span><span class="sxs-lookup"><span data-stu-id="0a9b9-125">string</span></span> | <span data-ttu-id="0a9b9-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-126">Bearer \{token\}.</span></span> <span data-ttu-id="0a9b9-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a9b9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a9b9-128">Request body</span></span>
<span data-ttu-id="0a9b9-129">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="0a9b9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a9b9-130">Response</span></span>
<span data-ttu-id="0a9b9-131">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [ProgramControl](../resources/programcontrol.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-131">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a9b9-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a9b9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a9b9-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a9b9-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a><span data-ttu-id="0a9b9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a9b9-134">Response</span></span>
><span data-ttu-id="0a9b9-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0a9b9-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0a9b9-137">See also</span></span>

| <span data-ttu-id="0a9b9-138">Methode</span><span class="sxs-lookup"><span data-stu-id="0a9b9-138">Method</span></span>           | <span data-ttu-id="0a9b9-139">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0a9b9-139">Return Type</span></span>    |<span data-ttu-id="0a9b9-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a9b9-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0a9b9-141">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="0a9b9-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="0a9b9-142">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0a9b9-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="0a9b9-143">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="0a9b9-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
