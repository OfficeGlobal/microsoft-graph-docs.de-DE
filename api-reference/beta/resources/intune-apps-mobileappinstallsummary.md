---
title: Ressourcentyp mobileAppInstallSummary
description: Enthält Eigenschaften für die Zusammenfassung der Installation einer mobilen App.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a75dba8303d254aff911cc66931d52abb8b76c07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916026"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="ff3ec-103">Ressourcentyp mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ff3ec-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="ff3ec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff3ec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff3ec-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff3ec-107">Enthält Eigenschaften für die Zusammenfassung der Installation einer mobilen App.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-107">Contains properties for the installation summary of a mobile app.</span></span>
## <a name="methods"></a><span data-ttu-id="ff3ec-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="ff3ec-108">Methods</span></span>
|<span data-ttu-id="ff3ec-109">Methode</span><span class="sxs-lookup"><span data-stu-id="ff3ec-109">Method</span></span>|<span data-ttu-id="ff3ec-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ff3ec-110">Return Type</span></span>|<span data-ttu-id="ff3ec-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff3ec-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff3ec-112">Abrufen von mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ff3ec-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="ff3ec-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ff3ec-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="ff3ec-114">Lesen Sie Eigenschaften und Beziehungen des [MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="ff3ec-115">MobileAppInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ff3ec-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="ff3ec-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ff3ec-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="ff3ec-117">Aktualisieren Sie die Eigenschaften eines [MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff3ec-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ff3ec-118">Properties</span></span>
|<span data-ttu-id="ff3ec-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff3ec-119">Property</span></span>|<span data-ttu-id="ff3ec-120">Typ</span><span class="sxs-lookup"><span data-stu-id="ff3ec-120">Type</span></span>|<span data-ttu-id="ff3ec-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff3ec-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff3ec-122">id</span><span class="sxs-lookup"><span data-stu-id="ff3ec-122">id</span></span>|<span data-ttu-id="ff3ec-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff3ec-123">String</span></span>|<span data-ttu-id="ff3ec-124">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ff3ec-124">Key of the entity.</span></span>|
|<span data-ttu-id="ff3ec-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff3ec-125">installedDeviceCount</span></span>|<span data-ttu-id="ff3ec-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ff3ec-126">Int32</span></span>|<span data-ttu-id="ff3ec-127">Anzahl der Geräte, die diese app erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="ff3ec-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff3ec-128">failedDeviceCount</span></span>|<span data-ttu-id="ff3ec-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ff3ec-129">Int32</span></span>|<span data-ttu-id="ff3ec-130">Anzahl der Geräte, die fehlgeschlagen sind, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="ff3ec-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff3ec-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="ff3ec-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ff3ec-132">Int32</span></span>|<span data-ttu-id="ff3ec-133">Anzahl der Geräte, die für diese app nicht zutreffen.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="ff3ec-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff3ec-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="ff3ec-135">Int32</span><span class="sxs-lookup"><span data-stu-id="ff3ec-135">Int32</span></span>|<span data-ttu-id="ff3ec-136">Anzahl der Geräte, die diese app installiert nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="ff3ec-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ff3ec-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="ff3ec-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ff3ec-138">Int32</span></span>|<span data-ttu-id="ff3ec-139">Anzahl der Geräte, die diese app installieren benachrichtigt wurden.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="ff3ec-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ff3ec-140">installedUserCount</span></span>|<span data-ttu-id="ff3ec-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ff3ec-141">Int32</span></span>|<span data-ttu-id="ff3ec-142">Anzahl der Benutzer, deren Geräte alle erfolgreich ausgeführt wurden, um diese app zu installieren.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="ff3ec-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ff3ec-143">failedUserCount</span></span>|<span data-ttu-id="ff3ec-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ff3ec-144">Int32</span></span>|<span data-ttu-id="ff3ec-145">Anzahl der Benutzer, die 1 haben oder weitere Gerät, deren Installation diese app fehlschlug.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="ff3ec-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="ff3ec-146">notApplicableUserCount</span></span>|<span data-ttu-id="ff3ec-147">Int32</span><span class="sxs-lookup"><span data-stu-id="ff3ec-147">Int32</span></span>|<span data-ttu-id="ff3ec-148">Anzahl der Benutzer, deren Geräte alle nicht zutreffend für diese app waren.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="ff3ec-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ff3ec-149">notInstalledUserCount</span></span>|<span data-ttu-id="ff3ec-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ff3ec-150">Int32</span></span>|<span data-ttu-id="ff3ec-151">Anzahl der Benutzer mit 1 oder mehrere Geräte, die diese app nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="ff3ec-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="ff3ec-152">pendingInstallUserCount</span></span>|<span data-ttu-id="ff3ec-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ff3ec-153">Int32</span></span>|<span data-ttu-id="ff3ec-154">Anzahl der Benutzer, die 1 haben oder weitere Geräte, die diese app installieren und 0 Geräte mit Fehlern benachrichtigt wurden.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff3ec-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ff3ec-155">Relationships</span></span>
<span data-ttu-id="ff3ec-156">Keine</span><span class="sxs-lookup"><span data-stu-id="ff3ec-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff3ec-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ff3ec-157">JSON Representation</span></span>
<span data-ttu-id="ff3ec-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ff3ec-158">Here is a JSON representation of the resource.</span></span>
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





