---
title: mobileAppContent-Ressourcentyp
description: Enthält Inhaltseigenschaften für eine bestimmte App-Version. Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cde82585bdbe4ca4c15102e6b343810f29fdae8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261299"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="2b917-104">mobileAppContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2b917-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="2b917-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2b917-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b917-106">Enthält Inhaltseigenschaften für eine bestimmte App-Version.</span><span class="sxs-lookup"><span data-stu-id="2b917-106">Contains content properties for a specific app version.</span></span> <span data-ttu-id="2b917-107">Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.</span><span class="sxs-lookup"><span data-stu-id="2b917-107">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>

## <a name="methods"></a><span data-ttu-id="2b917-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="2b917-108">Methods</span></span>
|<span data-ttu-id="2b917-109">Methode</span><span class="sxs-lookup"><span data-stu-id="2b917-109">Method</span></span>|<span data-ttu-id="2b917-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2b917-110">Return Type</span></span>|<span data-ttu-id="2b917-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b917-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2b917-112">mobileAppContents auflisten</span><span class="sxs-lookup"><span data-stu-id="2b917-112">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="2b917-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2b917-113">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="2b917-114">Auflisten von Eigenschaften und Beziehungen der [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="2b917-114">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="2b917-115">mobileAppContent abrufen</span><span class="sxs-lookup"><span data-stu-id="2b917-115">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="2b917-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2b917-116">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2b917-117">Lesen von Eigenschaften und Beziehungen des [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b917-117">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="2b917-118">mobileAppContent erstellen</span><span class="sxs-lookup"><span data-stu-id="2b917-118">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="2b917-119">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2b917-119">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2b917-120">Erstellen eines neuen [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b917-120">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="2b917-121">mobileAppContent löschen</span><span class="sxs-lookup"><span data-stu-id="2b917-121">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="2b917-122">Keine</span><span class="sxs-lookup"><span data-stu-id="2b917-122">None</span></span>|<span data-ttu-id="2b917-123">Löscht eine [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="2b917-123">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="2b917-124">Update mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2b917-124">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="2b917-125">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="2b917-125">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="2b917-126">Aktualisieren der Eigenschaften eines [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b917-126">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2b917-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2b917-127">Properties</span></span>
|<span data-ttu-id="2b917-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2b917-128">Property</span></span>|<span data-ttu-id="2b917-129">Typ</span><span class="sxs-lookup"><span data-stu-id="2b917-129">Type</span></span>|<span data-ttu-id="2b917-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b917-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b917-131">id</span><span class="sxs-lookup"><span data-stu-id="2b917-131">id</span></span>|<span data-ttu-id="2b917-132">String</span><span class="sxs-lookup"><span data-stu-id="2b917-132">String</span></span>|<span data-ttu-id="2b917-133">Die Version des App-Inhalts.</span><span class="sxs-lookup"><span data-stu-id="2b917-133">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b917-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2b917-134">Relationships</span></span>
|<span data-ttu-id="2b917-135">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2b917-135">Relationship</span></span>|<span data-ttu-id="2b917-136">Typ</span><span class="sxs-lookup"><span data-stu-id="2b917-136">Type</span></span>|<span data-ttu-id="2b917-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b917-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b917-138">files</span><span class="sxs-lookup"><span data-stu-id="2b917-138">files</span></span>|<span data-ttu-id="2b917-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2b917-139">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="2b917-140">Die Liste der Dateien für diese App-Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="2b917-140">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b917-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2b917-141">JSON Representation</span></span>
<span data-ttu-id="2b917-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2b917-142">Here is a JSON representation of the resource.</span></span>
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



