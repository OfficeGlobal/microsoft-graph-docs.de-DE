---
title: Liste ProgramControls eines Programms
description: In Azure AD Access Feature überprüft, eine Liste aller ProgramControl Objekte für ein bestimmtes Programm verknüpft.
localization_priority: Normal
ms.openlocfilehash: 8895634b098474cdbeab695cbe730a1e2fd02e2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809335"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="385d2-103">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="385d2-103">List programControls of a program</span></span>

> <span data-ttu-id="385d2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="385d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="385d2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="385d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="385d2-106">Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature Listen Sie aller [ProgramControl](../resources/programcontrol.md) -Objekte, um ein bestimmtes Programm verknüpft.</span><span class="sxs-lookup"><span data-stu-id="385d2-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="385d2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="385d2-107">Permissions</span></span>
<span data-ttu-id="385d2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="385d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="385d2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="385d2-110">Permission type</span></span>                        | <span data-ttu-id="385d2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="385d2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="385d2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="385d2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="385d2-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="385d2-113"></span></span>  <span data-ttu-id="385d2-114">Der angemeldeten Benutzer muss auch in ein Verzeichnis-Rolle sein, die diese zum Lesen von einem Programm zulässt.</span><span class="sxs-lookup"><span data-stu-id="385d2-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="385d2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="385d2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="385d2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="385d2-116">Not supported.</span></span> |
|<span data-ttu-id="385d2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="385d2-117">Application</span></span>                            | <span data-ttu-id="385d2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="385d2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="385d2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="385d2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="385d2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="385d2-120">Request headers</span></span>
| <span data-ttu-id="385d2-121">Name</span><span class="sxs-lookup"><span data-stu-id="385d2-121">Name</span></span>         | <span data-ttu-id="385d2-122">Typ</span><span class="sxs-lookup"><span data-stu-id="385d2-122">Type</span></span>        | <span data-ttu-id="385d2-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="385d2-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="385d2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="385d2-124">Authorization</span></span> | <span data-ttu-id="385d2-125">string</span><span class="sxs-lookup"><span data-stu-id="385d2-125">string</span></span> | <span data-ttu-id="385d2-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="385d2-126">Bearer \{token\}.</span></span> <span data-ttu-id="385d2-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="385d2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="385d2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="385d2-128">Request body</span></span>
<span data-ttu-id="385d2-129">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="385d2-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="385d2-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="385d2-130">Response</span></span>
<span data-ttu-id="385d2-131">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [ProgramControl](../resources/programcontrol.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="385d2-131">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="385d2-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="385d2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="385d2-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="385d2-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs('673a7379-9c38-4f01-bd9d-4fda7260b807')/controls
```

##### <a name="response"></a><span data-ttu-id="385d2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="385d2-134">Response</span></span>
><span data-ttu-id="385d2-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="385d2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "id": "bd68f301-e44b-4ad1-ba6d-a07314ed2e79",
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


<!-- {
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
