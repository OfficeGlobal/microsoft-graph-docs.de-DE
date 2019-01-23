---
title: termsAndConditionsAssignment-Ressourcentyp
description: Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2de08d2bc90061ed4096a9a010b332872eb36ef
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422026"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="f9418-104">termsAndConditionsAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f9418-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="f9418-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f9418-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f9418-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9418-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9418-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f9418-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9418-108">Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe.</span><span class="sxs-lookup"><span data-stu-id="f9418-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="f9418-109">Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.</span><span class="sxs-lookup"><span data-stu-id="f9418-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>

## <a name="methods"></a><span data-ttu-id="f9418-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="f9418-110">Methods</span></span>
|<span data-ttu-id="f9418-111">Methode</span><span class="sxs-lookup"><span data-stu-id="f9418-111">Method</span></span>|<span data-ttu-id="f9418-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f9418-112">Return Type</span></span>|<span data-ttu-id="f9418-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9418-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f9418-114">termsAndConditionsAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="f9418-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="f9418-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="f9418-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="f9418-116">Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="f9418-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="f9418-117">termsAndConditionsAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="f9418-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="f9418-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f9418-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="f9418-119">Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9418-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="f9418-120">termsAndConditionsAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="f9418-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="f9418-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f9418-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="f9418-122">Erstellen eines neuen [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9418-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="f9418-123">termsAndConditionsAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="f9418-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="f9418-124">Keine</span><span class="sxs-lookup"><span data-stu-id="f9418-124">None</span></span>|<span data-ttu-id="f9418-125">Löscht ein [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f9418-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="f9418-126">termsAndConditionsAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f9418-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="f9418-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="f9418-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="f9418-128">Aktualisieren der Eigenschaften eines [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f9418-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f9418-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f9418-129">Properties</span></span>
|<span data-ttu-id="f9418-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9418-130">Property</span></span>|<span data-ttu-id="f9418-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f9418-131">Type</span></span>|<span data-ttu-id="f9418-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9418-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9418-133">id</span><span class="sxs-lookup"><span data-stu-id="f9418-133">id</span></span>|<span data-ttu-id="f9418-134">String</span><span class="sxs-lookup"><span data-stu-id="f9418-134">String</span></span>|<span data-ttu-id="f9418-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="f9418-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="f9418-136">target</span><span class="sxs-lookup"><span data-stu-id="f9418-136">target</span></span>|[<span data-ttu-id="f9418-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f9418-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f9418-138">Zuweisungsziel, dem die Richtlinie der Nutzungsbedingungen zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="f9418-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9418-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f9418-139">Relationships</span></span>
<span data-ttu-id="f9418-140">Keine</span><span class="sxs-lookup"><span data-stu-id="f9418-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9418-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f9418-141">JSON Representation</span></span>
<span data-ttu-id="f9418-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9418-142">Here is a JSON representation of the resource.</span></span>
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




