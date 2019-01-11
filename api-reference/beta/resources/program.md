---
title: Programm Ressourcentyp
description: 'In Azure AD Access Feature überprüft, ein Programm ist ein Container, Programm Steuerelemente halten. Ein Mandant kann eine oder mehrere Programme verfügen.  Jedes Steuerelement verknüpft eine Überprüfung Zugriff auf ein Programm, um zugehörige Access findet erleichtern überprüft.  '
localization_priority: Normal
ms.openlocfilehash: a342fd159bba3f7e31c55ffab9a64a72353bc7ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863903"
---
# <a name="program-resource-type"></a><span data-ttu-id="9be98-105">Programm Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9be98-105">program resource type</span></span>

> <span data-ttu-id="9be98-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9be98-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9be98-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9be98-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9be98-108">In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion ist ein Programm einen Container, halten Programm Steuerelemente.</span><span class="sxs-lookup"><span data-stu-id="9be98-108">In the Azure AD [access reviews](accessreviews-root.md) feature, a program is a container, holding program controls.</span></span> <span data-ttu-id="9be98-109">Ein Mandant kann eine oder mehrere Programme verfügen.</span><span class="sxs-lookup"><span data-stu-id="9be98-109">A tenant can have one or more programs.</span></span>  <span data-ttu-id="9be98-110">Jedes Steuerelement verknüpft eine Überprüfung Zugriff auf ein Programm, um zugehörige Access findet erleichtern überprüft.</span><span class="sxs-lookup"><span data-stu-id="9be98-110">Each control links an access review to a program, to make it easier to locate related access reviews.</span></span>  

<span data-ttu-id="9be98-111">Jeder Mandant, die auf-Azure AD an hat Zugriff Bewertungen hat ein Programm `Default program`.</span><span class="sxs-lookup"><span data-stu-id="9be98-111">Each tenant that has on-boarded Azure AD access reviews has one program, `Default program`.</span></span>  <span data-ttu-id="9be98-112">Ein globaler Administrator kann zusätzliche Programme, beispielsweise zum Darstellen der Compliance-Initiativen erstellen.</span><span class="sxs-lookup"><span data-stu-id="9be98-112">A global administrator can create additional programs, for example to represent compliance initiatives.</span></span> 


## <a name="methods"></a><span data-ttu-id="9be98-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="9be98-113">Methods</span></span>

| <span data-ttu-id="9be98-114">Methode</span><span class="sxs-lookup"><span data-stu-id="9be98-114">Method</span></span>           | <span data-ttu-id="9be98-115">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9be98-115">Return Type</span></span>    |<span data-ttu-id="9be98-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9be98-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9be98-117">Erstellen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="9be98-117">Create program</span></span>](../api/program-create.md) |   [<span data-ttu-id="9be98-118">Programm</span><span class="sxs-lookup"><span data-stu-id="9be98-118">program</span></span>](program.md)   |   <span data-ttu-id="9be98-119">Erstellen Sie ein neues Programm.</span><span class="sxs-lookup"><span data-stu-id="9be98-119">Create a new program.</span></span>|
|[<span data-ttu-id="9be98-120">Programm löschen</span><span class="sxs-lookup"><span data-stu-id="9be98-120">Delete program</span></span>](../api/program-delete.md) |   <span data-ttu-id="9be98-121">Keine.</span><span class="sxs-lookup"><span data-stu-id="9be98-121">None.</span></span>   |   <span data-ttu-id="9be98-122">Löschen eines Programms.</span><span class="sxs-lookup"><span data-stu-id="9be98-122">Delete a program.</span></span>|
|[<span data-ttu-id="9be98-123">Programme auflisten</span><span class="sxs-lookup"><span data-stu-id="9be98-123">List programs</span></span>](../api/program-list.md) |  <span data-ttu-id="9be98-124">[Programm](program.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9be98-124">[program](program.md) collection</span></span>|   <span data-ttu-id="9be98-125">Rufen Sie eine Auflistung aller Programme.</span><span class="sxs-lookup"><span data-stu-id="9be98-125">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="9be98-126">Liste ProgramControls eines Programms</span><span class="sxs-lookup"><span data-stu-id="9be98-126">List programControls of a program</span></span>](../api/program-listcontrols.md) |      <span data-ttu-id="9be98-127">[ProgramControl](programcontrol.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9be98-127">[programControl](programcontrol.md) collection</span></span>| <span data-ttu-id="9be98-128">Rufen Sie eine Auflistung der Steuerelemente eines Programms.</span><span class="sxs-lookup"><span data-stu-id="9be98-128">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="9be98-129">Update-Programm</span><span class="sxs-lookup"><span data-stu-id="9be98-129">Update program</span></span>](../api/program-update.md) |   [<span data-ttu-id="9be98-130">Programm</span><span class="sxs-lookup"><span data-stu-id="9be98-130">program</span></span>](program.md)|  <span data-ttu-id="9be98-131">Aktualisieren eines Programms.</span><span class="sxs-lookup"><span data-stu-id="9be98-131">Update a program.</span></span>|

