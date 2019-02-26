---
title: managedDeviceMobileAppConfigurationDeviceSummary-Ressourcentyp
description: Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für eine Zusammenfassung des Gerätestatus von MDM-Konfigurationen mobiler Apps.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e62d02b5b702b56d72a0c75f9e5da1f6ad9dbdc3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259640"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a><span data-ttu-id="43b83-103">managedDeviceMobileAppConfigurationDeviceSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="43b83-103">managedDeviceMobileAppConfigurationDeviceSummary resource type</span></span>

> <span data-ttu-id="43b83-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="43b83-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43b83-105">Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für eine Zusammenfassung des Gerätestatus von MDM-Konfigurationen mobiler Apps.</span><span class="sxs-lookup"><span data-stu-id="43b83-105">Contains properties, inherited properties and actions for an MDM mobile app configuration device status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="43b83-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="43b83-106">Methods</span></span>
|<span data-ttu-id="43b83-107">Methode</span><span class="sxs-lookup"><span data-stu-id="43b83-107">Method</span></span>|<span data-ttu-id="43b83-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="43b83-108">Return Type</span></span>|<span data-ttu-id="43b83-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43b83-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="43b83-110">managedDeviceMobileAppConfigurationDeviceSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="43b83-110">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[<span data-ttu-id="43b83-111">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="43b83-111">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="43b83-112">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="43b83-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|
|[<span data-ttu-id="43b83-113">managedDeviceMobileAppConfigurationDeviceSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="43b83-113">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[<span data-ttu-id="43b83-114">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="43b83-114">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="43b83-115">Aktualisieren der Eigenschaften eines [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="43b83-115">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43b83-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="43b83-116">Properties</span></span>
|<span data-ttu-id="43b83-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43b83-117">Property</span></span>|<span data-ttu-id="43b83-118">Typ</span><span class="sxs-lookup"><span data-stu-id="43b83-118">Type</span></span>|<span data-ttu-id="43b83-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43b83-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43b83-120">id</span><span class="sxs-lookup"><span data-stu-id="43b83-120">id</span></span>|<span data-ttu-id="43b83-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="43b83-121">String</span></span>|<span data-ttu-id="43b83-122">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="43b83-122">Key of the entity.</span></span>|
|<span data-ttu-id="43b83-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="43b83-123">pendingCount</span></span>|<span data-ttu-id="43b83-124">Int32</span><span class="sxs-lookup"><span data-stu-id="43b83-124">Int32</span></span>|<span data-ttu-id="43b83-125">Anzahl der ausstehenden Geräte</span><span class="sxs-lookup"><span data-stu-id="43b83-125">Number of pending devices</span></span>|
|<span data-ttu-id="43b83-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="43b83-126">notApplicableCount</span></span>|<span data-ttu-id="43b83-127">Int32</span><span class="sxs-lookup"><span data-stu-id="43b83-127">Int32</span></span>|<span data-ttu-id="43b83-128">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="43b83-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="43b83-129">successCount</span><span class="sxs-lookup"><span data-stu-id="43b83-129">successCount</span></span>|<span data-ttu-id="43b83-130">Int32</span><span class="sxs-lookup"><span data-stu-id="43b83-130">Int32</span></span>|<span data-ttu-id="43b83-131">Anzahl der erfolgreichen Geräte</span><span class="sxs-lookup"><span data-stu-id="43b83-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="43b83-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="43b83-132">errorCount</span></span>|<span data-ttu-id="43b83-133">Int32</span><span class="sxs-lookup"><span data-stu-id="43b83-133">Int32</span></span>|<span data-ttu-id="43b83-134">Anzahl der fehlerhaften Geräte</span><span class="sxs-lookup"><span data-stu-id="43b83-134">Number of error devices</span></span>|
|<span data-ttu-id="43b83-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="43b83-135">failedCount</span></span>|<span data-ttu-id="43b83-136">Int32</span><span class="sxs-lookup"><span data-stu-id="43b83-136">Int32</span></span>|<span data-ttu-id="43b83-137">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="43b83-137">Number of failed devices</span></span>|
|<span data-ttu-id="43b83-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="43b83-138">lastUpdateDateTime</span></span>|<span data-ttu-id="43b83-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43b83-139">DateTimeOffset</span></span>|<span data-ttu-id="43b83-140">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="43b83-140">Last update time</span></span>|
|<span data-ttu-id="43b83-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="43b83-141">configurationVersion</span></span>|<span data-ttu-id="43b83-142">Int32</span><span class="sxs-lookup"><span data-stu-id="43b83-142">Int32</span></span>|<span data-ttu-id="43b83-143">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="43b83-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="43b83-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="43b83-144">Relationships</span></span>
<span data-ttu-id="43b83-145">Keine</span><span class="sxs-lookup"><span data-stu-id="43b83-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43b83-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="43b83-146">JSON Representation</span></span>
<span data-ttu-id="43b83-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="43b83-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
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



