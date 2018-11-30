---
title: termsAndConditionsAssignment-Ressourcentyp
description: C) Richtlinie zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
ms.openlocfilehash: 848998e59f214fc679aba7c27a2a529be05c8adc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018793"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="5778b-104">termsAndConditionsAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5778b-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="5778b-105">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5778b-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5778b-106">Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe.</span><span class="sxs-lookup"><span data-stu-id="5778b-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="5778b-107">Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.</span><span class="sxs-lookup"><span data-stu-id="5778b-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="5778b-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="5778b-108">Methods</span></span>
|<span data-ttu-id="5778b-109">Methode</span><span class="sxs-lookup"><span data-stu-id="5778b-109">Method</span></span>|<span data-ttu-id="5778b-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5778b-110">Return Type</span></span>|<span data-ttu-id="5778b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5778b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5778b-112">termsAndConditionsAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="5778b-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="5778b-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5778b-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="5778b-114">Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="5778b-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="5778b-115">termsAndConditionsAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="5778b-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="5778b-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5778b-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="5778b-117">Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5778b-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="5778b-118">termsAndConditionsAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="5778b-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="5778b-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5778b-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="5778b-120">Erstellen eines neuen [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5778b-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="5778b-121">termsAndConditionsAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="5778b-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="5778b-122">Keine</span><span class="sxs-lookup"><span data-stu-id="5778b-122">None</span></span>|<span data-ttu-id="5778b-123">Löscht ein [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5778b-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="5778b-124">termsAndConditionsAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5778b-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="5778b-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="5778b-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="5778b-126">Aktualisieren der Eigenschaften eines [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5778b-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5778b-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5778b-127">Properties</span></span>
|<span data-ttu-id="5778b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5778b-128">Property</span></span>|<span data-ttu-id="5778b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5778b-129">Type</span></span>|<span data-ttu-id="5778b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5778b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5778b-131">id</span><span class="sxs-lookup"><span data-stu-id="5778b-131">id</span></span>|<span data-ttu-id="5778b-132">String</span><span class="sxs-lookup"><span data-stu-id="5778b-132">String</span></span>|<span data-ttu-id="5778b-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="5778b-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5778b-134">target</span><span class="sxs-lookup"><span data-stu-id="5778b-134">target</span></span>|[<span data-ttu-id="5778b-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5778b-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5778b-136">Zuweisungsziel, dem die Richtlinie der Nutzungsbedingungen zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="5778b-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5778b-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5778b-137">Relationships</span></span>
<span data-ttu-id="5778b-138">Keine</span><span class="sxs-lookup"><span data-stu-id="5778b-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5778b-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5778b-139">JSON Representation</span></span>
<span data-ttu-id="5778b-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5778b-140">Here is a JSON representation of the resource.</span></span>
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



