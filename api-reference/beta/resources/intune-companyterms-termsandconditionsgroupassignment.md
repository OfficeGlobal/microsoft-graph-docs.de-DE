---
title: termsAndConditionsGroupAssignment-Ressourcentyp
description: Eine termsAndConditionsGroupAssignment-Entität stellt die Zuordnung einer bestimmten Geschäftsbedingungen (T&C) zu einer bestimmten Gruppe dar. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b5b97e691ff16ce2c86057ab5dae229d8657974
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142686"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="d7f60-104">termsAndConditionsGroupAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d7f60-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="d7f60-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d7f60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7f60-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d7f60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7f60-107">Eine termsAndConditionsGroupAssignment-Entität stellt die Zuordnung einer bestimmten Geschäftsbedingungen (T&C) zu einer bestimmten Gruppe dar.</span><span class="sxs-lookup"><span data-stu-id="d7f60-107">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="d7f60-108">Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.</span><span class="sxs-lookup"><span data-stu-id="d7f60-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="d7f60-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="d7f60-109">Methods</span></span>
|<span data-ttu-id="d7f60-110">Methode</span><span class="sxs-lookup"><span data-stu-id="d7f60-110">Method</span></span>|<span data-ttu-id="d7f60-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d7f60-111">Return Type</span></span>|<span data-ttu-id="d7f60-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7f60-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d7f60-113">TermsAndConditionsGroupAssignments aufListen</span><span class="sxs-lookup"><span data-stu-id="d7f60-113">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="d7f60-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d7f60-114">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="d7f60-115">AufListen von Eigenschaften und Beziehungen der [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="d7f60-115">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="d7f60-116">TermsAndConditionsGroupAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="d7f60-116">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="d7f60-117">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d7f60-117">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="d7f60-118">Lesen von Eigenschaften und Beziehungen des [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d7f60-118">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="d7f60-119">TermsAndConditionsGroupAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="d7f60-119">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="d7f60-120">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d7f60-120">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="d7f60-121">Erstellen eines neuen [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d7f60-121">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="d7f60-122">TermsAndConditionsGroupAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="d7f60-122">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="d7f60-123">Keine</span><span class="sxs-lookup"><span data-stu-id="d7f60-123">None</span></span>|<span data-ttu-id="d7f60-124">Löscht eine [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d7f60-124">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="d7f60-125">TermsAndConditionsGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d7f60-125">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="d7f60-126">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d7f60-126">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="d7f60-127">Aktualisieren der Eigenschaften eines [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d7f60-127">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7f60-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d7f60-128">Properties</span></span>
|<span data-ttu-id="d7f60-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d7f60-129">Property</span></span>|<span data-ttu-id="d7f60-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d7f60-130">Type</span></span>|<span data-ttu-id="d7f60-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7f60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7f60-132">id</span><span class="sxs-lookup"><span data-stu-id="d7f60-132">id</span></span>|<span data-ttu-id="d7f60-133">String</span><span class="sxs-lookup"><span data-stu-id="d7f60-133">String</span></span>|<span data-ttu-id="d7f60-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="d7f60-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d7f60-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="d7f60-135">targetGroupId</span></span>|<span data-ttu-id="d7f60-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d7f60-136">String</span></span>|<span data-ttu-id="d7f60-137">Eindeutiger Bezeichner einer Gruppe, der die T&C-Richtlinie zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="d7f60-137">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7f60-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d7f60-138">Relationships</span></span>
|<span data-ttu-id="d7f60-139">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d7f60-139">Relationship</span></span>|<span data-ttu-id="d7f60-140">Typ</span><span class="sxs-lookup"><span data-stu-id="d7f60-140">Type</span></span>|<span data-ttu-id="d7f60-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7f60-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7f60-142">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="d7f60-142">termsAndConditions</span></span>|[<span data-ttu-id="d7f60-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="d7f60-143">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="d7f60-144">Navigationslink zu den Geschäftsbedingungen, die zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="d7f60-144">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7f60-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d7f60-145">JSON Representation</span></span>
<span data-ttu-id="d7f60-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d7f60-146">Here is a JSON representation of the resource.</span></span>
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




