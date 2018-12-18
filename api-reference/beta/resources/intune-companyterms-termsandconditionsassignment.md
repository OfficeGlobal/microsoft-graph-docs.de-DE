---
title: termsAndConditionsAssignment-Ressourcentyp
description: C) Richtlinie zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
author: tfitzmac
ms.openlocfilehash: a7b0e9deb391b9431be1ed4f282cb6e5a63ced6e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351051"
---
# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="2c16e-104">termsAndConditionsAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2c16e-104">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="2c16e-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2c16e-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c16e-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2c16e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c16e-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2c16e-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c16e-108">Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe.</span><span class="sxs-lookup"><span data-stu-id="2c16e-108">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="2c16e-109">Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.</span><span class="sxs-lookup"><span data-stu-id="2c16e-109">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="2c16e-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="2c16e-110">Methods</span></span>
|<span data-ttu-id="2c16e-111">Methode</span><span class="sxs-lookup"><span data-stu-id="2c16e-111">Method</span></span>|<span data-ttu-id="2c16e-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2c16e-112">Return Type</span></span>|<span data-ttu-id="2c16e-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c16e-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2c16e-114">termsAndConditionsAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="2c16e-114">List termsAndConditionsAssignments</span></span>](../api/intune-companyterms-termsandconditionsassignment-list.md)|<span data-ttu-id="2c16e-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2c16e-115">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="2c16e-116">Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="2c16e-116">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="2c16e-117">termsAndConditionsAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="2c16e-117">Get termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-get.md)|[<span data-ttu-id="2c16e-118">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2c16e-118">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="2c16e-119">Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2c16e-119">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="2c16e-120">termsAndConditionsAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="2c16e-120">Create termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-create.md)|[<span data-ttu-id="2c16e-121">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2c16e-121">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="2c16e-122">Erstellen eines neuen [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2c16e-122">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="2c16e-123">termsAndConditionsAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="2c16e-123">Delete termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-delete.md)|<span data-ttu-id="2c16e-124">Keine</span><span class="sxs-lookup"><span data-stu-id="2c16e-124">None</span></span>|<span data-ttu-id="2c16e-125">Löscht ein [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2c16e-125">Deletes a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="2c16e-126">termsAndConditionsAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2c16e-126">Update termsAndConditionsAssignment</span></span>](../api/intune-companyterms-termsandconditionsassignment-update.md)|[<span data-ttu-id="2c16e-127">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2c16e-127">termsAndConditionsAssignment</span></span>](../resources/intune-companyterms-termsandconditionsassignment.md)|<span data-ttu-id="2c16e-128">Aktualisieren der Eigenschaften eines [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2c16e-128">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c16e-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2c16e-129">Properties</span></span>
|<span data-ttu-id="2c16e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c16e-130">Property</span></span>|<span data-ttu-id="2c16e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2c16e-131">Type</span></span>|<span data-ttu-id="2c16e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c16e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c16e-133">id</span><span class="sxs-lookup"><span data-stu-id="2c16e-133">id</span></span>|<span data-ttu-id="2c16e-134">String</span><span class="sxs-lookup"><span data-stu-id="2c16e-134">String</span></span>|<span data-ttu-id="2c16e-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="2c16e-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="2c16e-136">target</span><span class="sxs-lookup"><span data-stu-id="2c16e-136">target</span></span>|[<span data-ttu-id="2c16e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2c16e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2c16e-138">Zuweisungsziel, dem die Richtlinie der Nutzungsbedingungen zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="2c16e-138">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c16e-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2c16e-139">Relationships</span></span>
<span data-ttu-id="2c16e-140">Keine</span><span class="sxs-lookup"><span data-stu-id="2c16e-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2c16e-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2c16e-141">JSON Representation</span></span>
<span data-ttu-id="2c16e-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2c16e-142">Here is a JSON representation of the resource.</span></span>
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





