---
title: Update-Programm
description: In Azure AD zugreifen auf Berichte-Funktion, aktualisieren Sie ein vorhandenes Programmobjekt zu.
ms.openlocfilehash: e3d8ca75683a076f156e359431204517b60e7c6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063499"
---
# <a name="update-program"></a><span data-ttu-id="518d2-103">Update-Programm</span><span class="sxs-lookup"><span data-stu-id="518d2-103">Update program</span></span>

> <span data-ttu-id="518d2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="518d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="518d2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="518d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="518d2-106">Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [Programm](../resources/program.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="518d2-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="518d2-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="518d2-107">Permissions</span></span>
<span data-ttu-id="518d2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="518d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="518d2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="518d2-110">Permission type</span></span>                        | <span data-ttu-id="518d2-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="518d2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="518d2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="518d2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="518d2-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="518d2-113"></span></span>  <span data-ttu-id="518d2-114">Der angemeldeten Benutzer muss auch in ein Verzeichnis-Rolle sein, die diese ein Programm aktualisieren zulässt.</span><span class="sxs-lookup"><span data-stu-id="518d2-114">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="518d2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="518d2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="518d2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="518d2-116">Not supported.</span></span> |
|<span data-ttu-id="518d2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="518d2-117">Application</span></span>                            | <span data-ttu-id="518d2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="518d2-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="518d2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="518d2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="518d2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="518d2-120">Request headers</span></span>
| <span data-ttu-id="518d2-121">Name</span><span class="sxs-lookup"><span data-stu-id="518d2-121">Name</span></span>         | <span data-ttu-id="518d2-122">Typ</span><span class="sxs-lookup"><span data-stu-id="518d2-122">Type</span></span>        | <span data-ttu-id="518d2-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="518d2-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="518d2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="518d2-124">Authorization</span></span> | <span data-ttu-id="518d2-125">string</span><span class="sxs-lookup"><span data-stu-id="518d2-125">string</span></span> | <span data-ttu-id="518d2-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="518d2-126">Bearer \{token\}.</span></span> <span data-ttu-id="518d2-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="518d2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="518d2-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="518d2-128">Request body</span></span>
<span data-ttu-id="518d2-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Programm](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="518d2-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="518d2-130">In der folgenden Tabelle werden die Eigenschaften gezeigt, die bereitgestellt werden können, wenn ein Programm zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="518d2-130">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="518d2-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="518d2-131">Property</span></span>     | <span data-ttu-id="518d2-132">Typ</span><span class="sxs-lookup"><span data-stu-id="518d2-132">Type</span></span>        | <span data-ttu-id="518d2-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="518d2-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="518d2-134">Der Name des Programms.</span><span class="sxs-lookup"><span data-stu-id="518d2-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="518d2-135">Die Beschreibung des Programms.</span><span class="sxs-lookup"><span data-stu-id="518d2-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="518d2-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="518d2-136">Response</span></span>
<span data-ttu-id="518d2-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `204, Accepted` Antwortobjekt und [Programmdateien](../resources/program.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="518d2-137">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="518d2-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="518d2-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="518d2-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="518d2-139">Request</span></span>
<span data-ttu-id="518d2-140">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Parameter-Objekt [Programm](../resources/program.md) zu ändern.</span><span class="sxs-lookup"><span data-stu-id="518d2-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```

##### <a name="response"></a><span data-ttu-id="518d2-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="518d2-141">Response</span></span>
><span data-ttu-id="518d2-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="518d2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3 new name",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="518d2-144">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="518d2-144">See also</span></span>

| <span data-ttu-id="518d2-145">Methode</span><span class="sxs-lookup"><span data-stu-id="518d2-145">Method</span></span>           | <span data-ttu-id="518d2-146">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="518d2-146">Return Type</span></span>    |<span data-ttu-id="518d2-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="518d2-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="518d2-148">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="518d2-148">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="518d2-149">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="518d2-149">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="518d2-150">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="518d2-150">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="518d2-151">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="518d2-151">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="518d2-152">programControl</span><span class="sxs-lookup"><span data-stu-id="518d2-152">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="518d2-153">Fügen Sie ein Programm ein ProgramControl hinzu.</span><span class="sxs-lookup"><span data-stu-id="518d2-153">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
