---
title: Erstellen von programControl
description: Zugriff auf in Azure AD Bewertungen Feature, Erstellen eines neuen ProgramControl-Objekts.  Dadurch werden eine Access-Überprüfung an ein Programm verknüpft.
localization_priority: Normal
ms.openlocfilehash: 89e31994ea91dba68e2f4563c64eeab53dd4db93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511114"
---
# <a name="create-programcontrol"></a><span data-ttu-id="d2f74-104">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="d2f74-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2f74-105">Erstellen Sie ein neues [ProgramControl](../resources/programcontrol.md) -Objekt in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.</span><span class="sxs-lookup"><span data-stu-id="d2f74-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="d2f74-106">Dadurch werden eine Access-Überprüfung an ein Programm verknüpft.</span><span class="sxs-lookup"><span data-stu-id="d2f74-106">This links an access review to a program.</span></span>

<span data-ttu-id="d2f74-107">Bevor Sie diese Anforderung machen, muss der Aufrufer zuvor verfügen</span><span class="sxs-lookup"><span data-stu-id="d2f74-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="d2f74-108">[erstellt ein Programm](program-create.md) oder [eine Anwendung abgerufen](program-list.md), damit den Wert der `programId` zum Einschließen in die Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2f74-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="d2f74-109">[erstellt eine Überprüfung Access](accessreview-create.md) oder [eine Access-Überprüfung abgerufen](accessreview-get.md), damit den Wert der `controlId` zum Einschließen in die Anforderung und</span><span class="sxs-lookup"><span data-stu-id="d2f74-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="d2f74-110">[die Liste der Typen von Steuerelementen Programm abgerufen](programcontroltype-list.md), damit den Wert der `controlTypeId` in der Anforderung enthalten.</span><span class="sxs-lookup"><span data-stu-id="d2f74-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="d2f74-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d2f74-111">Permissions</span></span>
<span data-ttu-id="d2f74-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2f74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2f74-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d2f74-114">Permission type</span></span>                        | <span data-ttu-id="d2f74-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d2f74-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2f74-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d2f74-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2f74-117">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="d2f74-117"></span></span>  <span data-ttu-id="d2f74-118">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Erstellen einer ProgramControl zulässt.</span><span class="sxs-lookup"><span data-stu-id="d2f74-118">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="d2f74-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d2f74-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2f74-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2f74-120">Not supported.</span></span> |
|<span data-ttu-id="d2f74-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d2f74-121">Application</span></span>                            | <span data-ttu-id="d2f74-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d2f74-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2f74-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2f74-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="d2f74-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d2f74-124">Request headers</span></span>
| <span data-ttu-id="d2f74-125">Name</span><span class="sxs-lookup"><span data-stu-id="d2f74-125">Name</span></span>         | <span data-ttu-id="d2f74-126">Typ</span><span class="sxs-lookup"><span data-stu-id="d2f74-126">Type</span></span>        | <span data-ttu-id="d2f74-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2f74-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d2f74-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2f74-128">Authorization</span></span> | <span data-ttu-id="d2f74-129">string</span><span class="sxs-lookup"><span data-stu-id="d2f74-129">string</span></span> | <span data-ttu-id="d2f74-130">Bearertoken</span><span class="sxs-lookup"><span data-stu-id="d2f74-130">Bearer \{token\}.</span></span> <span data-ttu-id="d2f74-131">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d2f74-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2f74-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d2f74-132">Request body</span></span>
<span data-ttu-id="d2f74-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [ProgramControl](../resources/programcontrol.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d2f74-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="d2f74-134">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie ein Programmsteuerelement erstellen.</span><span class="sxs-lookup"><span data-stu-id="d2f74-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="d2f74-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d2f74-135">Property</span></span>     | <span data-ttu-id="d2f74-136">Typ</span><span class="sxs-lookup"><span data-stu-id="d2f74-136">Type</span></span>        | <span data-ttu-id="d2f74-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2f74-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="d2f74-138">Die ProgramId des Programms wird dieses Steuerelement eines Teils werden sollte.</span><span class="sxs-lookup"><span data-stu-id="d2f74-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="d2f74-139">Die ControlId des Steuerelements, insbesondere die eine Access-ID überprüfen.</span><span class="sxs-lookup"><span data-stu-id="d2f74-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="d2f74-140">Die ProgramControlType identifiziert den Typ des programmfreigabesteuerung – beispielsweise ein Steuerelement verknüpfen mit Gast Access überprüft.</span><span class="sxs-lookup"><span data-stu-id="d2f74-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="d2f74-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2f74-141">Response</span></span>
<span data-ttu-id="d2f74-142">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortcode und eines [ProgramControl](../resources/programcontrol.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d2f74-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="d2f74-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d2f74-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2f74-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2f74-144">Request</span></span>
<span data-ttu-id="d2f74-145">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ProgramControl](../resources/programcontrol.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d2f74-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```

##### <a name="response"></a><span data-ttu-id="d2f74-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2f74-146">Response</span></span>
><span data-ttu-id="d2f74-p106">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d2f74-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```

## <a name="see-also"></a><span data-ttu-id="d2f74-149">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="d2f74-149">See also</span></span>

| <span data-ttu-id="d2f74-150">Methode</span><span class="sxs-lookup"><span data-stu-id="d2f74-150">Method</span></span>           | <span data-ttu-id="d2f74-151">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d2f74-151">Return Type</span></span>    |<span data-ttu-id="d2f74-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2f74-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2f74-153">Liste programControlTypes</span><span class="sxs-lookup"><span data-stu-id="d2f74-153">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="d2f74-154">[ProgramControlType](../resources/programcontroltype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d2f74-154">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="d2f74-155">Programm Steuerelement Listentypen.</span><span class="sxs-lookup"><span data-stu-id="d2f74-155">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
