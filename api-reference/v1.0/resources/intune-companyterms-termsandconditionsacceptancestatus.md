---
title: termsAndConditionsAcceptanceStatus-Ressourcentyp
description: C) Richtlinie von einem bestimmten Benutzer. Benutzer müssen die neueste Version der Geschäftsbedingungen akzeptieren, um weiterhin Zugriff auf das Unternehmensportal zu haben.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17d76be4db1f790d00fb90322307ff04152291be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849392"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="400d9-104">termsAndConditionsAcceptanceStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="400d9-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="400d9-105">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="400d9-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="400d9-106">Eine termsAndConditionsAcceptanceStatus-Entität stellt den Annahmestatus einer bestimmten Geschäftsbedingungen-Richtlinie durch einen bestimmten Benutzer dar.</span><span class="sxs-lookup"><span data-stu-id="400d9-106">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="400d9-107">Benutzer müssen die neueste Version der Geschäftsbedingungen akzeptieren, um weiterhin Zugriff auf das Unternehmensportal zu haben.</span><span class="sxs-lookup"><span data-stu-id="400d9-107">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="400d9-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="400d9-108">Methods</span></span>
|<span data-ttu-id="400d9-109">Methode</span><span class="sxs-lookup"><span data-stu-id="400d9-109">Method</span></span>|<span data-ttu-id="400d9-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="400d9-110">Return Type</span></span>|<span data-ttu-id="400d9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="400d9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="400d9-112">termsAndConditionsAcceptanceStatuses auflisten</span><span class="sxs-lookup"><span data-stu-id="400d9-112">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="400d9-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="400d9-113">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="400d9-114">Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="400d9-114">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="400d9-115">termsAndConditionsAcceptanceStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="400d9-115">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="400d9-116">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="400d9-116">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="400d9-117">Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="400d9-117">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="400d9-118">termsAndConditionsAcceptanceStatus erstellen</span><span class="sxs-lookup"><span data-stu-id="400d9-118">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="400d9-119">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="400d9-119">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="400d9-120">Erstellen eines neuen [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="400d9-120">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="400d9-121">termsAndConditionsAcceptanceStatus löschen</span><span class="sxs-lookup"><span data-stu-id="400d9-121">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="400d9-122">Keine</span><span class="sxs-lookup"><span data-stu-id="400d9-122">None</span></span>|<span data-ttu-id="400d9-123">Löscht ein [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="400d9-123">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="400d9-124">termsAndConditionsAcceptanceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="400d9-124">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="400d9-125">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="400d9-125">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="400d9-126">Aktualisieren der Eigenschaften eines [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="400d9-126">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="400d9-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="400d9-127">Properties</span></span>
|<span data-ttu-id="400d9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="400d9-128">Property</span></span>|<span data-ttu-id="400d9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="400d9-129">Type</span></span>|<span data-ttu-id="400d9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="400d9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="400d9-131">id</span><span class="sxs-lookup"><span data-stu-id="400d9-131">id</span></span>|<span data-ttu-id="400d9-132">String</span><span class="sxs-lookup"><span data-stu-id="400d9-132">String</span></span>|<span data-ttu-id="400d9-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="400d9-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="400d9-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="400d9-134">userDisplayName</span></span>|<span data-ttu-id="400d9-135">String</span><span class="sxs-lookup"><span data-stu-id="400d9-135">String</span></span>|<span data-ttu-id="400d9-136">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="400d9-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="400d9-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="400d9-137">acceptedVersion</span></span>|<span data-ttu-id="400d9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="400d9-138">Int32</span></span>|<span data-ttu-id="400d9-139">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="400d9-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="400d9-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="400d9-140">acceptedDateTime</span></span>|<span data-ttu-id="400d9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="400d9-141">DateTimeOffset</span></span>|<span data-ttu-id="400d9-142">Datum und Uhrzeit, zu der die Nutzungsbedingungen zuletzt vom Benutzer akzeptiert wurden.</span><span class="sxs-lookup"><span data-stu-id="400d9-142">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="400d9-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="400d9-143">Relationships</span></span>
|<span data-ttu-id="400d9-144">Beziehung</span><span class="sxs-lookup"><span data-stu-id="400d9-144">Relationship</span></span>|<span data-ttu-id="400d9-145">Typ</span><span class="sxs-lookup"><span data-stu-id="400d9-145">Type</span></span>|<span data-ttu-id="400d9-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="400d9-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="400d9-147">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="400d9-147">termsAndConditions</span></span>|[<span data-ttu-id="400d9-148">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="400d9-148">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="400d9-149">Navigationslink zu den Geschäftsbedingungen, die zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="400d9-149">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="400d9-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="400d9-150">JSON Representation</span></span>
<span data-ttu-id="400d9-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="400d9-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```



