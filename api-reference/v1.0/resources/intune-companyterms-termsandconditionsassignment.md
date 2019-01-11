---
title: termsAndConditionsAssignment-Ressourcentyp
description: C) Richtlinie zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ba87e7b5f3b39f20befb1536f3a87583437eeee3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889369"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="6ade9-104">termsAndConditionsAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6ade9-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="6ade9-105">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6ade9-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ade9-106">Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe.</span><span class="sxs-lookup"><span data-stu-id="6ade9-106">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="6ade9-107">Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.</span><span class="sxs-lookup"><span data-stu-id="6ade9-107">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="6ade9-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="6ade9-108">Methods</span></span>
|<span data-ttu-id="6ade9-109">Methode</span><span class="sxs-lookup"><span data-stu-id="6ade9-109">Method</span></span>|<span data-ttu-id="6ade9-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="6ade9-110">Return Type</span></span>|<span data-ttu-id="6ade9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ade9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6ade9-112">termsAndConditionsAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="6ade9-112">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="6ade9-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="6ade9-113">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="6ade9-114">Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="6ade9-114">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="6ade9-115">termsAndConditionsAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="6ade9-115">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="6ade9-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6ade9-116">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="6ade9-117">Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6ade9-117">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="6ade9-118">termsAndConditionsAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="6ade9-118">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="6ade9-119">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6ade9-119">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="6ade9-120">Erstellen eines neuen [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6ade9-120">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="6ade9-121">termsAndConditionsAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="6ade9-121">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="6ade9-122">Keine</span><span class="sxs-lookup"><span data-stu-id="6ade9-122">None</span></span>|<span data-ttu-id="6ade9-123">Löscht ein [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6ade9-123">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="6ade9-124">termsAndConditionsAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6ade9-124">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="6ade9-125">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="6ade9-125">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="6ade9-126">Aktualisieren der Eigenschaften eines [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6ade9-126">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ade9-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ade9-127">Properties</span></span>
|<span data-ttu-id="6ade9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ade9-128">Property</span></span>|<span data-ttu-id="6ade9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6ade9-129">Type</span></span>|<span data-ttu-id="6ade9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ade9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ade9-131">id</span><span class="sxs-lookup"><span data-stu-id="6ade9-131">id</span></span>|<span data-ttu-id="6ade9-132">String</span><span class="sxs-lookup"><span data-stu-id="6ade9-132">String</span></span>|<span data-ttu-id="6ade9-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="6ade9-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="6ade9-134">target</span><span class="sxs-lookup"><span data-stu-id="6ade9-134">target</span></span>|[<span data-ttu-id="6ade9-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6ade9-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6ade9-136">Zuweisungsziel, dem die Richtlinie der Nutzungsbedingungen zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="6ade9-136">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ade9-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6ade9-137">Relationships</span></span>
<span data-ttu-id="6ade9-138">Keine</span><span class="sxs-lookup"><span data-stu-id="6ade9-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ade9-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ade9-139">JSON Representation</span></span>
<span data-ttu-id="6ade9-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ade9-140">Here is a JSON representation of the resource.</span></span>
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



