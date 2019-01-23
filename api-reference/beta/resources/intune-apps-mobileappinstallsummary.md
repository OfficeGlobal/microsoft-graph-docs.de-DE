---
title: Ressourcentyp mobileAppInstallSummary
description: Enthält Eigenschaften für die Zusammenfassung der Installation einer mobilen App.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2bd7c30c1b00e83731766bcd80f9a9fafd8e8b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416713"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="0888f-103">Ressourcentyp mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0888f-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="0888f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0888f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0888f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0888f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0888f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0888f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0888f-107">Enthält Eigenschaften für die Zusammenfassung der Installation einer mobilen App.</span><span class="sxs-lookup"><span data-stu-id="0888f-107">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="0888f-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="0888f-108">Methods</span></span>
|<span data-ttu-id="0888f-109">Methode</span><span class="sxs-lookup"><span data-stu-id="0888f-109">Method</span></span>|<span data-ttu-id="0888f-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0888f-110">Return Type</span></span>|<span data-ttu-id="0888f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0888f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0888f-112">Abrufen von mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0888f-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="0888f-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0888f-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="0888f-114">Lesen Sie Eigenschaften und Beziehungen des [MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0888f-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="0888f-115">MobileAppInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0888f-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="0888f-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0888f-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="0888f-117">Aktualisieren Sie die Eigenschaften eines [MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0888f-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0888f-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0888f-118">Properties</span></span>
|<span data-ttu-id="0888f-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0888f-119">Property</span></span>|<span data-ttu-id="0888f-120">Typ</span><span class="sxs-lookup"><span data-stu-id="0888f-120">Type</span></span>|<span data-ttu-id="0888f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0888f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0888f-122">id</span><span class="sxs-lookup"><span data-stu-id="0888f-122">id</span></span>|<span data-ttu-id="0888f-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0888f-123">String</span></span>|<span data-ttu-id="0888f-124">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0888f-124">Key of the entity.</span></span>|
|<span data-ttu-id="0888f-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0888f-125">installedDeviceCount</span></span>|<span data-ttu-id="0888f-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0888f-126">Int32</span></span>|<span data-ttu-id="0888f-127">Anzahl der Geräte, die diese app erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="0888f-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="0888f-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0888f-128">failedDeviceCount</span></span>|<span data-ttu-id="0888f-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0888f-129">Int32</span></span>|<span data-ttu-id="0888f-130">Anzahl der Geräte, die fehlgeschlagen sind, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="0888f-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="0888f-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0888f-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="0888f-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0888f-132">Int32</span></span>|<span data-ttu-id="0888f-133">Anzahl der Geräte, die für diese app nicht zutreffen.</span><span class="sxs-lookup"><span data-stu-id="0888f-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="0888f-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0888f-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="0888f-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0888f-135">Int32</span></span>|<span data-ttu-id="0888f-136">Anzahl der Geräte, die diese app installiert nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="0888f-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="0888f-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0888f-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="0888f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0888f-138">Int32</span></span>|<span data-ttu-id="0888f-139">Anzahl der Geräte, die diese app installieren benachrichtigt wurden.</span><span class="sxs-lookup"><span data-stu-id="0888f-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="0888f-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="0888f-140">installedUserCount</span></span>|<span data-ttu-id="0888f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="0888f-141">Int32</span></span>|<span data-ttu-id="0888f-142">Anzahl der Benutzer, deren Geräte alle erfolgreich ausgeführt wurden, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="0888f-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="0888f-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="0888f-143">failedUserCount</span></span>|<span data-ttu-id="0888f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="0888f-144">Int32</span></span>|<span data-ttu-id="0888f-145">Anzahl der Benutzer, die 1 haben oder weitere Gerät, deren Installation diese app fehlschlug.</span><span class="sxs-lookup"><span data-stu-id="0888f-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="0888f-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="0888f-146">notApplicableUserCount</span></span>|<span data-ttu-id="0888f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0888f-147">Int32</span></span>|<span data-ttu-id="0888f-148">Anzahl der Benutzer, deren Geräte alle nicht zutreffend für diese app waren.</span><span class="sxs-lookup"><span data-stu-id="0888f-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="0888f-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="0888f-149">notInstalledUserCount</span></span>|<span data-ttu-id="0888f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0888f-150">Int32</span></span>|<span data-ttu-id="0888f-151">Anzahl der Benutzer mit 1 oder mehrere Geräte, die diese app nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="0888f-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="0888f-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="0888f-152">pendingInstallUserCount</span></span>|<span data-ttu-id="0888f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0888f-153">Int32</span></span>|<span data-ttu-id="0888f-154">Anzahl der Benutzer, die 1 haben oder weitere Geräte, die diese app installieren und 0 Geräte mit Fehlern benachrichtigt wurden.</span><span class="sxs-lookup"><span data-stu-id="0888f-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0888f-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0888f-155">Relationships</span></span>
<span data-ttu-id="0888f-156">Keine</span><span class="sxs-lookup"><span data-stu-id="0888f-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0888f-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0888f-157">JSON Representation</span></span>
<span data-ttu-id="0888f-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0888f-158">Here is a JSON representation of the resource.</span></span>
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




