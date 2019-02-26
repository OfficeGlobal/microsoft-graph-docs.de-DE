---
title: deviceCategory-Ressourcentyp
description: Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden. Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75fb11ef3b734e6d5d0490be1abc3c5399433a70
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174552"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="744b1-104">deviceCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="744b1-104">deviceCategory resource type</span></span>

> <span data-ttu-id="744b1-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="744b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="744b1-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="744b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="744b1-107">Gerätekategorien bieten eine Möglichkeit zum Organisieren Ihrer Geräte.</span><span class="sxs-lookup"><span data-stu-id="744b1-107">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="744b1-108">Unter Verwendung von Gerätekategorien können Unternehmensadministratoren eindeutige Kategorien definieren, die für Ihr Unternehmen sinnvoll sind.</span><span class="sxs-lookup"><span data-stu-id="744b1-108">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="744b1-109">Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="744b1-109"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="744b1-110">Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.</span><span class="sxs-lookup"><span data-stu-id="744b1-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="744b1-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="744b1-111">Methods</span></span>
|<span data-ttu-id="744b1-112">Methode</span><span class="sxs-lookup"><span data-stu-id="744b1-112">Method</span></span>|<span data-ttu-id="744b1-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="744b1-113">Return Type</span></span>|<span data-ttu-id="744b1-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="744b1-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="744b1-115">deviceCategories auflisten</span><span class="sxs-lookup"><span data-stu-id="744b1-115">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="744b1-116">[deviceCategory](../resources/intune-shared-devicecategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="744b1-116">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="744b1-117">Auflisten von Eigenschaften und Beziehungen der [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="744b1-117">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="744b1-118">deviceCategory abrufen</span><span class="sxs-lookup"><span data-stu-id="744b1-118">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="744b1-119">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="744b1-119">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="744b1-120">Lesen von Eigenschaften und Beziehungen des [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="744b1-120">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="744b1-121">deviceCategory erstellen</span><span class="sxs-lookup"><span data-stu-id="744b1-121">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="744b1-122">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="744b1-122">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="744b1-123">Erstellen eines neuen [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="744b1-123">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="744b1-124">deviceCategory löschen</span><span class="sxs-lookup"><span data-stu-id="744b1-124">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="744b1-125">Keine</span><span class="sxs-lookup"><span data-stu-id="744b1-125">None</span></span>|<span data-ttu-id="744b1-126">Löscht ein [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="744b1-126">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="744b1-127">deviceCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="744b1-127">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="744b1-128">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="744b1-128">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="744b1-129">Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts</span><span class="sxs-lookup"><span data-stu-id="744b1-129">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="744b1-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="744b1-130">Properties</span></span>
|<span data-ttu-id="744b1-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="744b1-131">Property</span></span>|<span data-ttu-id="744b1-132">Typ</span><span class="sxs-lookup"><span data-stu-id="744b1-132">Type</span></span>|<span data-ttu-id="744b1-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="744b1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="744b1-134">id</span><span class="sxs-lookup"><span data-stu-id="744b1-134">id</span></span>|<span data-ttu-id="744b1-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="744b1-135">String</span></span>|<span data-ttu-id="744b1-136">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="744b1-136">Unique identifier for the device category.</span></span> <span data-ttu-id="744b1-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="744b1-137">Read-only.</span></span>|
|<span data-ttu-id="744b1-138">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="744b1-138">**Onboarding**</span></span>|
|<span data-ttu-id="744b1-139">displayName</span><span class="sxs-lookup"><span data-stu-id="744b1-139">displayName</span></span>|<span data-ttu-id="744b1-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="744b1-140">String</span></span>|<span data-ttu-id="744b1-141">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="744b1-141">Display name for the device category.</span></span>|
|<span data-ttu-id="744b1-142">description</span><span class="sxs-lookup"><span data-stu-id="744b1-142">description</span></span>|<span data-ttu-id="744b1-143">String</span><span class="sxs-lookup"><span data-stu-id="744b1-143">String</span></span>|<span data-ttu-id="744b1-144">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="744b1-144">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="744b1-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="744b1-145">Relationships</span></span>
<span data-ttu-id="744b1-146">Keine</span><span class="sxs-lookup"><span data-stu-id="744b1-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="744b1-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="744b1-147">JSON Representation</span></span>
<span data-ttu-id="744b1-148">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="744b1-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



