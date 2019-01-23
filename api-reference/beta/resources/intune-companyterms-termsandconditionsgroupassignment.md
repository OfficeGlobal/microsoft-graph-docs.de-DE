---
title: Ressourcentyp termsAndConditionsGroupAssignment
description: Eine Entität TermsAndConditionsGroupAssignment stellt die Zuordnung von einer angegebenen Geschäftsbedingungen (T&C) Richtlinie zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0cdb629c380898af078bf0b5eaeb3c39344a5657
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418575"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a><span data-ttu-id="6d828-104">Ressourcentyp termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6d828-104">termsAndConditionsGroupAssignment resource type</span></span>

> <span data-ttu-id="6d828-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6d828-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6d828-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6d828-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d828-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6d828-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d828-108">Eine Entität TermsAndConditionsGroupAssignment stellt die Zuordnung von einer angegebenen Geschäftsbedingungen (T&C) Richtlinie zu einer bestimmten Gruppe.</span><span class="sxs-lookup"><span data-stu-id="6d828-108">A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="6d828-109">Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.</span><span class="sxs-lookup"><span data-stu-id="6d828-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="6d828-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="6d828-110">Methods</span></span>
|<span data-ttu-id="6d828-111">Methode</span><span class="sxs-lookup"><span data-stu-id="6d828-111">Method</span></span>|<span data-ttu-id="6d828-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6d828-112">Return Type</span></span>|<span data-ttu-id="6d828-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d828-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6d828-114">Liste termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="6d828-114">List termsAndConditionsGroupAssignments</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|<span data-ttu-id="6d828-115">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="6d828-115">[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) collection</span></span>|<span data-ttu-id="6d828-116">Listeneigenschaften und Beziehungen der [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="6d828-116">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>|
|[<span data-ttu-id="6d828-117">Abrufen von termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6d828-117">Get termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[<span data-ttu-id="6d828-118">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6d828-118">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="6d828-119">Lesen Sie Eigenschaften und Beziehungen des [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d828-119">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="6d828-120">Erstellen von termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6d828-120">Create termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[<span data-ttu-id="6d828-121">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6d828-121">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="6d828-122">Erstellen eines neuen [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d828-122">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|
|[<span data-ttu-id="6d828-123">TermsAndConditionsGroupAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="6d828-123">Delete termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|<span data-ttu-id="6d828-124">Keine</span><span class="sxs-lookup"><span data-stu-id="6d828-124">None</span></span>|<span data-ttu-id="6d828-125">Löscht eine [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6d828-125">Deletes a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).</span></span>|
|[<span data-ttu-id="6d828-126">TermsAndConditionsGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6d828-126">Update termsAndConditionsGroupAssignment</span></span>](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[<span data-ttu-id="6d828-127">termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="6d828-127">termsAndConditionsGroupAssignment</span></span>](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|<span data-ttu-id="6d828-128">Aktualisieren Sie die Eigenschaften eines [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6d828-128">Update the properties of a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d828-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6d828-129">Properties</span></span>
|<span data-ttu-id="6d828-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d828-130">Property</span></span>|<span data-ttu-id="6d828-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6d828-131">Type</span></span>|<span data-ttu-id="6d828-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d828-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d828-133">id</span><span class="sxs-lookup"><span data-stu-id="6d828-133">id</span></span>|<span data-ttu-id="6d828-134">String</span><span class="sxs-lookup"><span data-stu-id="6d828-134">String</span></span>|<span data-ttu-id="6d828-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="6d828-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="6d828-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="6d828-136">targetGroupId</span></span>|<span data-ttu-id="6d828-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d828-137">String</span></span>|<span data-ttu-id="6d828-138">Eindeutiger Bezeichner der einer Gruppe, der die T&C Richtlinie zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="6d828-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d828-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6d828-139">Relationships</span></span>
|<span data-ttu-id="6d828-140">Beziehung</span><span class="sxs-lookup"><span data-stu-id="6d828-140">Relationship</span></span>|<span data-ttu-id="6d828-141">Typ</span><span class="sxs-lookup"><span data-stu-id="6d828-141">Type</span></span>|<span data-ttu-id="6d828-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d828-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d828-143">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6d828-143">termsAndConditions</span></span>|[<span data-ttu-id="6d828-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="6d828-144">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="6d828-145">Navigationslink zu den Geschäftsbedingungen, die zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="6d828-145">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d828-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6d828-146">JSON Representation</span></span>
<span data-ttu-id="6d828-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6d828-147">Here is a JSON representation of the resource.</span></span>
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




