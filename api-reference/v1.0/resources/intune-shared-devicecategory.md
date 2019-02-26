---
title: deviceCategory-Ressourcentyp
description: Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden. Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a0bb1e994bcf42ba91a55fdfc75946204d1f9b06
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254898"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="ea473-104">deviceCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ea473-104">deviceCategory resource type</span></span>

> <span data-ttu-id="ea473-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ea473-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea473-106">Gerätekategorien bieten eine Möglichkeit zum Organisieren Ihrer Geräte.</span><span class="sxs-lookup"><span data-stu-id="ea473-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="ea473-107">Mithilfe von Gerätekategorien können Unternehmensadministratoren eigene Kategorien definieren, die für ihr Unternehmen sinnvoll sind.</span><span class="sxs-lookup"><span data-stu-id="ea473-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="ea473-108">Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="ea473-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="ea473-109">Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.</span><span class="sxs-lookup"><span data-stu-id="ea473-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="ea473-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="ea473-110">Methods</span></span>
|<span data-ttu-id="ea473-111">Methode</span><span class="sxs-lookup"><span data-stu-id="ea473-111">Method</span></span>|<span data-ttu-id="ea473-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ea473-112">Return Type</span></span>|<span data-ttu-id="ea473-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea473-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea473-114">[DeviceCategories](../api/intune-shared-devicecategory-list.md) -Auflistung auflisten</span><span class="sxs-lookup"><span data-stu-id="ea473-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="ea473-115">Auflisten von Eigenschaften und Beziehungen der [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="ea473-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="ea473-116">deviceCategory abrufen</span><span class="sxs-lookup"><span data-stu-id="ea473-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="ea473-117">Lesen von Eigenschaften und Beziehungen des [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea473-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="ea473-118">deviceCategory erstellen</span><span class="sxs-lookup"><span data-stu-id="ea473-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="ea473-119">Erstellen eines neuen [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ea473-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="ea473-120">[DeviceCategory löschen](../api/intune-shared-devicecategory-delete.md).</span><span class="sxs-lookup"><span data-stu-id="ea473-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="ea473-121">deviceCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ea473-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="ea473-122">Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts</span><span class="sxs-lookup"><span data-stu-id="ea473-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea473-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ea473-123">Properties</span></span>
|<span data-ttu-id="ea473-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea473-124">Property</span></span>|<span data-ttu-id="ea473-125">Typ</span><span class="sxs-lookup"><span data-stu-id="ea473-125">Type</span></span>|<span data-ttu-id="ea473-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea473-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea473-127">id</span><span class="sxs-lookup"><span data-stu-id="ea473-127">id</span></span>|<span data-ttu-id="ea473-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea473-128">String</span></span>|<span data-ttu-id="ea473-129">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="ea473-129">Unique identifier for the device category.</span></span> <span data-ttu-id="ea473-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ea473-130">Read-only.</span></span>|
|<span data-ttu-id="ea473-131">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="ea473-131">**Onboarding**</span></span>|
|<span data-ttu-id="ea473-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ea473-132">displayName</span></span>|<span data-ttu-id="ea473-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea473-133">String</span></span>|<span data-ttu-id="ea473-134">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="ea473-134">Display name for the device category.</span></span>|
|<span data-ttu-id="ea473-135">description</span><span class="sxs-lookup"><span data-stu-id="ea473-135">description</span></span>|<span data-ttu-id="ea473-136">String</span><span class="sxs-lookup"><span data-stu-id="ea473-136">String</span></span>|<span data-ttu-id="ea473-137">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="ea473-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea473-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ea473-138">Relationships</span></span>
<span data-ttu-id="ea473-139">Keine</span><span class="sxs-lookup"><span data-stu-id="ea473-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea473-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ea473-140">JSON Representation</span></span>
<span data-ttu-id="ea473-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ea473-141">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



