---
title: Liste ProgramControls eines Programms
description: In Azure AD Access Feature überprüft, eine Liste aller ProgramControl Objekte für ein bestimmtes Programm verknüpft.
ms.openlocfilehash: 78b28851dadfa1c24bc5bc0556b1c471e7bc09e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058131"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="61bbf-103">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="61bbf-103">List programControls of a program</span></span>

> <span data-ttu-id="61bbf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="61bbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61bbf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61bbf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61bbf-106">Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature Listen Sie aller [ProgramControl](../resources/programcontrol.md) -Objekte, um ein bestimmtes Programm verknüpft.</span><span class="sxs-lookup"><span data-stu-id="61bbf-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="61bbf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="61bbf-107">Permissions</span></span>
<span data-ttu-id="61bbf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61bbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61bbf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61bbf-110">Permission type</span></span>                        | <span data-ttu-id="61bbf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61bbf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="61bbf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61bbf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="61bbf-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="61bbf-113"></span></span>  <span data-ttu-id="61bbf-114">Der angemeldeten Benutzer muss auch in ein Verzeichnis-Rolle sein, die diese zum Lesen von einem Programm zulässt.</span><span class="sxs-lookup"><span data-stu-id="61bbf-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="61bbf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61bbf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61bbf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61bbf-116">Not supported.</span></span> |
|<span data-ttu-id="61bbf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61bbf-117">Application</span></span>                            | <span data-ttu-id="61bbf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61bbf-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61bbf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61bbf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="61bbf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61bbf-120">Request headers</span></span>
| <span data-ttu-id="61bbf-121">Name</span><span class="sxs-lookup"><span data-stu-id="61bbf-121">Name</span></span>         | <span data-ttu-id="61bbf-122">Typ</span><span class="sxs-lookup"><span data-stu-id="61bbf-122">Type</span></span>        | <span data-ttu-id="61bbf-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61bbf-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="61bbf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="61bbf-124">Authorization</span></span> | <span data-ttu-id="61bbf-125">string</span><span class="sxs-lookup"><span data-stu-id="61bbf-125">string</span></span> | <span data-ttu-id="61bbf-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="61bbf-126">Bearer \{token\}.</span></span> <span data-ttu-id="61bbf-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="61bbf-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61bbf-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61bbf-128">Request body</span></span>
<span data-ttu-id="61bbf-129">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="61bbf-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="61bbf-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="61bbf-130">Response</span></span>
<span data-ttu-id="61bbf-131">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [ProgramControl](../resources/programcontrol.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="61bbf-131">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61bbf-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61bbf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61bbf-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61bbf-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs('673a7379-9c38-4f01-bd9d-4fda7260b807')/controls
```

##### <a name="response"></a><span data-ttu-id="61bbf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="61bbf-134">Response</span></span>
><span data-ttu-id="61bbf-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="61bbf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