## <a name="permissions"></a><span data-ttu-id="9be98-132">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9be98-132">Permissions</span></span>

|<span data-ttu-id="9be98-133">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9be98-133">Permission type</span></span>                        | <span data-ttu-id="9be98-134">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9be98-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9be98-135">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9be98-135">Delegated (work or school account)</span></span>     | <span data-ttu-id="9be98-136">ProgramControl.Read.All ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9be98-136">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span> |
|<span data-ttu-id="9be98-137">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9be98-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9be98-138">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9be98-138">Not supported.</span></span> |
|<span data-ttu-id="9be98-139">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9be98-139">Application</span></span>                            | <span data-ttu-id="9be98-140">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9be98-140">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="9be98-141">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9be98-141">Properties</span></span>
| <span data-ttu-id="9be98-142">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9be98-142">Property</span></span>     | <span data-ttu-id="9be98-143">Typ</span><span class="sxs-lookup"><span data-stu-id="9be98-143">Type</span></span>   |<span data-ttu-id="9be98-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9be98-144">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  <span data-ttu-id="9be98-145">Das Feature zugewiesenen Bezeichner des Programms.</span><span class="sxs-lookup"><span data-stu-id="9be98-145">The feature-assigned identifier of the program.</span></span>                    |
| `displayName`               |`String`                              |  <span data-ttu-id="9be98-146">Der Name des Programms.</span><span class="sxs-lookup"><span data-stu-id="9be98-146">The name of the program.</span></span>  <span data-ttu-id="9be98-147">Erforderliche auf erstellen.</span><span class="sxs-lookup"><span data-stu-id="9be98-147">Required on create.</span></span>                  |
| `description`               |`String`                              |  <span data-ttu-id="9be98-148">Die Beschreibung des Programms.</span><span class="sxs-lookup"><span data-stu-id="9be98-148">The description of the program.</span></span>           |

## <a name="relationships"></a><span data-ttu-id="9be98-149">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9be98-149">Relationships</span></span>
| <span data-ttu-id="9be98-150">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9be98-150">Relationship</span></span> | <span data-ttu-id="9be98-151">Typ</span><span class="sxs-lookup"><span data-stu-id="9be98-151">Type</span></span>   |<span data-ttu-id="9be98-152">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9be98-152">Description</span></span>|
|:---------------|:--------|:----------|
| `controls`                  |[<span data-ttu-id="9be98-153">programControl</span><span class="sxs-lookup"><span data-stu-id="9be98-153">programControl</span></span>](programcontrol.md) | <span data-ttu-id="9be98-154">Steuerelemente, die das Programm zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="9be98-154">Controls associated with the program.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9be98-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9be98-155">JSON representation</span></span>

<span data-ttu-id="9be98-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9be98-156">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
