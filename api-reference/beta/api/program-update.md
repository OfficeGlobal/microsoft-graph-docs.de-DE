---
title: Update-Programm
description: In Azure AD zugreifen auf Berichte-Funktion, aktualisieren Sie ein vorhandenes Programmobjekt zu.
localization_priority: Normal
ms.openlocfilehash: 75562aac5a7b3f3aaef0c8a1251d32a7728813aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529922"
---
# <a name="update-program"></a><span data-ttu-id="689bc-103">Update-Programm</span><span class="sxs-lookup"><span data-stu-id="689bc-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="689bc-104">Aktualisieren Sie in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature eines vorhandenen [Programm](../resources/program.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="689bc-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="689bc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="689bc-105">Permissions</span></span>
<span data-ttu-id="689bc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="689bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="689bc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="689bc-108">Permission type</span></span>                        | <span data-ttu-id="689bc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="689bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="689bc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="689bc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="689bc-111">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="689bc-111"></span></span>  <span data-ttu-id="689bc-112">Der angemeldeten Benutzer muss auch in ein Verzeichnis-Rolle sein, die diese ein Programm aktualisieren zulässt.</span><span class="sxs-lookup"><span data-stu-id="689bc-112">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="689bc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="689bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="689bc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="689bc-114">Not supported.</span></span> |
|<span data-ttu-id="689bc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="689bc-115">Application</span></span>                            | <span data-ttu-id="689bc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="689bc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="689bc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="689bc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="689bc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="689bc-118">Request headers</span></span>
| <span data-ttu-id="689bc-119">Name</span><span class="sxs-lookup"><span data-stu-id="689bc-119">Name</span></span>         | <span data-ttu-id="689bc-120">Typ</span><span class="sxs-lookup"><span data-stu-id="689bc-120">Type</span></span>        | <span data-ttu-id="689bc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="689bc-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="689bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="689bc-122">Authorization</span></span> | <span data-ttu-id="689bc-123">string</span><span class="sxs-lookup"><span data-stu-id="689bc-123">string</span></span> | <span data-ttu-id="689bc-124">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="689bc-124">Bearer \{token\}.</span></span> <span data-ttu-id="689bc-125">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="689bc-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="689bc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="689bc-126">Request body</span></span>
<span data-ttu-id="689bc-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Programm](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="689bc-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="689bc-128">In der folgenden Tabelle werden die Eigenschaften gezeigt, die bereitgestellt werden können, wenn ein Programm zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="689bc-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="689bc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="689bc-129">Property</span></span>     | <span data-ttu-id="689bc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="689bc-130">Type</span></span>        | <span data-ttu-id="689bc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="689bc-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="689bc-132">Der Name des Programms.</span><span class="sxs-lookup"><span data-stu-id="689bc-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="689bc-133">Die Beschreibung des Programms.</span><span class="sxs-lookup"><span data-stu-id="689bc-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="689bc-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="689bc-134">Response</span></span>
<span data-ttu-id="689bc-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `204, Accepted` Antwortobjekt und [Programmdateien](../resources/program.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="689bc-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="689bc-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="689bc-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="689bc-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="689bc-137">Request</span></span>
<span data-ttu-id="689bc-138">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der Parameter-Objekt [Programm](../resources/program.md) zu ändern.</span><span class="sxs-lookup"><span data-stu-id="689bc-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

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

##### <a name="response"></a><span data-ttu-id="689bc-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="689bc-139">Response</span></span>
><span data-ttu-id="689bc-p104">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="689bc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="689bc-142">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="689bc-142">See also</span></span>

| <span data-ttu-id="689bc-143">Methode</span><span class="sxs-lookup"><span data-stu-id="689bc-143">Method</span></span>           | <span data-ttu-id="689bc-144">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="689bc-144">Return Type</span></span>    |<span data-ttu-id="689bc-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="689bc-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="689bc-146">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="689bc-146">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="689bc-147">[ProgramControl](../resources/programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="689bc-147">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="689bc-148">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="689bc-148">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="689bc-149">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="689bc-149">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="689bc-150">programControl</span><span class="sxs-lookup"><span data-stu-id="689bc-150">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="689bc-151">Fügen Sie ein Programm ein ProgramControl hinzu.</span><span class="sxs-lookup"><span data-stu-id="689bc-151">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
