---
title: Ressourcentyp programControl
description: In Azure AD Access Feature überprüft, und das Programm Control-Objekt stellt ein Steuerelement, Verknüpfen einer Access-Überprüfung an ein Programm dar.
localization_priority: Normal
ms.openlocfilehash: 82d9263a909fb11e688ffa6b27f0cf92601ae9e9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576556"
---
# <a name="programcontrol-resource-type"></a><span data-ttu-id="5c639-103">Ressourcentyp programControl</span><span class="sxs-lookup"><span data-stu-id="5c639-103">programControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c639-104">In Azure AD [Access überprüft](accessreviews-root.md) Feature stellt das Programm Control-Objekt ein Steuerelement, Verknüpfen einer Access-Überprüfung mit einer Anwendung.</span><span class="sxs-lookup"><span data-stu-id="5c639-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control object represents a control, linking an access review to a program.</span></span>


## <a name="methods"></a><span data-ttu-id="5c639-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="5c639-105">Methods</span></span>

| <span data-ttu-id="5c639-106">Methode</span><span class="sxs-lookup"><span data-stu-id="5c639-106">Method</span></span>           | <span data-ttu-id="5c639-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5c639-107">Return Type</span></span>    |<span data-ttu-id="5c639-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c639-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5c639-109">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="5c639-109">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="5c639-110">programControl</span><span class="sxs-lookup"><span data-stu-id="5c639-110">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="5c639-111">Fügen Sie ein Programm ein ProgramControl hinzu.</span><span class="sxs-lookup"><span data-stu-id="5c639-111">Add a programControl to a program.</span></span>|
|[<span data-ttu-id="5c639-112">ProgramControl löschen</span><span class="sxs-lookup"><span data-stu-id="5c639-112">Delete programControl</span></span>](../api/programcontrol-delete.md) |     <span data-ttu-id="5c639-113">Keine.</span><span class="sxs-lookup"><span data-stu-id="5c639-113">None.</span></span>   |   <span data-ttu-id="5c639-114">Entfernen einer ProgramControl aus einem Programm.</span><span class="sxs-lookup"><span data-stu-id="5c639-114">Remove a programControl from a program.</span></span>|
|[<span data-ttu-id="5c639-115">Liste programControls</span><span class="sxs-lookup"><span data-stu-id="5c639-115">List programControls</span></span>](../api/programcontrol-list.md) | <span data-ttu-id="5c639-116">[ProgramControl](programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5c639-116">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="5c639-117">Von Listensteuerelementen in allen Programmen im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5c639-117">List controls across all programs in the tenant.</span></span>|

## <a name="permissions"></a><span data-ttu-id="5c639-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5c639-118">Permissions</span></span>

|<span data-ttu-id="5c639-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c639-119">Permission type</span></span>                        | <span data-ttu-id="5c639-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c639-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c639-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c639-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c639-122">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c639-122">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="5c639-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c639-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c639-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c639-124">Not supported.</span></span> |
|<span data-ttu-id="5c639-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c639-125">Application</span></span>                            | <span data-ttu-id="5c639-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c639-126">Not supported.</span></span> |

## <a name="properties"></a><span data-ttu-id="5c639-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5c639-127">Properties</span></span>
| <span data-ttu-id="5c639-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c639-128">Property</span></span>     | <span data-ttu-id="5c639-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5c639-129">Type</span></span>   |<span data-ttu-id="5c639-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c639-130">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="5c639-131">Die Feature-zugewiesenen Bezeichner der Verknüpfung zwischen Programm und Steuerelement</span><span class="sxs-lookup"><span data-stu-id="5c639-131">The feature-assigned identifier of the link between program and control</span></span>                                      |
| `programId`              |`String`                | <span data-ttu-id="5c639-132">Die ProgramId des Programms dieses Steuerelement ist ein Teil der.</span><span class="sxs-lookup"><span data-stu-id="5c639-132">The programId of the program this control is a part of.</span></span> <span data-ttu-id="5c639-133">Erforderliche auf erstellen.</span><span class="sxs-lookup"><span data-stu-id="5c639-133">Required on create.</span></span>                            |
| `controlId`              |`String`                | <span data-ttu-id="5c639-134">Die ControlId des Steuerelements, insbesondere die eine Access-ID überprüfen.</span><span class="sxs-lookup"><span data-stu-id="5c639-134">The controlId of the control, in particular the identifier of an access review.</span></span> <span data-ttu-id="5c639-135">Erforderliche auf erstellen.</span><span class="sxs-lookup"><span data-stu-id="5c639-135">Required on create.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="5c639-136">Die ProgramControlType identifiziert den Typ des programmfreigabesteuerung – beispielsweise ein Steuerelement verknüpfen mit Gast Access überprüft.</span><span class="sxs-lookup"><span data-stu-id="5c639-136">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> <span data-ttu-id="5c639-137">Erforderliche auf erstellen.</span><span class="sxs-lookup"><span data-stu-id="5c639-137">Required on create.</span></span> |
| `displayName`            |`String`                | <span data-ttu-id="5c639-138">Der Name des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="5c639-138">The name of the control.</span></span>                                                             |
| `status`                 |`String`                | <span data-ttu-id="5c639-139">Der Status des Lebenszyklus des Steuerelements.</span><span class="sxs-lookup"><span data-stu-id="5c639-139">The life cycle status of the control.</span></span>                                                 |
| `createdDateTime`        |`DateTimeOffset`        | <span data-ttu-id="5c639-140">Das Erstellungsdatum und die Uhrzeit des Steuerelements Programm.</span><span class="sxs-lookup"><span data-stu-id="5c639-140">The creation date and time of the program control.</span></span>                                        |
| `owner`                  |[<span data-ttu-id="5c639-141">Benutzeridentität</span><span class="sxs-lookup"><span data-stu-id="5c639-141">userIdentity</span></span>](useridentity.md)   | <span data-ttu-id="5c639-142">Der Benutzer, die das Programmsteuerelement erstellt.</span><span class="sxs-lookup"><span data-stu-id="5c639-142">The user who created the program control.</span></span>                                               |
| `resource`               | [<span data-ttu-id="5c639-143">programResource</span><span class="sxs-lookup"><span data-stu-id="5c639-143">programResource</span></span>](programresource.md)       | <span data-ttu-id="5c639-144">Die Ressource, eine Gruppe oder eine app, Ziel dieses Programm Steuerelement Access überprüfen.</span><span class="sxs-lookup"><span data-stu-id="5c639-144">The resource, a group or an app, targeted by this program control's access review.</span></span>                   |

## <a name="relationships"></a><span data-ttu-id="5c639-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5c639-145">Relationships</span></span>
| <span data-ttu-id="5c639-146">Beziehung</span><span class="sxs-lookup"><span data-stu-id="5c639-146">Relationship</span></span> | <span data-ttu-id="5c639-147">Typ</span><span class="sxs-lookup"><span data-stu-id="5c639-147">Type</span></span>   |<span data-ttu-id="5c639-148">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c639-148">Description</span></span>|
|:---------------|:--------|:----------|
| `program`                |[<span data-ttu-id="5c639-149">Programm</span><span class="sxs-lookup"><span data-stu-id="5c639-149">program</span></span>](program.md)               | <span data-ttu-id="5c639-150">Die Anwendung dieses Steuerelement ist Bestandteil.</span><span class="sxs-lookup"><span data-stu-id="5c639-150">The program this control is part of.</span></span>                                                |

## <a name="see-also"></a><span data-ttu-id="5c639-151">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5c639-151">See also</span></span>

| <span data-ttu-id="5c639-152">Methode</span><span class="sxs-lookup"><span data-stu-id="5c639-152">Method</span></span>           | <span data-ttu-id="5c639-153">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5c639-153">Return Type</span></span>    |<span data-ttu-id="5c639-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c639-154">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5c639-155">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="5c639-155">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="5c639-156">[ProgramControl](programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5c639-156">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="5c639-157">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="5c639-157">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="5c639-158">Liste programControlTypes</span><span class="sxs-lookup"><span data-stu-id="5c639-158">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="5c639-159">[ProgramControlType](programcontroltype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5c639-159">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="5c639-160">Programm Steuerelement Listentypen.</span><span class="sxs-lookup"><span data-stu-id="5c639-160">List program control types.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5c639-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5c639-161">JSON representation</span></span>

<span data-ttu-id="5c639-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5c639-162">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-programresource-complex-type"></a><span data-ttu-id="5c639-163">Den komplexen Typ programResource</span><span class="sxs-lookup"><span data-stu-id="5c639-163">The programResource complex type</span></span>

<span data-ttu-id="5c639-164">Die Programm-Ressource, die ein Programm Control-Objekt enthaltenen ist eine Darstellung der einen Verweis auf ein Objekt, das das Ziel der Überprüfung Zugriff ist.</span><span class="sxs-lookup"><span data-stu-id="5c639-164">The program resource, contained within a program control object, is a representation of a reference to an object which is the target of the access review.</span></span>

<span data-ttu-id="5c639-165">Dieser Typ erbt von `microsoft.graph.identity` und verfügt über eine zusätzliche Eigenschaft:</span><span class="sxs-lookup"><span data-stu-id="5c639-165">This type inherits from `microsoft.graph.identity` and has one additional property:</span></span>

| <span data-ttu-id="5c639-166">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c639-166">Property</span></span>     | <span data-ttu-id="5c639-167">Typ</span><span class="sxs-lookup"><span data-stu-id="5c639-167">Type</span></span>   |<span data-ttu-id="5c639-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c639-168">Description</span></span>|
|:---------------|:--------|:----------|
| `type`               |`String`  | <span data-ttu-id="5c639-169">Der Typ der Ressource, zurück, der angibt, ob es sich um eine Gruppe oder eine app handelt.</span><span class="sxs-lookup"><span data-stu-id="5c639-169">Type of the resource, indicating whether it is a group or an app.</span></span> |     


<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontrol.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
