---
title: Erstellen der Anwendung
description: Zugriff auf in Azure AD Bewertungen Feature, erstellen Sie ein neues Programmobjekt.
localization_priority: Normal
ms.openlocfilehash: a6e9ab300cf44a2f3973c468679af7fa48262680
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521299"
---
# <a name="create-program"></a><span data-ttu-id="5576f-103">Erstellen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="5576f-103">Create program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5576f-104">Erstellen Sie ein neues [Programm](../resources/program.md) -Objekt in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.</span><span class="sxs-lookup"><span data-stu-id="5576f-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5576f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5576f-105">Permissions</span></span>
<span data-ttu-id="5576f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5576f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5576f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5576f-108">Permission type</span></span>                        | <span data-ttu-id="5576f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5576f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5576f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5576f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5576f-111">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="5576f-111"></span></span>  <span data-ttu-id="5576f-112">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Erstellen eines Programms zulässt.</span><span class="sxs-lookup"><span data-stu-id="5576f-112">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="5576f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5576f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5576f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5576f-114">Not supported.</span></span> |
|<span data-ttu-id="5576f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5576f-115">Application</span></span>                            | <span data-ttu-id="5576f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5576f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5576f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5576f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="5576f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5576f-118">Request headers</span></span>
| <span data-ttu-id="5576f-119">Name</span><span class="sxs-lookup"><span data-stu-id="5576f-119">Name</span></span>         | <span data-ttu-id="5576f-120">Typ</span><span class="sxs-lookup"><span data-stu-id="5576f-120">Type</span></span>        | <span data-ttu-id="5576f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5576f-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5576f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5576f-122">Authorization</span></span> | <span data-ttu-id="5576f-123">string</span><span class="sxs-lookup"><span data-stu-id="5576f-123">string</span></span> | <span data-ttu-id="5576f-124">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="5576f-124">Bearer \{token\}.</span></span> <span data-ttu-id="5576f-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5576f-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5576f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5576f-126">Request body</span></span>
<span data-ttu-id="5576f-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Programm](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="5576f-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="5576f-128">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie ein Programm erstellen.</span><span class="sxs-lookup"><span data-stu-id="5576f-128">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="5576f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5576f-129">Property</span></span>     | <span data-ttu-id="5576f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5576f-130">Type</span></span>        | <span data-ttu-id="5576f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5576f-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="5576f-132">Der Name des Programms.</span><span class="sxs-lookup"><span data-stu-id="5576f-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="5576f-133">Die Beschreibung des Programms.</span><span class="sxs-lookup"><span data-stu-id="5576f-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="5576f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5576f-134">Response</span></span>
<span data-ttu-id="5576f-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortobjekt und [Programmdateien](../resources/program.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5576f-135">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5576f-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5576f-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5576f-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5576f-137">Request</span></span>
<span data-ttu-id="5576f-138">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Programm](../resources/program.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5576f-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="5576f-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="5576f-139">Response</span></span>
><span data-ttu-id="5576f-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5576f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5576f-142">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5576f-142">See also</span></span>

| <span data-ttu-id="5576f-143">Methode</span><span class="sxs-lookup"><span data-stu-id="5576f-143">Method</span></span>           | <span data-ttu-id="5576f-144">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5576f-144">Return Type</span></span>    |<span data-ttu-id="5576f-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5576f-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5576f-146">Programme auflisten</span><span class="sxs-lookup"><span data-stu-id="5576f-146">List programs</span></span>](program-list.md) | <span data-ttu-id="5576f-147">[Programm](../resources/program.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5576f-147">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="5576f-148">Rufen Sie eine Auflistung aller Programme.</span><span class="sxs-lookup"><span data-stu-id="5576f-148">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="5576f-149">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="5576f-149">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="5576f-150">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5576f-150">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="5576f-151">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="5576f-151">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="5576f-152">Update-Programm</span><span class="sxs-lookup"><span data-stu-id="5576f-152">Update program</span></span>](program-update.md) |  [<span data-ttu-id="5576f-153">Programm</span><span class="sxs-lookup"><span data-stu-id="5576f-153">program</span></span>](../resources/program.md)| <span data-ttu-id="5576f-154">Aktualisieren eines Programms.</span><span class="sxs-lookup"><span data-stu-id="5576f-154">Update a program.</span></span>|
|[<span data-ttu-id="5576f-155">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="5576f-155">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="5576f-156">programControl</span><span class="sxs-lookup"><span data-stu-id="5576f-156">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="5576f-157">Fügen Sie ein Programm ein ProgramControl hinzu.</span><span class="sxs-lookup"><span data-stu-id="5576f-157">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
