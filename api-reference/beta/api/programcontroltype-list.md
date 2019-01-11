---
title: Liste programControlTypes
description: Öffnen Sie in Azure AD Bewertungen Feature, Sie alle ProgramControlType Objekte auflisten.
localization_priority: Normal
ms.openlocfilehash: ae5a2298d3c0f542f7d8fd766f412b8cf5648730
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860886"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="99ef6-103">Liste programControlTypes</span><span class="sxs-lookup"><span data-stu-id="99ef6-103">List programControlTypes</span></span>

> <span data-ttu-id="99ef6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="99ef6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99ef6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99ef6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99ef6-106">Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature Listen Sie aller [ProgramControlType](../resources/programcontroltype.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="99ef6-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="99ef6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="99ef6-107">Permissions</span></span>
<span data-ttu-id="99ef6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99ef6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99ef6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99ef6-110">Permission type</span></span>                        | <span data-ttu-id="99ef6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99ef6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="99ef6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99ef6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="99ef6-113">`ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="99ef6-113"></span></span>  <span data-ttu-id="99ef6-114">Der angemeldeten Benutzer muss auch in ein Verzeichnis-Rolle sein, die diese zum Lesen von einem Programm zulässt.</span><span class="sxs-lookup"><span data-stu-id="99ef6-114">The signed in user must also be in a directory role which permits them to read a program.</span></span> |
|<span data-ttu-id="99ef6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99ef6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99ef6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99ef6-116">Not supported.</span></span> |
|<span data-ttu-id="99ef6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99ef6-117">Application</span></span>                            | <span data-ttu-id="99ef6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99ef6-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99ef6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99ef6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="99ef6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99ef6-120">Request headers</span></span>
| <span data-ttu-id="99ef6-121">Name</span><span class="sxs-lookup"><span data-stu-id="99ef6-121">Name</span></span>         | <span data-ttu-id="99ef6-122">Typ</span><span class="sxs-lookup"><span data-stu-id="99ef6-122">Type</span></span>        | <span data-ttu-id="99ef6-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99ef6-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="99ef6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="99ef6-124">Authorization</span></span> | <span data-ttu-id="99ef6-125">string</span><span class="sxs-lookup"><span data-stu-id="99ef6-125">string</span></span> | <span data-ttu-id="99ef6-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="99ef6-126">Bearer \{token\}.</span></span> <span data-ttu-id="99ef6-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99ef6-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99ef6-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99ef6-128">Request body</span></span>
<span data-ttu-id="99ef6-129">Keine Anforderungstext sollte angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="99ef6-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="99ef6-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="99ef6-130">Response</span></span>
<span data-ttu-id="99ef6-131">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200, OK` Antwortcode und ein Array von [ProgramControlType](../resources/programcontroltype.md) -Objekten im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="99ef6-131">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99ef6-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99ef6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99ef6-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99ef6-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="99ef6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="99ef6-134">Response</span></span>
><span data-ttu-id="99ef6-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="99ef6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="99ef6-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="99ef6-137">See also</span></span>

| <span data-ttu-id="99ef6-138">Methode</span><span class="sxs-lookup"><span data-stu-id="99ef6-138">Method</span></span>           | <span data-ttu-id="99ef6-139">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="99ef6-139">Return Type</span></span>    |<span data-ttu-id="99ef6-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99ef6-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99ef6-141">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="99ef6-141">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="99ef6-142">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="99ef6-142">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="99ef6-143">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="99ef6-143">Get a collection of the controls of a program.</span></span>|


<!-- {
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
