---
title: termsAndConditionsAssignment-Ressourcentyp
description: Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 309136805a6d5e41a5aee8e20cc80b6d7665ef66
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156063"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="f05db-104">termsAndConditionsAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f05db-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="f05db-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f05db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f05db-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f05db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f05db-107">Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe.</span><span class="sxs-lookup"><span data-stu-id="f05db-107">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="f05db-108">Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.</span><span class="sxs-lookup"><span data-stu-id="f05db-108">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="f05db-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="f05db-109">Methods</span></span>
|<span data-ttu-id="f05db-110">Methode</span><span class="sxs-lookup"><span data-stu-id="f05db-110">Method</span></span>|<span data-ttu-id="f05db-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f05db-111">Return Type</span></span>|<span data-ttu-id="f05db-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f05db-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f05db-113">termsAndConditionsAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="f05db-113">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="f05db-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f05db-114">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="f05db-115">Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="f05db-115">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="f05db-116">termsAndConditionsAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="f05db-116">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="f05db-117">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f05db-117">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="f05db-118">Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f05db-118">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="f05db-119">termsAndConditionsAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="f05db-119">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="f05db-120">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f05db-120">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="f05db-121">Erstellen eines neuen [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f05db-121">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="f05db-122">termsAndConditionsAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="f05db-122">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="f05db-123">Keine</span><span class="sxs-lookup"><span data-stu-id="f05db-123">None</span></span>|<span data-ttu-id="f05db-124">Löscht ein [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f05db-124">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="f05db-125">termsAndConditionsAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f05db-125">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="f05db-126">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f05db-126">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="f05db-127">Aktualisieren der Eigenschaften eines [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f05db-127">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f05db-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f05db-128">Properties</span></span>
|<span data-ttu-id="f05db-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f05db-129">Property</span></span>|<span data-ttu-id="f05db-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f05db-130">Type</span></span>|<span data-ttu-id="f05db-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f05db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f05db-132">id</span><span class="sxs-lookup"><span data-stu-id="f05db-132">id</span></span>|<span data-ttu-id="f05db-133">String</span><span class="sxs-lookup"><span data-stu-id="f05db-133">String</span></span>|<span data-ttu-id="f05db-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="f05db-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f05db-135">target</span><span class="sxs-lookup"><span data-stu-id="f05db-135">target</span></span>|[<span data-ttu-id="f05db-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f05db-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f05db-137">Zuweisungsziel, dem die Richtlinie der Nutzungsbedingungen zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="f05db-137">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f05db-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f05db-138">Relationships</span></span>
<span data-ttu-id="f05db-139">Keine</span><span class="sxs-lookup"><span data-stu-id="f05db-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f05db-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f05db-140">JSON Representation</span></span>
<span data-ttu-id="f05db-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f05db-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




