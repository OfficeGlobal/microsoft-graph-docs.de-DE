---
title: deviceConfigurationUserOverview-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0103d6eda14e2411a3ece16a7dcff8eef50d9b9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883972"
---
# <a name="deviceconfigurationuseroverview-resource-type"></a><span data-ttu-id="85535-103">deviceConfigurationUserOverview-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="85535-103">deviceConfigurationUserOverview resource type</span></span>

> <span data-ttu-id="85535-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="85535-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85535-105">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="85535-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="85535-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="85535-106">Methods</span></span>
|<span data-ttu-id="85535-107">Methode</span><span class="sxs-lookup"><span data-stu-id="85535-107">Method</span></span>|<span data-ttu-id="85535-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="85535-108">Return Type</span></span>|<span data-ttu-id="85535-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85535-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="85535-110">deviceConfigurationUserOverview abrufen</span><span class="sxs-lookup"><span data-stu-id="85535-110">Get deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-get.md)|[<span data-ttu-id="85535-111">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="85535-111">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="85535-112">Lesen von Eigenschaften und Beziehungen des [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="85535-112">Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|
|[<span data-ttu-id="85535-113">deviceConfigurationUserOverview aktualisieren</span><span class="sxs-lookup"><span data-stu-id="85535-113">Update deviceConfigurationUserOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationuseroverview-update.md)|[<span data-ttu-id="85535-114">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="85535-114">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="85535-115">Aktualisieren der Eigenschaften eines [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="85535-115">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="85535-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="85535-116">Properties</span></span>
|<span data-ttu-id="85535-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85535-117">Property</span></span>|<span data-ttu-id="85535-118">Typ</span><span class="sxs-lookup"><span data-stu-id="85535-118">Type</span></span>|<span data-ttu-id="85535-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85535-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85535-120">id</span><span class="sxs-lookup"><span data-stu-id="85535-120">id</span></span>|<span data-ttu-id="85535-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85535-121">String</span></span>|<span data-ttu-id="85535-122">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="85535-122">Key of the entity.</span></span>|
|<span data-ttu-id="85535-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="85535-123">pendingCount</span></span>|<span data-ttu-id="85535-124">Int32</span><span class="sxs-lookup"><span data-stu-id="85535-124">Int32</span></span>|<span data-ttu-id="85535-125">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="85535-125">Number of pending Users</span></span>|
|<span data-ttu-id="85535-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="85535-126">notApplicableCount</span></span>|<span data-ttu-id="85535-127">Int32</span><span class="sxs-lookup"><span data-stu-id="85535-127">Int32</span></span>|<span data-ttu-id="85535-128">Anzahl der Benutzer nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="85535-128">Number of not applicable users</span></span>|
|<span data-ttu-id="85535-129">successCount</span><span class="sxs-lookup"><span data-stu-id="85535-129">successCount</span></span>|<span data-ttu-id="85535-130">Int32</span><span class="sxs-lookup"><span data-stu-id="85535-130">Int32</span></span>|<span data-ttu-id="85535-131">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="85535-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="85535-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="85535-132">errorCount</span></span>|<span data-ttu-id="85535-133">Int32</span><span class="sxs-lookup"><span data-stu-id="85535-133">Int32</span></span>|<span data-ttu-id="85535-134">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="85535-134">Number of error Users</span></span>|
|<span data-ttu-id="85535-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="85535-135">failedCount</span></span>|<span data-ttu-id="85535-136">Int32</span><span class="sxs-lookup"><span data-stu-id="85535-136">Int32</span></span>|<span data-ttu-id="85535-137">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="85535-137">Number of failed Users</span></span>|
|<span data-ttu-id="85535-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="85535-138">lastUpdateDateTime</span></span>|<span data-ttu-id="85535-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85535-139">DateTimeOffset</span></span>|<span data-ttu-id="85535-140">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="85535-140">Last update time</span></span>|
|<span data-ttu-id="85535-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="85535-141">configurationVersion</span></span>|<span data-ttu-id="85535-142">Int32</span><span class="sxs-lookup"><span data-stu-id="85535-142">Int32</span></span>|<span data-ttu-id="85535-143">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="85535-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="85535-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="85535-144">Relationships</span></span>
<span data-ttu-id="85535-145">Keine</span><span class="sxs-lookup"><span data-stu-id="85535-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="85535-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="85535-146">JSON Representation</span></span>
<span data-ttu-id="85535-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="85535-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



