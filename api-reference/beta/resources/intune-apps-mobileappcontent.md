---
title: mobileAppContent-Ressourcentyp
description: Enthält Inhaltseigenschaften für eine bestimmte App-Version. Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 82c2100fb7bd9e906bf6cf9092d3df88865c26e8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153445"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="2a8a6-104">mobileAppContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2a8a6-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="2a8a6-105">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a8a6-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a8a6-107">Enthält Inhaltseigenschaften für eine bestimmte App-Version.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-107">Contains content properties for a specific app version.</span></span> <span data-ttu-id="2a8a6-108">Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-108">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="2a8a6-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="2a8a6-109">Methods</span></span>
|<span data-ttu-id="2a8a6-110">Methode</span><span class="sxs-lookup"><span data-stu-id="2a8a6-110">Method</span></span>|<span data-ttu-id="2a8a6-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2a8a6-111">Return Type</span></span>|<span data-ttu-id="2a8a6-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a8a6-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2a8a6-113">mobileAppContents auflisten</span><span class="sxs-lookup"><span data-stu-id="2a8a6-113">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="2a8a6-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2a8a6-114">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="2a8a6-115">Auflisten von Eigenschaften und Beziehungen der [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-115">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="2a8a6-116">mobileAppContent abrufen</span><span class="sxs-lookup"><span data-stu-id="2a8a6-116">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="2a8a6-117">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2a8a6-117">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2a8a6-118">Lesen von Eigenschaften und Beziehungen des [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-118">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="2a8a6-119">mobileAppContent erstellen</span><span class="sxs-lookup"><span data-stu-id="2a8a6-119">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="2a8a6-120">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2a8a6-120">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2a8a6-121">Erstellen eines neuen [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-121">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="2a8a6-122">mobileAppContent löschen</span><span class="sxs-lookup"><span data-stu-id="2a8a6-122">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="2a8a6-123">Keine</span><span class="sxs-lookup"><span data-stu-id="2a8a6-123">None</span></span>|<span data-ttu-id="2a8a6-124">Löscht eine [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-124">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="2a8a6-125">Update mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2a8a6-125">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="2a8a6-126">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2a8a6-126">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2a8a6-127">Aktualisieren der Eigenschaften eines [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-127">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a8a6-128">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2a8a6-128">Properties</span></span>
|<span data-ttu-id="2a8a6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a8a6-129">Property</span></span>|<span data-ttu-id="2a8a6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2a8a6-130">Type</span></span>|<span data-ttu-id="2a8a6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a8a6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a8a6-132">id</span><span class="sxs-lookup"><span data-stu-id="2a8a6-132">id</span></span>|<span data-ttu-id="2a8a6-133">String</span><span class="sxs-lookup"><span data-stu-id="2a8a6-133">String</span></span>|<span data-ttu-id="2a8a6-134">Die Version des App-Inhalts.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-134">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a8a6-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2a8a6-135">Relationships</span></span>
|<span data-ttu-id="2a8a6-136">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2a8a6-136">Relationship</span></span>|<span data-ttu-id="2a8a6-137">Typ</span><span class="sxs-lookup"><span data-stu-id="2a8a6-137">Type</span></span>|<span data-ttu-id="2a8a6-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a8a6-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a8a6-139">files</span><span class="sxs-lookup"><span data-stu-id="2a8a6-139">files</span></span>|<span data-ttu-id="2a8a6-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2a8a6-140">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="2a8a6-141">Die Liste der Dateien für diese App-Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-141">The list of files for this app content version.</span></span>|
|<span data-ttu-id="2a8a6-142">containedApps</span><span class="sxs-lookup"><span data-stu-id="2a8a6-142">containedApps</span></span>|<span data-ttu-id="2a8a6-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="2a8a6-143">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="2a8a6-144">Die Sammlung der enthaltenen apps in einem MobileLobApp, das als Paket fungiert.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-144">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a8a6-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2a8a6-145">JSON Representation</span></span>
<span data-ttu-id="2a8a6-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a8a6-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```




