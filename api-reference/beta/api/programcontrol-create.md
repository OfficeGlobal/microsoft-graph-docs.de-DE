---
title: Erstellen von programControl
description: Zugriff auf in Azure AD Bewertungen Feature, Erstellen eines neuen ProgramControl-Objekts.  Dadurch werden eine Access-Überprüfung an ein Programm verknüpft.
ms.openlocfilehash: fa6a93b13391fd4b9e3c5816bb2a27259e730c0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063700"
---
# <a name="create-programcontrol"></a><span data-ttu-id="5b58b-104">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="5b58b-104">Create programControl</span></span>

> <span data-ttu-id="5b58b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b58b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b58b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b58b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b58b-107">Erstellen Sie ein neues [ProgramControl](../resources/programcontrol.md) -Objekt in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.</span><span class="sxs-lookup"><span data-stu-id="5b58b-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="5b58b-108">Dadurch werden eine Access-Überprüfung an ein Programm verknüpft.</span><span class="sxs-lookup"><span data-stu-id="5b58b-108">This links an access review to a program.</span></span>

<span data-ttu-id="5b58b-109">Bevor Sie diese Anforderung machen, muss der Aufrufer zuvor verfügen</span><span class="sxs-lookup"><span data-stu-id="5b58b-109">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="5b58b-110">[erstellt ein Programm](program-create.md) oder [eine Anwendung abgerufen](program-list.md), damit den Wert der `programId` zum Einschließen in die Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b58b-110">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="5b58b-111">[erstellt eine Überprüfung Access](accessreview-create.md) oder [eine Access-Überprüfung abgerufen](accessreview-get.md), damit den Wert der `controlId` zum Einschließen in die Anforderung und</span><span class="sxs-lookup"><span data-stu-id="5b58b-111">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="5b58b-112">[die Liste der Typen von Steuerelementen Programm abgerufen](programcontroltype-list.md), damit den Wert der `controlTypeId` in der Anforderung enthalten.</span><span class="sxs-lookup"><span data-stu-id="5b58b-112">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="5b58b-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5b58b-113">Permissions</span></span>
<span data-ttu-id="5b58b-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b58b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b58b-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b58b-116">Permission type</span></span>                        | <span data-ttu-id="5b58b-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b58b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b58b-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b58b-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b58b-119">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="5b58b-119"></span></span>  <span data-ttu-id="5b58b-120">Der Benutzer angemeldet muss auch in einer Directory-Rolle sein, die diese zum Erstellen einer ProgramControl zulässt.</span><span class="sxs-lookup"><span data-stu-id="5b58b-120">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="5b58b-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b58b-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b58b-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b58b-122">Not supported.</span></span> |
|<span data-ttu-id="5b58b-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b58b-123">Application</span></span>                            | <span data-ttu-id="5b58b-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b58b-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b58b-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b58b-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="5b58b-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b58b-126">Request headers</span></span>
| <span data-ttu-id="5b58b-127">Name</span><span class="sxs-lookup"><span data-stu-id="5b58b-127">Name</span></span>         | <span data-ttu-id="5b58b-128">Typ</span><span class="sxs-lookup"><span data-stu-id="5b58b-128">Type</span></span>        | <span data-ttu-id="5b58b-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b58b-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5b58b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b58b-130">Authorization</span></span> | <span data-ttu-id="5b58b-131">string</span><span class="sxs-lookup"><span data-stu-id="5b58b-131">string</span></span> | <span data-ttu-id="5b58b-132">Bearer \{token\}.</span><span class="sxs-lookup"><span data-stu-id="5b58b-132">Bearer \{token\}.</span></span> <span data-ttu-id="5b58b-133">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b58b-133">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b58b-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b58b-134">Request body</span></span>
<span data-ttu-id="5b58b-135">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [ProgramControl](../resources/programcontrol.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5b58b-135">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="5b58b-136">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie ein Programmsteuerelement erstellen.</span><span class="sxs-lookup"><span data-stu-id="5b58b-136">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="5b58b-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b58b-137">Property</span></span>     | <span data-ttu-id="5b58b-138">Typ</span><span class="sxs-lookup"><span data-stu-id="5b58b-138">Type</span></span>        | <span data-ttu-id="5b58b-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b58b-139">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="5b58b-140">Die ProgramId des Programms wird dieses Steuerelement eines Teils werden sollte.</span><span class="sxs-lookup"><span data-stu-id="5b58b-140">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="5b58b-141">Die ControlId des Steuerelements, insbesondere die eine Access-ID überprüfen.</span><span class="sxs-lookup"><span data-stu-id="5b58b-141">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="5b58b-142">Die ProgramControlType identifiziert den Typ des programmfreigabesteuerung – beispielsweise ein Steuerelement verknüpfen mit Gast Access überprüft.</span><span class="sxs-lookup"><span data-stu-id="5b58b-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="5b58b-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b58b-143">Response</span></span>
<span data-ttu-id="5b58b-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201, Created` Antwortcode und eines [ProgramControl](../resources/programcontrol.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5b58b-144">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="5b58b-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b58b-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b58b-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b58b-146">Request</span></span>
<span data-ttu-id="5b58b-147">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [ProgramControl](../resources/programcontrol.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5b58b-147">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="5b58b-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b58b-148">Response</span></span>
><span data-ttu-id="5b58b-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="5b58b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5b58b-151">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5b58b-151">See also</span></span>

| <span data-ttu-id="5b58b-152">Methode</span><span class="sxs-lookup"><span data-stu-id="5b58b-152">Method</span></span>           | <span data-ttu-id="5b58b-153">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5b58b-153">Return Type</span></span>    |<span data-ttu-id="5b58b-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b58b-154">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b58b-155">Liste programControlTypes</span><span class="sxs-lookup"><span data-stu-id="5b58b-155">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="5b58b-156">[ProgramControlType](../resources/programcontroltype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5b58b-156">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="5b58b-157">Programm Steuerelement Listentypen.</span><span class="sxs-lookup"><span data-stu-id="5b58b-157">List program control types.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
