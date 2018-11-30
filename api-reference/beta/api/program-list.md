---
title: Programme auflisten
description: Zugriff auf in Azure AD Bewertungen Feature, listet alle Programmobjekte.
ms.openlocfilehash: fd934ec4dcfe4feb6167a6cf397be3669099c123
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059433"
---
# <a name="list-programs"></a><span data-ttu-id="b44fc-103">Programme auflisten</span><span class="sxs-lookup"><span data-stu-id="b44fc-103">List programs</span></span>

> <span data-ttu-id="b44fc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b44fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b44fc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b44fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b44fc-106">Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature Listen Sie aller [Programm](../resources/program.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b44fc-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b44fc-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b44fc-107">Permissions</span></span>
<span data-ttu-id="b44fc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b44fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b44fc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b44fc-110">Permission type</span></span>                        | <span data-ttu-id="b44fc-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b44fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b44fc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b44fc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b44fc-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="b44fc-113"></span></span>  <span data-ttu-id="b44fc-114">Der angemeldeten Benutzer muss auch in ein Verzeichnis-Rolle sein, die diese zum Lesen von einem Programm zulässt.</span><span class="sxs-lookup"><span data-stu-id="b44fc-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="b44fc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b44fc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b44fc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b44fc-116">Not supported.</span></span> |
|<span data-ttu-id="b44fc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b44fc-117">Application</span></span>                            | <span data-ttu-id="b44fc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b44fc-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b44fc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b44fc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="b44fc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b44fc-120">Request headers</span></span>
| <span data-ttu-id="b44fc-121">Name</span><span class="sxs-lookup"><span data-stu-id="b44fc-121">Name</span></span>         | <span data-ttu-id="b44fc-122">Typ</span><span class="sxs-lookup"><span data-stu-id="b44fc-122">Type</span></span>        | <span data-ttu-id="b44fc-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b44fc-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b44fc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b44fc-124">Authorization</span></span> | <span data-ttu-id="b44fc-125">string</span><span class="sxs-lookup"><span data-stu-id="b44fc-125">string</span></span> | <span data-ttu-id="b44fc-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="b44fc-126">Bearer \{token\}.</span></span> <span data-ttu-id="b44fc-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b44fc-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b44fc-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b44fc-128">Request body</span></span>
<span data-ttu-id="b44fc-129">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="b44fc-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="b44fc-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="b44fc-130">Response</span></span>
<span data-ttu-id="b44fc-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200, OK` Antwortcode und ein Array von Objekten im Antworttext [Programm](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="b44fc-131">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b44fc-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b44fc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b44fc-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b44fc-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```

##### <a name="response"></a><span data-ttu-id="b44fc-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b44fc-134">Response</span></span>
><span data-ttu-id="b44fc-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b44fc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b44fc-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="b44fc-137">See also</span></span>

| <span data-ttu-id="b44fc-138">Methode</span><span class="sxs-lookup"><span data-stu-id="b44fc-138">Method</span></span>           | <span data-ttu-id="b44fc-139">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b44fc-139">Return Type</span></span>    |<span data-ttu-id="b44fc-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b44fc-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b44fc-141">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="b44fc-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="b44fc-142">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b44fc-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="b44fc-143">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="b44fc-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
