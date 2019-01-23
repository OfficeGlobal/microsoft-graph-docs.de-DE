---
title: eBookInstallSummary-Ressourcentyp
description: Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4e8952012624a038f497fea3c6b81ad364448a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415341"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="07317-103">eBookInstallSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="07317-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="07317-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="07317-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07317-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07317-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07317-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07317-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07317-107">Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.</span><span class="sxs-lookup"><span data-stu-id="07317-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="07317-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="07317-108">Methods</span></span>
|<span data-ttu-id="07317-109">Methode</span><span class="sxs-lookup"><span data-stu-id="07317-109">Method</span></span>|<span data-ttu-id="07317-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="07317-110">Return Type</span></span>|<span data-ttu-id="07317-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07317-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="07317-112">eBookInstallSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="07317-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="07317-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="07317-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="07317-114">Lesen der Eigenschaften und Beziehungen von [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekten.</span><span class="sxs-lookup"><span data-stu-id="07317-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="07317-115">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="07317-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="07317-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="07317-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="07317-117">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="07317-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="07317-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07317-118">Properties</span></span>
|<span data-ttu-id="07317-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07317-119">Property</span></span>|<span data-ttu-id="07317-120">Typ</span><span class="sxs-lookup"><span data-stu-id="07317-120">Type</span></span>|<span data-ttu-id="07317-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07317-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07317-122">id</span><span class="sxs-lookup"><span data-stu-id="07317-122">id</span></span>|<span data-ttu-id="07317-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07317-123">String</span></span>|<span data-ttu-id="07317-124">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="07317-124">Key of the entity.</span></span>|
|<span data-ttu-id="07317-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07317-125">installedDeviceCount</span></span>|<span data-ttu-id="07317-126">Int32</span><span class="sxs-lookup"><span data-stu-id="07317-126">Int32</span></span>|<span data-ttu-id="07317-127">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="07317-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="07317-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07317-128">failedDeviceCount</span></span>|<span data-ttu-id="07317-129">Int32</span><span class="sxs-lookup"><span data-stu-id="07317-129">Int32</span></span>|<span data-ttu-id="07317-130">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="07317-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="07317-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07317-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="07317-132">Int32</span><span class="sxs-lookup"><span data-stu-id="07317-132">Int32</span></span>|<span data-ttu-id="07317-133">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="07317-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="07317-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="07317-134">installedUserCount</span></span>|<span data-ttu-id="07317-135">Int32</span><span class="sxs-lookup"><span data-stu-id="07317-135">Int32</span></span>|<span data-ttu-id="07317-136">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="07317-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="07317-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="07317-137">failedUserCount</span></span>|<span data-ttu-id="07317-138">Int32</span><span class="sxs-lookup"><span data-stu-id="07317-138">Int32</span></span>|<span data-ttu-id="07317-139">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="07317-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="07317-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="07317-140">notInstalledUserCount</span></span>|<span data-ttu-id="07317-141">Int32</span><span class="sxs-lookup"><span data-stu-id="07317-141">Int32</span></span>|<span data-ttu-id="07317-142">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="07317-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07317-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="07317-143">Relationships</span></span>
<span data-ttu-id="07317-144">Keine</span><span class="sxs-lookup"><span data-stu-id="07317-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07317-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07317-145">JSON Representation</span></span>
<span data-ttu-id="07317-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="07317-146">Here is a JSON representation of the resource.</span></span>
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




