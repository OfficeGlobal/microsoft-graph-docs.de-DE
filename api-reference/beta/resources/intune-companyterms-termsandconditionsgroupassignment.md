---
title: Ressourcentyp termsAndConditionsGroupAssignment
description: C) Richtlinie zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
author: tfitzmac
ms.openlocfilehash: 044d82e00e2da81c59de5cdb26b9441da351db8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327615"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="3609b-104">Ressourcentyp termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3609b-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="3609b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3609b-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3609b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3609b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3609b-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3609b-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3609b-108">Eine Entität TermsAndConditionsGroupAssignment stellt die Zuweisung einer bestimmten Geschäftsbedingungen (T & C) Richtlinie zu einer bestimmten Gruppe.</span><span class="sxs-lookup"><span data-stu-id="3609b-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="3609b-109">Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.</span><span class="sxs-lookup"><span data-stu-id="3609b-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="3609b-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="3609b-110">Methods</span></span>
|<span data-ttu-id="3609b-111">Methode</span><span class="sxs-lookup"><span data-stu-id="3609b-111">Method</span></span>|<span data-ttu-id="3609b-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3609b-112">Return Type</span></span>|<span data-ttu-id="3609b-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3609b-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3609b-114">Liste termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="3609b-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="3609b-115">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3609b-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="3609b-116">Listeneigenschaften und Beziehungen der [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="3609b-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="3609b-117">Abrufen von termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3609b-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="3609b-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3609b-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="3609b-119">Lesen Sie Eigenschaften und Beziehungen des [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3609b-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="3609b-120">Erstellen von termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3609b-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="3609b-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3609b-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="3609b-122">Erstellen eines neuen [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3609b-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="3609b-123">TermsAndConditionsGroupAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="3609b-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="3609b-124">Keines</span><span class="sxs-lookup"><span data-stu-id="3609b-124">None</span></span>|<span data-ttu-id="3609b-125">Löscht eine [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3609b-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="3609b-126">TermsAndConditionsGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3609b-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="3609b-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="3609b-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="3609b-128">Aktualisieren Sie die Eigenschaften eines [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3609b-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3609b-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3609b-129">Properties</span></span>
|<span data-ttu-id="3609b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3609b-130">Property</span></span>|<span data-ttu-id="3609b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3609b-131">Type</span></span>|<span data-ttu-id="3609b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3609b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3609b-133">id</span><span class="sxs-lookup"><span data-stu-id="3609b-133">id</span></span>|<span data-ttu-id="3609b-134">String</span><span class="sxs-lookup"><span data-stu-id="3609b-134">String</span></span>|<span data-ttu-id="3609b-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="3609b-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="3609b-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="3609b-136">targetGroupId</span></span>|<span data-ttu-id="3609b-137">String</span><span class="sxs-lookup"><span data-stu-id="3609b-137">String</span></span>|<span data-ttu-id="3609b-138">Eindeutiger Bezeichner der einer Gruppe, der die Richtlinie T & C zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="3609b-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3609b-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3609b-139">Relationships</span></span>
|<span data-ttu-id="3609b-140">Beziehung</span><span class="sxs-lookup"><span data-stu-id="3609b-140">Relationship</span></span>|<span data-ttu-id="3609b-141">Typ</span><span class="sxs-lookup"><span data-stu-id="3609b-141">Type</span></span>|<span data-ttu-id="3609b-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3609b-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3609b-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3609b-143">termsAndConditions</span></span>|[<span data-ttu-id="3609b-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3609b-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="3609b-145">Navigationslink zu den Geschäftsbedingungen, die zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="3609b-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3609b-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3609b-146">JSON Representation</span></span>
<span data-ttu-id="3609b-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3609b-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```





