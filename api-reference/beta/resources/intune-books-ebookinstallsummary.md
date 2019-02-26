---
title: eBookInstallSummary-Ressourcentyp
description: Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52d08d00bfbc26e0b72ddf53404eff8d55bb72b9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151240"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="003f9-103">eBookInstallSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="003f9-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="003f9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="003f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="003f9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="003f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="003f9-106">Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.</span><span class="sxs-lookup"><span data-stu-id="003f9-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="003f9-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="003f9-107">Methods</span></span>
|<span data-ttu-id="003f9-108">Methode</span><span class="sxs-lookup"><span data-stu-id="003f9-108">Method</span></span>|<span data-ttu-id="003f9-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="003f9-109">Return Type</span></span>|<span data-ttu-id="003f9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="003f9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="003f9-111">eBookInstallSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="003f9-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="003f9-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="003f9-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="003f9-113">Lesen der Eigenschaften und Beziehungen von [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekten.</span><span class="sxs-lookup"><span data-stu-id="003f9-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="003f9-114">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="003f9-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="003f9-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="003f9-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="003f9-116">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="003f9-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="003f9-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="003f9-117">Properties</span></span>
|<span data-ttu-id="003f9-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="003f9-118">Property</span></span>|<span data-ttu-id="003f9-119">Typ</span><span class="sxs-lookup"><span data-stu-id="003f9-119">Type</span></span>|<span data-ttu-id="003f9-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="003f9-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="003f9-121">id</span><span class="sxs-lookup"><span data-stu-id="003f9-121">id</span></span>|<span data-ttu-id="003f9-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="003f9-122">String</span></span>|<span data-ttu-id="003f9-123">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="003f9-123">Key of the entity.</span></span>|
|<span data-ttu-id="003f9-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="003f9-124">installedDeviceCount</span></span>|<span data-ttu-id="003f9-125">Int32</span><span class="sxs-lookup"><span data-stu-id="003f9-125">Int32</span></span>|<span data-ttu-id="003f9-126">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="003f9-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="003f9-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="003f9-127">failedDeviceCount</span></span>|<span data-ttu-id="003f9-128">Int32</span><span class="sxs-lookup"><span data-stu-id="003f9-128">Int32</span></span>|<span data-ttu-id="003f9-129">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="003f9-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="003f9-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="003f9-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="003f9-131">Int32</span><span class="sxs-lookup"><span data-stu-id="003f9-131">Int32</span></span>|<span data-ttu-id="003f9-132">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="003f9-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="003f9-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="003f9-133">installedUserCount</span></span>|<span data-ttu-id="003f9-134">Int32</span><span class="sxs-lookup"><span data-stu-id="003f9-134">Int32</span></span>|<span data-ttu-id="003f9-135">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="003f9-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="003f9-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="003f9-136">failedUserCount</span></span>|<span data-ttu-id="003f9-137">Int32</span><span class="sxs-lookup"><span data-stu-id="003f9-137">Int32</span></span>|<span data-ttu-id="003f9-138">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="003f9-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="003f9-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="003f9-139">notInstalledUserCount</span></span>|<span data-ttu-id="003f9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="003f9-140">Int32</span></span>|<span data-ttu-id="003f9-141">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="003f9-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="003f9-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="003f9-142">Relationships</span></span>
<span data-ttu-id="003f9-143">Keine</span><span class="sxs-lookup"><span data-stu-id="003f9-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="003f9-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="003f9-144">JSON Representation</span></span>
<span data-ttu-id="003f9-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="003f9-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```




