---
title: Erstellen der Anwendung
description: Zugriff auf in Azure AD Bewertungen Feature, erstellen Sie ein neues Programmobjekt.
ms.openlocfilehash: 1ac3fa1f0b555fc92449adf0e57217d0a7d50375
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064152"
---
# <a name="create-program"></a><span data-ttu-id="f3d00-103">Erstellen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3d00-103">Create program</span></span>

> <span data-ttu-id="f3d00-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f3d00-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3d00-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3d00-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3d00-106">Erstellen Sie ein neues [Programm](../resources/program.md) -Objekt in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.</span><span class="sxs-lookup"><span data-stu-id="f3d00-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3d00-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f3d00-107">Permissions</span></span>
<span data-ttu-id="f3d00-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3d00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3d00-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3d00-110">Permission type</span></span>                        | <span data-ttu-id="f3d00-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3d00-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3d00-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3d00-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3d00-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="f3d00-113"></span></span>  <span data-ttu-id="f3d00-114">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Erstellen eines Programms zulässt.</span><span class="sxs-lookup"><span data-stu-id="f3d00-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="f3d00-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3d00-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3d00-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3d00-116">Not supported.</span></span> |
|<span data-ttu-id="f3d00-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3d00-117">Application</span></span>                            | <span data-ttu-id="f3d00-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3d00-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3d00-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3d00-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="f3d00-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3d00-120">Request headers</span></span>
| <span data-ttu-id="f3d00-121">Name</span><span class="sxs-lookup"><span data-stu-id="f3d00-121">Name</span></span>         | <span data-ttu-id="f3d00-122">Typ</span><span class="sxs-lookup"><span data-stu-id="f3d00-122">Type</span></span>        | <span data-ttu-id="f3d00-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3d00-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f3d00-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3d00-124">Authorization</span></span> | <span data-ttu-id="f3d00-125">string</span><span class="sxs-lookup"><span data-stu-id="f3d00-125">string</span></span> | <span data-ttu-id="f3d00-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="f3d00-126">Bearer \{token\}.</span></span> <span data-ttu-id="f3d00-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f3d00-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3d00-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3d00-128">Request body</span></span>
<span data-ttu-id="f3d00-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Programm](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="f3d00-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="f3d00-130">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie ein Programm erstellen.</span><span class="sxs-lookup"><span data-stu-id="f3d00-130">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="f3d00-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f3d00-131">Property</span></span>     | <span data-ttu-id="f3d00-132">Typ</span><span class="sxs-lookup"><span data-stu-id="f3d00-132">Type</span></span>        | <span data-ttu-id="f3d00-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3d00-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="f3d00-134">Der Name des Programms.</span><span class="sxs-lookup"><span data-stu-id="f3d00-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="f3d00-135">Die Beschreibung des Programms.</span><span class="sxs-lookup"><span data-stu-id="f3d00-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="f3d00-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3d00-136">Response</span></span>
<span data-ttu-id="f3d00-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortobjekt und [Programmdateien](../resources/program.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f3d00-137">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3d00-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3d00-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3d00-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3d00-139">Request</span></span>
<span data-ttu-id="f3d00-140">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Programm](../resources/program.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f3d00-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```

##### <a name="response"></a><span data-ttu-id="f3d00-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3d00-141">Response</span></span>
><span data-ttu-id="f3d00-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="f3d00-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="f3d00-144">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="f3d00-144">See also</span></span>

| <span data-ttu-id="f3d00-145">Methode</span><span class="sxs-lookup"><span data-stu-id="f3d00-145">Method</span></span>           | <span data-ttu-id="f3d00-146">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f3d00-146">Return Type</span></span>    |<span data-ttu-id="f3d00-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3d00-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f3d00-148">Programme auflisten</span><span class="sxs-lookup"><span data-stu-id="f3d00-148">List programs</span></span>](program-list.md) | <span data-ttu-id="f3d00-149">[Programm](../resources/program.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f3d00-149">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="f3d00-150">Rufen Sie eine Auflistung aller Programme.</span><span class="sxs-lookup"><span data-stu-id="f3d00-150">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="f3d00-151">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="f3d00-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="f3d00-152">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f3d00-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="f3d00-153">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="f3d00-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="f3d00-154">Update-Programm</span><span class="sxs-lookup"><span data-stu-id="f3d00-154">Update program</span></span>](program-update.md) |  [<span data-ttu-id="f3d00-155">Programm</span><span class="sxs-lookup"><span data-stu-id="f3d00-155">program</span></span>](../resources/program.md)| <span data-ttu-id="f3d00-156">Aktualisieren eines Programms.</span><span class="sxs-lookup"><span data-stu-id="f3d00-156">Update a program.</span></span>|
|[<span data-ttu-id="f3d00-157">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="f3d00-157">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="f3d00-158">programControl</span><span class="sxs-lookup"><span data-stu-id="f3d00-158">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="f3d00-159">Fügen Sie ein Programm ein ProgramControl hinzu.</span><span class="sxs-lookup"><span data-stu-id="f3d00-159">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
