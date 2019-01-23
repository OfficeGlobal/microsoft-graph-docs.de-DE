---
title: termsAndConditionsAcceptanceStatus-Ressourcentyp
description: Eine termsAndConditionsAcceptanceStatus-Entität stellt den Annahmestatus einer bestimmten Geschäftsbedingungen-Richtlinie durch einen bestimmten Benutzer dar. Benutzer müssen die neueste Version der Geschäftsbedingungen akzeptieren, um weiterhin Zugriff auf das Unternehmensportal zu haben.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e6156c1f5cf952f485e6f0a210a7aef4bd7b3ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412555"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="bcb6c-104">termsAndConditionsAcceptanceStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bcb6c-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="bcb6c-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bcb6c-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bcb6c-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcb6c-108">Eine termsAndConditionsAcceptanceStatus-Entität stellt den Annahmestatus einer bestimmten Geschäftsbedingungen-Richtlinie durch einen bestimmten Benutzer dar.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="bcb6c-109">Benutzer müssen die neueste Version der Geschäftsbedingungen akzeptieren, um weiterhin Zugriff auf das Unternehmensportal zu haben.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>

## <a name="methods"></a><span data-ttu-id="bcb6c-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="bcb6c-110">Methods</span></span>
|<span data-ttu-id="bcb6c-111">Methode</span><span class="sxs-lookup"><span data-stu-id="bcb6c-111">Method</span></span>|<span data-ttu-id="bcb6c-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bcb6c-112">Return Type</span></span>|<span data-ttu-id="bcb6c-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bcb6c-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bcb6c-114">termsAndConditionsAcceptanceStatuses auflisten</span><span class="sxs-lookup"><span data-stu-id="bcb6c-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="bcb6c-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bcb6c-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="bcb6c-116">Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="bcb6c-117">termsAndConditionsAcceptanceStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="bcb6c-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="bcb6c-118">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="bcb6c-118">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="bcb6c-119">Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="bcb6c-120">termsAndConditionsAcceptanceStatus erstellen</span><span class="sxs-lookup"><span data-stu-id="bcb6c-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="bcb6c-121">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="bcb6c-121">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="bcb6c-122">Erstellen eines neuen [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="bcb6c-123">termsAndConditionsAcceptanceStatus löschen</span><span class="sxs-lookup"><span data-stu-id="bcb6c-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="bcb6c-124">Keine</span><span class="sxs-lookup"><span data-stu-id="bcb6c-124">None</span></span>|<span data-ttu-id="bcb6c-125">Löscht ein [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="bcb6c-126">termsAndConditionsAcceptanceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bcb6c-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="bcb6c-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="bcb6c-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="bcb6c-128">Aktualisieren der Eigenschaften eines [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bcb6c-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bcb6c-129">Properties</span></span>
|<span data-ttu-id="bcb6c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bcb6c-130">Property</span></span>|<span data-ttu-id="bcb6c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bcb6c-131">Type</span></span>|<span data-ttu-id="bcb6c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bcb6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcb6c-133">id</span><span class="sxs-lookup"><span data-stu-id="bcb6c-133">id</span></span>|<span data-ttu-id="bcb6c-134">String</span><span class="sxs-lookup"><span data-stu-id="bcb6c-134">String</span></span>|<span data-ttu-id="bcb6c-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="bcb6c-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="bcb6c-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="bcb6c-136">userDisplayName</span></span>|<span data-ttu-id="bcb6c-137">String</span><span class="sxs-lookup"><span data-stu-id="bcb6c-137">String</span></span>|<span data-ttu-id="bcb6c-138">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="bcb6c-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="bcb6c-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="bcb6c-139">acceptedVersion</span></span>|<span data-ttu-id="bcb6c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bcb6c-140">Int32</span></span>|<span data-ttu-id="bcb6c-141">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="bcb6c-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="bcb6c-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcb6c-142">acceptedDateTime</span></span>|<span data-ttu-id="bcb6c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcb6c-143">DateTimeOffset</span></span>|<span data-ttu-id="bcb6c-144">Datum und Uhrzeit, zu der die Nutzungsbedingungen zuletzt vom Benutzer akzeptiert wurden.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-144">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcb6c-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bcb6c-145">Relationships</span></span>
|<span data-ttu-id="bcb6c-146">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bcb6c-146">Relationship</span></span>|<span data-ttu-id="bcb6c-147">Typ</span><span class="sxs-lookup"><span data-stu-id="bcb6c-147">Type</span></span>|<span data-ttu-id="bcb6c-148">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bcb6c-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcb6c-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="bcb6c-149">termsAndConditions</span></span>|[<span data-ttu-id="bcb6c-150">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="bcb6c-150">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="bcb6c-151">Navigationslink zu den Geschäftsbedingungen, die zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-151">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcb6c-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bcb6c-152">JSON Representation</span></span>
<span data-ttu-id="bcb6c-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bcb6c-153">Here is a JSON representation of the resource.</span></span>
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




