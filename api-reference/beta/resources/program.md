---
title: Programm Ressourcentyp
description: 'In Azure AD Access Feature überprüft, ein Programm ist ein Container, Programm Steuerelemente halten. Ein Mandant kann eine oder mehrere Programme verfügen.  Jedes Steuerelement verknüpft eine Überprüfung Zugriff auf ein Programm, um zugehörige Access findet erleichtern überprüft.  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515188"
---
# <a name="program-resource-type"></a><span data-ttu-id="02bd2-105">Programm Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="02bd2-105">program resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02bd2-106">In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion ist ein Programm einen Container, halten Programm Steuerelemente.</span><span class="sxs-lookup"><span data-stu-id="02bd2-106">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="02bd2-107">Ein Mandant kann eine oder mehrere Programme verfügen.</span><span class="sxs-lookup"><span data-stu-id="02bd2-107">A tenant can have one or more programs.</span></span>  <span data-ttu-id="02bd2-108">Jedes Steuerelement verknüpft eine Überprüfung Zugriff auf ein Programm, um zugehörige Access findet erleichtern überprüft.</span><span class="sxs-lookup"><span data-stu-id="02bd2-108">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="02bd2-109">Jeder Mandant, die auf-Azure AD an hat Zugriff Bewertungen hat ein Programm `Default program`.</span><span class="sxs-lookup"><span data-stu-id="02bd2-109">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="02bd2-110">Ein globaler Administrator kann zusätzliche Programme, beispielsweise zum Darstellen der Compliance-Initiativen erstellen.</span><span class="sxs-lookup"><span data-stu-id="02bd2-110">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="02bd2-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="02bd2-111">Methods</span></span>

| <span data-ttu-id="02bd2-112">Methode</span><span class="sxs-lookup"><span data-stu-id="02bd2-112">Method</span></span>           | <span data-ttu-id="02bd2-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="02bd2-113">Return Type</span></span>    |<span data-ttu-id="02bd2-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02bd2-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02bd2-115">Erstellen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="02bd2-115">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="02bd2-116">Programm</span><span class="sxs-lookup"><span data-stu-id="02bd2-116">program</span></span>](program.md)   |   <span data-ttu-id="02bd2-117">Erstellen Sie ein neues Programm.</span><span class="sxs-lookup"><span data-stu-id="02bd2-117">Create a new program.</span></span>|
|[<span data-ttu-id="02bd2-118">Programm löschen</span><span class="sxs-lookup"><span data-stu-id="02bd2-118">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="02bd2-119">Keine.</span><span class="sxs-lookup"><span data-stu-id="02bd2-119">None.</span></span>   |   <span data-ttu-id="02bd2-120">Löschen eines Programms.</span><span class="sxs-lookup"><span data-stu-id="02bd2-120">Delete a program.</span></span>|
|[<span data-ttu-id="02bd2-121">Programme auflisten</span><span class="sxs-lookup"><span data-stu-id="02bd2-121">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="02bd2-122">[Programm](program.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="02bd2-122">[program](program.md) collection</span></span>|   <span data-ttu-id="02bd2-123">Rufen Sie eine Auflistung aller Programme.</span><span class="sxs-lookup"><span data-stu-id="02bd2-123">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="02bd2-124">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="02bd2-124">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="02bd2-125">[ProgramControl](programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="02bd2-125">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="02bd2-126">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="02bd2-126">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="02bd2-127">Update-Programm</span><span class="sxs-lookup"><span data-stu-id="02bd2-127">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="02bd2-128">Programm</span><span class="sxs-lookup"><span data-stu-id="02bd2-128">program</span></span>](program.md)|  <span data-ttu-id="02bd2-129">Aktualisieren eines Programms.</span><span class="sxs-lookup"><span data-stu-id="02bd2-129">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="02bd2-130">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="02bd2-130">Permissions</span></span>

|<span data-ttu-id="02bd2-131">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02bd2-131">Permission type</span></span>                        | <span data-ttu-id="02bd2-132">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02bd2-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="02bd2-133">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02bd2-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="02bd2-134">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02bd2-134">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="02bd2-135">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02bd2-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02bd2-136">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02bd2-136">Not supported.</span></span> |
|<span data-ttu-id="02bd2-137">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02bd2-137">Application</span></span>                            | <span data-ttu-id="02bd2-138">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="02bd2-138">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="02bd2-139">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="02bd2-139">Properties</span></span>
| <span data-ttu-id="02bd2-140">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02bd2-140">Property</span></span>     | <span data-ttu-id="02bd2-141">Typ</span><span class="sxs-lookup"><span data-stu-id="02bd2-141">Type</span></span>   |<span data-ttu-id="02bd2-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02bd2-142">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="02bd2-143">Das Feature zugewiesenen Bezeichner des Programms.</span><span class="sxs-lookup"><span data-stu-id="02bd2-143">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="02bd2-144">Der Name des Programms.</span><span class="sxs-lookup"><span data-stu-id="02bd2-144">The name of the program.</span></span>  <span data-ttu-id="02bd2-145">Erforderliche auf erstellen.</span><span class="sxs-lookup"><span data-stu-id="02bd2-145">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="02bd2-146">Die Beschreibung des Programms.</span><span class="sxs-lookup"><span data-stu-id="02bd2-146">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="02bd2-147">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="02bd2-147">Relationships</span></span>
| <span data-ttu-id="02bd2-148">Beziehung</span><span class="sxs-lookup"><span data-stu-id="02bd2-148">Relationship</span></span> | <span data-ttu-id="02bd2-149">Typ</span><span class="sxs-lookup"><span data-stu-id="02bd2-149">Type</span></span>   |<span data-ttu-id="02bd2-150">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02bd2-150">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="02bd2-151">programControl</span><span class="sxs-lookup"><span data-stu-id="02bd2-151">programControl</span></span>](programcontrol.md) | <span data-ttu-id="02bd2-152">Steuerelemente, die das Programm zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="02bd2-152">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02bd2-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="02bd2-153">JSON representation</span></span>

<span data-ttu-id="02bd2-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="02bd2-154">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/program.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
