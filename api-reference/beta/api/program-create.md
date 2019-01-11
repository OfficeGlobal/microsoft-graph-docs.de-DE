---
title: Erstellen der Anwendung
description: Zugriff auf in Azure AD Bewertungen Feature, erstellen Sie ein neues Programmobjekt.
localization_priority: Normal
ms.openlocfilehash: b982242bbdddb9769d64c9757d9041fddc215d53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844016"
---
# <a name="create-program"></a><span data-ttu-id="b76ee-103">Erstellen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="b76ee-103">Create program</span></span>

> <span data-ttu-id="b76ee-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b76ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b76ee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b76ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b76ee-106">Erstellen Sie ein neues [Programm](../resources/program.md) -Objekt in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.</span><span class="sxs-lookup"><span data-stu-id="b76ee-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b76ee-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b76ee-107">Permissions</span></span>
<span data-ttu-id="b76ee-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b76ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b76ee-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b76ee-110">Permission type</span></span>                        | <span data-ttu-id="b76ee-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b76ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b76ee-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b76ee-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b76ee-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="b76ee-113"></span></span>  <span data-ttu-id="b76ee-114">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Erstellen eines Programms zulässt.</span><span class="sxs-lookup"><span data-stu-id="b76ee-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="b76ee-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b76ee-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b76ee-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b76ee-116">Not supported.</span></span> |
|<span data-ttu-id="b76ee-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b76ee-117">Application</span></span>                            | <span data-ttu-id="b76ee-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b76ee-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b76ee-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b76ee-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="b76ee-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b76ee-120">Request headers</span></span>
| <span data-ttu-id="b76ee-121">Name</span><span class="sxs-lookup"><span data-stu-id="b76ee-121">Name</span></span>         | <span data-ttu-id="b76ee-122">Typ</span><span class="sxs-lookup"><span data-stu-id="b76ee-122">Type</span></span>        | <span data-ttu-id="b76ee-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b76ee-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b76ee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b76ee-124">Authorization</span></span> | <span data-ttu-id="b76ee-125">string</span><span class="sxs-lookup"><span data-stu-id="b76ee-125">string</span></span> | <span data-ttu-id="b76ee-126">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="b76ee-126">Bearer \{token\}.</span></span> <span data-ttu-id="b76ee-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b76ee-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b76ee-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b76ee-128">Request body</span></span>
<span data-ttu-id="b76ee-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Programm](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="b76ee-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="b76ee-130">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie ein Programm erstellen.</span><span class="sxs-lookup"><span data-stu-id="b76ee-130">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="b76ee-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b76ee-131">Property</span></span>     | <span data-ttu-id="b76ee-132">Typ</span><span class="sxs-lookup"><span data-stu-id="b76ee-132">Type</span></span>        | <span data-ttu-id="b76ee-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b76ee-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="b76ee-134">Der Name des Programms.</span><span class="sxs-lookup"><span data-stu-id="b76ee-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="b76ee-135">Die Beschreibung des Programms.</span><span class="sxs-lookup"><span data-stu-id="b76ee-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="b76ee-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b76ee-136">Response</span></span>
<span data-ttu-id="b76ee-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortobjekt und [Programmdateien](../resources/program.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b76ee-137">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b76ee-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b76ee-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b76ee-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b76ee-139">Request</span></span>
<span data-ttu-id="b76ee-140">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Programm](../resources/program.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b76ee-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="b76ee-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="b76ee-141">Response</span></span>
><span data-ttu-id="b76ee-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b76ee-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b76ee-144">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="b76ee-144">See also</span></span>

| <span data-ttu-id="b76ee-145">Methode</span><span class="sxs-lookup"><span data-stu-id="b76ee-145">Method</span></span>           | <span data-ttu-id="b76ee-146">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b76ee-146">Return Type</span></span>    |<span data-ttu-id="b76ee-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b76ee-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b76ee-148">Programme auflisten</span><span class="sxs-lookup"><span data-stu-id="b76ee-148">List programs</span></span>](program-list.md) | <span data-ttu-id="b76ee-149">[Programm](../resources/program.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b76ee-149">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="b76ee-150">Rufen Sie eine Auflistung aller Programme.</span><span class="sxs-lookup"><span data-stu-id="b76ee-150">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="b76ee-151">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="b76ee-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="b76ee-152">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b76ee-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="b76ee-153">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="b76ee-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="b76ee-154">Update-Programm</span><span class="sxs-lookup"><span data-stu-id="b76ee-154">Update program</span></span>](program-update.md) |  [<span data-ttu-id="b76ee-155">Programm</span><span class="sxs-lookup"><span data-stu-id="b76ee-155">program</span></span>](../resources/program.md)| <span data-ttu-id="b76ee-156">Aktualisieren eines Programms.</span><span class="sxs-lookup"><span data-stu-id="b76ee-156">Update a program.</span></span>|
|[<span data-ttu-id="b76ee-157">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="b76ee-157">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="b76ee-158">programControl</span><span class="sxs-lookup"><span data-stu-id="b76ee-158">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="b76ee-159">Fügen Sie ein Programm ein ProgramControl hinzu.</span><span class="sxs-lookup"><span data-stu-id="b76ee-159">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
