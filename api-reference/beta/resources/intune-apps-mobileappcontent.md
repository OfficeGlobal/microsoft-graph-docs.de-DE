---
title: mobileAppContent-Ressourcentyp
description: Enthält Inhaltseigenschaften für eine bestimmte App-Version. Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ceeb6cd4e989f4e020c885dde119c39d9659539c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418183"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="16064-104">mobileAppContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16064-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="16064-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="16064-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16064-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16064-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16064-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16064-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16064-108">Enthält Inhaltseigenschaften für eine bestimmte App-Version.</span><span class="sxs-lookup"><span data-stu-id="16064-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="16064-109">Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.</span><span class="sxs-lookup"><span data-stu-id="16064-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="16064-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="16064-110">Methods</span></span>
|<span data-ttu-id="16064-111">Methode</span><span class="sxs-lookup"><span data-stu-id="16064-111">Method</span></span>|<span data-ttu-id="16064-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="16064-112">Return Type</span></span>|<span data-ttu-id="16064-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16064-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="16064-114">mobileAppContents auflisten</span><span class="sxs-lookup"><span data-stu-id="16064-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="16064-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="16064-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="16064-116">Auflisten von Eigenschaften und Beziehungen der [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="16064-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="16064-117">mobileAppContent abrufen</span><span class="sxs-lookup"><span data-stu-id="16064-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="16064-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="16064-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="16064-119">Lesen von Eigenschaften und Beziehungen des [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="16064-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="16064-120">mobileAppContent erstellen</span><span class="sxs-lookup"><span data-stu-id="16064-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="16064-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="16064-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="16064-122">Erstellen eines neuen [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="16064-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="16064-123">mobileAppContent löschen</span><span class="sxs-lookup"><span data-stu-id="16064-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="16064-124">Keine</span><span class="sxs-lookup"><span data-stu-id="16064-124">None</span></span>|<span data-ttu-id="16064-125">Löscht eine [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="16064-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="16064-126">Update mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="16064-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="16064-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="16064-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="16064-128">Aktualisieren der Eigenschaften eines [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="16064-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="16064-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16064-129">Properties</span></span>
|<span data-ttu-id="16064-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16064-130">Property</span></span>|<span data-ttu-id="16064-131">Typ</span><span class="sxs-lookup"><span data-stu-id="16064-131">Type</span></span>|<span data-ttu-id="16064-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16064-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16064-133">id</span><span class="sxs-lookup"><span data-stu-id="16064-133">id</span></span>|<span data-ttu-id="16064-134">String</span><span class="sxs-lookup"><span data-stu-id="16064-134">String</span></span>|<span data-ttu-id="16064-135">Die Version des App-Inhalts.</span><span class="sxs-lookup"><span data-stu-id="16064-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16064-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="16064-136">Relationships</span></span>
|<span data-ttu-id="16064-137">Beziehung</span><span class="sxs-lookup"><span data-stu-id="16064-137">Relationship</span></span>|<span data-ttu-id="16064-138">Typ</span><span class="sxs-lookup"><span data-stu-id="16064-138">Type</span></span>|<span data-ttu-id="16064-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16064-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16064-140">files</span><span class="sxs-lookup"><span data-stu-id="16064-140">files</span></span>|<span data-ttu-id="16064-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="16064-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="16064-142">Die Liste der Dateien für diese App-Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="16064-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="16064-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="16064-143">containedApps</span></span>|<span data-ttu-id="16064-144">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="16064-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="16064-145">Die Auflistung der enthaltenen apps in einer MobileLobApp fungiert als Paket.</span><span class="sxs-lookup"><span data-stu-id="16064-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16064-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16064-146">JSON Representation</span></span>
<span data-ttu-id="16064-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="16064-147">Here is a JSON representation of the resource.</span></span>
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




