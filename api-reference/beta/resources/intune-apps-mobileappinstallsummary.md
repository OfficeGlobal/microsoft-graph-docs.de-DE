---
title: mobileAppInstallSummary-Ressourcentyp
description: Enthält Eigenschaften für die Installationszusammenfassung einer mobilen App.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9747d53c56f9e505b61e1fa38bf5abdc27d14e42
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150764"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="5ab59-103">mobileAppInstallSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5ab59-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="5ab59-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5ab59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ab59-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5ab59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ab59-106">Enthält Eigenschaften für die Installationszusammenfassung einer mobilen App.</span><span class="sxs-lookup"><span data-stu-id="5ab59-106">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="5ab59-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="5ab59-107">Methods</span></span>
|<span data-ttu-id="5ab59-108">Methode</span><span class="sxs-lookup"><span data-stu-id="5ab59-108">Method</span></span>|<span data-ttu-id="5ab59-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5ab59-109">Return Type</span></span>|<span data-ttu-id="5ab59-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ab59-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5ab59-111">MobileAppInstallSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="5ab59-111">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="5ab59-112">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5ab59-112">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="5ab59-113">Lesen von Eigenschaften und Beziehungen des [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5ab59-113">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="5ab59-114">MobileAppInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5ab59-114">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="5ab59-115">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5ab59-115">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="5ab59-116">Aktualisieren der Eigenschaften eines [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5ab59-116">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5ab59-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5ab59-117">Properties</span></span>
|<span data-ttu-id="5ab59-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5ab59-118">Property</span></span>|<span data-ttu-id="5ab59-119">Typ</span><span class="sxs-lookup"><span data-stu-id="5ab59-119">Type</span></span>|<span data-ttu-id="5ab59-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ab59-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ab59-121">id</span><span class="sxs-lookup"><span data-stu-id="5ab59-121">id</span></span>|<span data-ttu-id="5ab59-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5ab59-122">String</span></span>|<span data-ttu-id="5ab59-123">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5ab59-123">Key of the entity.</span></span>|
|<span data-ttu-id="5ab59-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ab59-124">installedDeviceCount</span></span>|<span data-ttu-id="5ab59-125">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab59-125">Int32</span></span>|<span data-ttu-id="5ab59-126">Die Anzahl der Geräte, die diese APP erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="5ab59-126">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="5ab59-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ab59-127">failedDeviceCount</span></span>|<span data-ttu-id="5ab59-128">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab59-128">Int32</span></span>|<span data-ttu-id="5ab59-129">Anzahl der Geräte, die diese APP nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="5ab59-129">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="5ab59-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ab59-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="5ab59-131">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab59-131">Int32</span></span>|<span data-ttu-id="5ab59-132">Die Anzahl der Geräte, die für diese APP nicht anwendbar sind.</span><span class="sxs-lookup"><span data-stu-id="5ab59-132">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="5ab59-133">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ab59-133">notInstalledDeviceCount</span></span>|<span data-ttu-id="5ab59-134">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab59-134">Int32</span></span>|<span data-ttu-id="5ab59-135">Anzahl der Geräte, auf denen diese APP nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="5ab59-135">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="5ab59-136">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ab59-136">pendingInstallDeviceCount</span></span>|<span data-ttu-id="5ab59-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab59-137">Int32</span></span>|<span data-ttu-id="5ab59-138">Anzahl der Geräte, die zur Installation dieser APP benachrichtigt wurden.</span><span class="sxs-lookup"><span data-stu-id="5ab59-138">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="5ab59-139">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="5ab59-139">installedUserCount</span></span>|<span data-ttu-id="5ab59-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab59-140">Int32</span></span>|<span data-ttu-id="5ab59-141">Die Anzahl der Benutzer, deren Geräte alle für die Installation dieser APP erfolgreich waren.</span><span class="sxs-lookup"><span data-stu-id="5ab59-141">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="5ab59-142">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="5ab59-142">failedUserCount</span></span>|<span data-ttu-id="5ab59-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab59-143">Int32</span></span>|<span data-ttu-id="5ab59-144">Die Anzahl der Benutzer, die über ein Gerät verfügen, für das diese APP nicht installiert werden konnte.</span><span class="sxs-lookup"><span data-stu-id="5ab59-144">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="5ab59-145">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="5ab59-145">notApplicableUserCount</span></span>|<span data-ttu-id="5ab59-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab59-146">Int32</span></span>|<span data-ttu-id="5ab59-147">Die Anzahl der Benutzer, deren Geräte für diese APP nicht anwendbar waren.</span><span class="sxs-lookup"><span data-stu-id="5ab59-147">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="5ab59-148">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="5ab59-148">notInstalledUserCount</span></span>|<span data-ttu-id="5ab59-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab59-149">Int32</span></span>|<span data-ttu-id="5ab59-150">Die Anzahl von Benutzern, die über 1 oder mehr Geräte verfügen, die diese APP nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="5ab59-150">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="5ab59-151">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="5ab59-151">pendingInstallUserCount</span></span>|<span data-ttu-id="5ab59-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5ab59-152">Int32</span></span>|<span data-ttu-id="5ab59-153">Die Anzahl der Benutzer mit mindestens 1 Gerät, die zur Installation dieser APP benachrichtigt wurden und über 0 Geräte mit Fehlern verfügen.</span><span class="sxs-lookup"><span data-stu-id="5ab59-153">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ab59-154">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5ab59-154">Relationships</span></span>
<span data-ttu-id="5ab59-155">Keine</span><span class="sxs-lookup"><span data-stu-id="5ab59-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ab59-156">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5ab59-156">JSON Representation</span></span>
<span data-ttu-id="5ab59-157">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5ab59-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```




