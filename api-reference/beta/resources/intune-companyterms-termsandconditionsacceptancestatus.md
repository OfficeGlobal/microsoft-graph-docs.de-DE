---
title: termsAndConditionsAcceptanceStatus-Ressourcentyp
description: C) Richtlinie von einem bestimmten Benutzer. Benutzer müssen die neueste Version der Geschäftsbedingungen akzeptieren, um weiterhin Zugriff auf das Unternehmensportal zu haben.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1c66b7ba799def675ab3b74ad2ea9b8ce2f7ec22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961078"
---
# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="1dbd3-104">termsAndConditionsAcceptanceStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1dbd3-104">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="1dbd3-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dbd3-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1dbd3-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1dbd3-108">Eine termsAndConditionsAcceptanceStatus-Entität stellt den Annahmestatus einer bestimmten Geschäftsbedingungen-Richtlinie durch einen bestimmten Benutzer dar.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-108">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="1dbd3-109">Benutzer müssen die neueste Version der Geschäftsbedingungen akzeptieren, um weiterhin Zugriff auf das Unternehmensportal zu haben.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-109">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="1dbd3-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="1dbd3-110">Methods</span></span>
|<span data-ttu-id="1dbd3-111">Methode</span><span class="sxs-lookup"><span data-stu-id="1dbd3-111">Method</span></span>|<span data-ttu-id="1dbd3-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1dbd3-112">Return Type</span></span>|<span data-ttu-id="1dbd3-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1dbd3-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1dbd3-114">termsAndConditionsAcceptanceStatuses auflisten</span><span class="sxs-lookup"><span data-stu-id="1dbd3-114">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-list.md)|<span data-ttu-id="1dbd3-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="1dbd3-115">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="1dbd3-116">Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-116">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="1dbd3-117">termsAndConditionsAcceptanceStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="1dbd3-117">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-get.md)|[<span data-ttu-id="1dbd3-118">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1dbd3-118">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="1dbd3-119">Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-119">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="1dbd3-120">termsAndConditionsAcceptanceStatus erstellen</span><span class="sxs-lookup"><span data-stu-id="1dbd3-120">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-create.md)|[<span data-ttu-id="1dbd3-121">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1dbd3-121">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="1dbd3-122">Erstellen eines neuen [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-122">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="1dbd3-123">termsAndConditionsAcceptanceStatus löschen</span><span class="sxs-lookup"><span data-stu-id="1dbd3-123">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-delete.md)|<span data-ttu-id="1dbd3-124">Keine</span><span class="sxs-lookup"><span data-stu-id="1dbd3-124">None</span></span>|<span data-ttu-id="1dbd3-125">Löscht ein [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-125">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="1dbd3-126">termsAndConditionsAcceptanceStatus aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1dbd3-126">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune-companyterms-termsandconditionsacceptancestatus-update.md)|[<span data-ttu-id="1dbd3-127">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="1dbd3-127">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|<span data-ttu-id="1dbd3-128">Aktualisieren der Eigenschaften eines [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-128">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1dbd3-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1dbd3-129">Properties</span></span>
|<span data-ttu-id="1dbd3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1dbd3-130">Property</span></span>|<span data-ttu-id="1dbd3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1dbd3-131">Type</span></span>|<span data-ttu-id="1dbd3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1dbd3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dbd3-133">id</span><span class="sxs-lookup"><span data-stu-id="1dbd3-133">id</span></span>|<span data-ttu-id="1dbd3-134">String</span><span class="sxs-lookup"><span data-stu-id="1dbd3-134">String</span></span>|<span data-ttu-id="1dbd3-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="1dbd3-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1dbd3-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1dbd3-136">userDisplayName</span></span>|<span data-ttu-id="1dbd3-137">String</span><span class="sxs-lookup"><span data-stu-id="1dbd3-137">String</span></span>|<span data-ttu-id="1dbd3-138">Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt</span><span class="sxs-lookup"><span data-stu-id="1dbd3-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="1dbd3-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="1dbd3-139">acceptedVersion</span></span>|<span data-ttu-id="1dbd3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1dbd3-140">Int32</span></span>|<span data-ttu-id="1dbd3-141">Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="1dbd3-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="1dbd3-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dbd3-142">acceptedDateTime</span></span>|<span data-ttu-id="1dbd3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dbd3-143">DateTimeOffset</span></span>|<span data-ttu-id="1dbd3-144">Datum und Uhrzeit, zu der die Nutzungsbedingungen zuletzt vom Benutzer akzeptiert wurden.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-144">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dbd3-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1dbd3-145">Relationships</span></span>
|<span data-ttu-id="1dbd3-146">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1dbd3-146">Relationship</span></span>|<span data-ttu-id="1dbd3-147">Typ</span><span class="sxs-lookup"><span data-stu-id="1dbd3-147">Type</span></span>|<span data-ttu-id="1dbd3-148">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1dbd3-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dbd3-149">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="1dbd3-149">termsAndConditions</span></span>|[<span data-ttu-id="1dbd3-150">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="1dbd3-150">termsAndConditions</span></span>](../resources/intune-companyterms-termsandconditions.md)|<span data-ttu-id="1dbd3-151">Navigationslink zu den Geschäftsbedingungen, die zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-151">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1dbd3-152">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1dbd3-152">JSON Representation</span></span>
<span data-ttu-id="1dbd3-153">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-153">Here is a JSON representation of the resource.</span></span>
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





