---
title: Ressourcentyp programControl
description: In Azure AD Access Feature überprüft, und das Programm Control-Objekt stellt ein Steuerelement, Verknüpfen einer Access-Überprüfung an ein Programm dar.
ms.openlocfilehash: 03e70ffdf0607eeb11abaf1b12065b4092294d23
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061148"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="54352-103">Ressourcentyp programControl</span><span class="sxs-lookup"><span data-stu-id="54352-103">programControl resource type</span></span>

> <span data-ttu-id="54352-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="54352-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54352-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54352-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54352-106">In Azure AD [Access überprüft](accessreviews-root.md) Feature stellt das Programm Control-Objekt ein Steuerelement, Verknüpfen einer Access-Überprüfung mit einer Anwendung.</span><span class="sxs-lookup"><span data-stu-id="54352-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="54352-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="54352-107">Methods</span></span>

| <span data-ttu-id="54352-108">Methode</span><span class="sxs-lookup"><span data-stu-id="54352-108">Method</span></span>           | <span data-ttu-id="54352-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="54352-109">Return Type</span></span>    |<span data-ttu-id="54352-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54352-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54352-111">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="54352-111">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="54352-112">programControl</span><span class="sxs-lookup"><span data-stu-id="54352-112">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="54352-113">Fügen Sie ein Programm ein ProgramControl hinzu.</span><span class="sxs-lookup"><span data-stu-id="54352-113">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="54352-114">ProgramControl löschen</span><span class="sxs-lookup"><span data-stu-id="54352-114">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="54352-115">Keine.</span><span class="sxs-lookup"><span data-stu-id="54352-115">None.</span></span>   |   <span data-ttu-id="54352-116">Entfernen einer ProgramControl aus einem Programm.</span><span class="sxs-lookup"><span data-stu-id="54352-116">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="54352-117">Liste programControls</span><span class="sxs-lookup"><span data-stu-id="54352-117">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="54352-118">[ProgramControl](programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="54352-118">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="54352-119">Von Listensteuerelementen in allen Programmen im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="54352-119">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="54352-120">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="54352-120">Permissions</span></span>

|<span data-ttu-id="54352-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="54352-121">Permission type</span></span>                        | <span data-ttu-id="54352-122">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="54352-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="54352-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="54352-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="54352-124">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54352-124">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="54352-125">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="54352-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54352-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54352-126">Not supported.</span></span> |
|<span data-ttu-id="54352-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="54352-127">Application</span></span>                            | <span data-ttu-id="54352-128">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="54352-128">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="54352-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="54352-129">Properties</span></span>
| <span data-ttu-id="54352-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54352-130">Property</span></span>     | <span data-ttu-id="54352-131">Typ</span><span class="sxs-lookup"><span data-stu-id="54352-131">Type</span></span>   |<span data-ttu-id="54352-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54352-132">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="54352-133">Die Feature-zugewiesenen Bezeichner der Verknüpfung zwischen Programm und Steuerelement</span><span class="sxs-lookup"><span data-stu-id="54352-133">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="54352-134">Die ProgramId des Programms dieses Steuerelement ist ein Teil der.</span><span class="sxs-lookup"><span data-stu-id="54352-134">The programId of the program this control is a part of.</span></span> <span data-ttu-id="54352-135">Erforderliche auf erstellen.</span><span class="sxs-lookup"><span data-stu-id="54352-135">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="54352-136">Die ControlId des Steuerelements, insbesondere die eine Access-ID überprüfen.</span><span class="sxs-lookup"><span data-stu-id="54352-136">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="54352-137">Erforderliche auf erstellen.</span><span class="sxs-lookup"><span data-stu-id="54352-137">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="54352-138">Die ProgramControlType identifiziert den Typ des programmfreigabesteuerung – beispielsweise ein Steuerelement verknüpfen mit Gast Access überprüft.</span><span class="sxs-lookup"><span data-stu-id="54352-138">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="54352-139">Erforderliche auf erstellen.</span><span class="sxs-lookup"><span data-stu-id="54352-139">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="54352-140">Der Name des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="54352-140">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="54352-141">Der Status des Lebenszyklus des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="54352-141">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="54352-142">Das Erstellungsdatum und die Uhrzeit des Steuerelements Programm.</span><span class="sxs-lookup"><span data-stu-id="54352-142">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="54352-143">Benutzeridentität</span><span class="sxs-lookup"><span data-stu-id="54352-143">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="54352-144">Der Benutzer, die das Programmsteuerelement erstellt.</span><span class="sxs-lookup"><span data-stu-id="54352-144">The user who created the program control.</span></span>                                               |
| `resource`               |`programResource`       | <span data-ttu-id="54352-145">Die Ressource, eine Gruppe oder eine app, Ziel dieses Programm Steuerelement Access überprüfen.</span><span class="sxs-lookup"><span data-stu-id="54352-145">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="54352-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="54352-146">Relationships</span></span>
| <span data-ttu-id="54352-147">Beziehung</span><span class="sxs-lookup"><span data-stu-id="54352-147">Relationship</span></span> | <span data-ttu-id="54352-148">Typ</span><span class="sxs-lookup"><span data-stu-id="54352-148">Type</span></span>   |<span data-ttu-id="54352-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54352-149">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="54352-150">Programm</span><span class="sxs-lookup"><span data-stu-id="54352-150">program</span></span>](program.md)               | <span data-ttu-id="54352-151">Die Anwendung dieses Steuerelement ist Bestandteil.</span><span class="sxs-lookup"><span data-stu-id="54352-151">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="54352-152">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="54352-152">See also</span></span>

| <span data-ttu-id="54352-153">Methode</span><span class="sxs-lookup"><span data-stu-id="54352-153">Method</span></span>           | <span data-ttu-id="54352-154">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="54352-154">Return Type</span></span>    |<span data-ttu-id="54352-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54352-155">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54352-156">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="54352-156">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="54352-157">[ProgramControl](programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="54352-157">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="54352-158">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="54352-158">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="54352-159">Liste programControlTypes</span><span class="sxs-lookup"><span data-stu-id="54352-159">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="54352-160">[ProgramControlType](programcontroltype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="54352-160">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="54352-161">Programm Steuerelement Listentypen.</span><span class="sxs-lookup"><span data-stu-id="54352-161">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54352-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="54352-162">JSON representation</span></span>

<span data-ttu-id="54352-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="54352-163">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": "microsoft.graph.userIdentity",
 "resource":"microsoft.graph.programResource"
}

```

## <a name="the-programresource-complex-type"></a><span data-ttu-id="54352-164">Den komplexen Typ programResource</span><span class="sxs-lookup"><span data-stu-id="54352-164">The programResource complex type</span></span>

<span data-ttu-id="54352-165">Die Programm-Ressource, die ein Programm Control-Objekt enthaltenen ist eine Darstellung der einen Verweis auf ein Objekt, das das Ziel der Überprüfung Zugriff ist.</span><span class="sxs-lookup"><span data-stu-id="54352-165">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="54352-166">Dieser Typ erbt von `microsoft.graph.identity` und verfügt über eine zusätzliche Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="54352-166">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="54352-167">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54352-167">Property</span></span>     | <span data-ttu-id="54352-168">Typ</span><span class="sxs-lookup"><span data-stu-id="54352-168">Type</span></span>   |<span data-ttu-id="54352-169">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54352-169">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="54352-170">Der Typ der Ressource, zurück, der angibt, ob es sich um eine Gruppe oder eine app handelt.</span><span class="sxs-lookup"><span data-stu-id="54352-170">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!-- {
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->