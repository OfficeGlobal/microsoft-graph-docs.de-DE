---
title: mobileAppContent-Ressourcentyp
description: Enthält Inhaltseigenschaften für eine bestimmte App-Version. Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aa68d0a07de4f0e85ee15acc189e003c4f4120a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845815"
---
# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="4e6a8-104">mobileAppContent-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4e6a8-104">mobileAppContent resource type</span></span>

> <span data-ttu-id="4e6a8-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e6a8-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e6a8-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e6a8-108">Enthält Inhaltseigenschaften für eine bestimmte App-Version.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-108">Contains content properties for a specific app version.</span></span> <span data-ttu-id="4e6a8-109">Jedes mobileAppContent-Objekt kann mehrere mobileAppContentFile-Objekte haben.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-109">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="4e6a8-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="4e6a8-110">Methods</span></span>
|<span data-ttu-id="4e6a8-111">Methode</span><span class="sxs-lookup"><span data-stu-id="4e6a8-111">Method</span></span>|<span data-ttu-id="4e6a8-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4e6a8-112">Return Type</span></span>|<span data-ttu-id="4e6a8-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e6a8-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4e6a8-114">mobileAppContents auflisten</span><span class="sxs-lookup"><span data-stu-id="4e6a8-114">List mobileAppContents</span></span>](../api/intune-apps-mobileappcontent-list.md)|<span data-ttu-id="4e6a8-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4e6a8-115">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="4e6a8-116">Auflisten von Eigenschaften und Beziehungen der [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-116">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="4e6a8-117">mobileAppContent abrufen</span><span class="sxs-lookup"><span data-stu-id="4e6a8-117">Get mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-get.md)|[<span data-ttu-id="4e6a8-118">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4e6a8-118">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="4e6a8-119">Lesen von Eigenschaften und Beziehungen des [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-119">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="4e6a8-120">mobileAppContent erstellen</span><span class="sxs-lookup"><span data-stu-id="4e6a8-120">Create mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-create.md)|[<span data-ttu-id="4e6a8-121">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4e6a8-121">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="4e6a8-122">Erstellen eines neuen [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-122">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="4e6a8-123">mobileAppContent löschen</span><span class="sxs-lookup"><span data-stu-id="4e6a8-123">Delete mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-delete.md)|<span data-ttu-id="4e6a8-124">Keine</span><span class="sxs-lookup"><span data-stu-id="4e6a8-124">None</span></span>|<span data-ttu-id="4e6a8-125">Löscht eine [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-125">Deletes a [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>|
|[<span data-ttu-id="4e6a8-126">Update mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4e6a8-126">Update mobileAppContent</span></span>](../api/intune-apps-mobileappcontent-update.md)|[<span data-ttu-id="4e6a8-127">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="4e6a8-127">mobileAppContent</span></span>](../resources/intune-apps-mobileappcontent.md)|<span data-ttu-id="4e6a8-128">Aktualisieren der Eigenschaften eines [mobileAppContent](../resources/intune-apps-mobileappcontent.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-128">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4e6a8-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4e6a8-129">Properties</span></span>
|<span data-ttu-id="4e6a8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e6a8-130">Property</span></span>|<span data-ttu-id="4e6a8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4e6a8-131">Type</span></span>|<span data-ttu-id="4e6a8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e6a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e6a8-133">id</span><span class="sxs-lookup"><span data-stu-id="4e6a8-133">id</span></span>|<span data-ttu-id="4e6a8-134">String</span><span class="sxs-lookup"><span data-stu-id="4e6a8-134">String</span></span>|<span data-ttu-id="4e6a8-135">Die Version des App-Inhalts.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-135">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e6a8-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4e6a8-136">Relationships</span></span>
|<span data-ttu-id="4e6a8-137">Beziehung</span><span class="sxs-lookup"><span data-stu-id="4e6a8-137">Relationship</span></span>|<span data-ttu-id="4e6a8-138">Typ</span><span class="sxs-lookup"><span data-stu-id="4e6a8-138">Type</span></span>|<span data-ttu-id="4e6a8-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e6a8-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e6a8-140">files</span><span class="sxs-lookup"><span data-stu-id="4e6a8-140">files</span></span>|<span data-ttu-id="4e6a8-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4e6a8-141">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="4e6a8-142">Die Liste der Dateien für diese App-Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-142">The list of files for this app content version.</span></span>|
|<span data-ttu-id="4e6a8-143">containedApps</span><span class="sxs-lookup"><span data-stu-id="4e6a8-143">containedApps</span></span>|<span data-ttu-id="4e6a8-144">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4e6a8-144">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="4e6a8-145">Die Auflistung der enthaltenen apps in einer MobileLobApp fungiert als Paket.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-145">The collection of contained apps in a MobileLobApp acting as a package.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e6a8-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4e6a8-146">JSON Representation</span></span>
<span data-ttu-id="4e6a8-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e6a8-147">Here is a JSON representation of the resource.</span></span>
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





