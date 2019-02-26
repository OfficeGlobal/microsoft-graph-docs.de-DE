---
title: eBookInstallSummary-Ressourcentyp
description: Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17075183e0541669923a69c140d228cb1cbd4a2e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251538"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="08750-103">eBookInstallSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="08750-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="08750-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="08750-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08750-105">Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.</span><span class="sxs-lookup"><span data-stu-id="08750-105">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="08750-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="08750-106">Methods</span></span>
|<span data-ttu-id="08750-107">Methode</span><span class="sxs-lookup"><span data-stu-id="08750-107">Method</span></span>|<span data-ttu-id="08750-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="08750-108">Return Type</span></span>|<span data-ttu-id="08750-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08750-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="08750-110">eBookInstallSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="08750-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="08750-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="08750-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="08750-112">Lesen der Eigenschaften und Beziehungen von [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekten.</span><span class="sxs-lookup"><span data-stu-id="08750-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="08750-113">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="08750-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="08750-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="08750-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="08750-115">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="08750-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="08750-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08750-116">Properties</span></span>
|<span data-ttu-id="08750-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08750-117">Property</span></span>|<span data-ttu-id="08750-118">Typ</span><span class="sxs-lookup"><span data-stu-id="08750-118">Type</span></span>|<span data-ttu-id="08750-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08750-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08750-120">id</span><span class="sxs-lookup"><span data-stu-id="08750-120">id</span></span>|<span data-ttu-id="08750-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08750-121">String</span></span>|<span data-ttu-id="08750-122">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="08750-122">Key of the entity.</span></span>|
|<span data-ttu-id="08750-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="08750-123">installedDeviceCount</span></span>|<span data-ttu-id="08750-124">Int32</span><span class="sxs-lookup"><span data-stu-id="08750-124">Int32</span></span>|<span data-ttu-id="08750-125">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="08750-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="08750-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="08750-126">failedDeviceCount</span></span>|<span data-ttu-id="08750-127">Int32</span><span class="sxs-lookup"><span data-stu-id="08750-127">Int32</span></span>|<span data-ttu-id="08750-128">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="08750-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="08750-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="08750-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="08750-130">Int32</span><span class="sxs-lookup"><span data-stu-id="08750-130">Int32</span></span>|<span data-ttu-id="08750-131">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="08750-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="08750-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="08750-132">installedUserCount</span></span>|<span data-ttu-id="08750-133">Int32</span><span class="sxs-lookup"><span data-stu-id="08750-133">Int32</span></span>|<span data-ttu-id="08750-134">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="08750-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="08750-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="08750-135">failedUserCount</span></span>|<span data-ttu-id="08750-136">Int32</span><span class="sxs-lookup"><span data-stu-id="08750-136">Int32</span></span>|<span data-ttu-id="08750-137">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="08750-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="08750-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="08750-138">notInstalledUserCount</span></span>|<span data-ttu-id="08750-139">Int32</span><span class="sxs-lookup"><span data-stu-id="08750-139">Int32</span></span>|<span data-ttu-id="08750-140">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="08750-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08750-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="08750-141">Relationships</span></span>
<span data-ttu-id="08750-142">Keine</span><span class="sxs-lookup"><span data-stu-id="08750-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08750-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08750-143">JSON Representation</span></span>
<span data-ttu-id="08750-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08750-144">Here is a JSON representation of the resource.</span></span>
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



