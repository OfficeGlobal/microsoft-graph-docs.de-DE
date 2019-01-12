---
title: eBookInstallSummary-Ressourcentyp
description: Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d3a5d1ce5c05d0a8c20a79aea2fd3562ab2170c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915942"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="14d13-103">eBookInstallSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="14d13-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="14d13-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="14d13-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14d13-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="14d13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14d13-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="14d13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14d13-107">Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.</span><span class="sxs-lookup"><span data-stu-id="14d13-107">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="14d13-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="14d13-108">Methods</span></span>
|<span data-ttu-id="14d13-109">Methode</span><span class="sxs-lookup"><span data-stu-id="14d13-109">Method</span></span>|<span data-ttu-id="14d13-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="14d13-110">Return Type</span></span>|<span data-ttu-id="14d13-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14d13-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14d13-112">eBookInstallSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="14d13-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="14d13-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="14d13-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="14d13-114">Lesen der Eigenschaften und Beziehungen von [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekten.</span><span class="sxs-lookup"><span data-stu-id="14d13-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="14d13-115">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="14d13-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="14d13-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="14d13-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="14d13-117">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="14d13-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="14d13-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="14d13-118">Properties</span></span>
|<span data-ttu-id="14d13-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="14d13-119">Property</span></span>|<span data-ttu-id="14d13-120">Typ</span><span class="sxs-lookup"><span data-stu-id="14d13-120">Type</span></span>|<span data-ttu-id="14d13-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="14d13-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14d13-122">id</span><span class="sxs-lookup"><span data-stu-id="14d13-122">id</span></span>|<span data-ttu-id="14d13-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="14d13-123">String</span></span>|<span data-ttu-id="14d13-124">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="14d13-124">Key of the entity.</span></span>|
|<span data-ttu-id="14d13-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14d13-125">installedDeviceCount</span></span>|<span data-ttu-id="14d13-126">Int32</span><span class="sxs-lookup"><span data-stu-id="14d13-126">Int32</span></span>|<span data-ttu-id="14d13-127">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="14d13-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="14d13-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14d13-128">failedDeviceCount</span></span>|<span data-ttu-id="14d13-129">Int32</span><span class="sxs-lookup"><span data-stu-id="14d13-129">Int32</span></span>|<span data-ttu-id="14d13-130">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="14d13-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="14d13-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14d13-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="14d13-132">Int32</span><span class="sxs-lookup"><span data-stu-id="14d13-132">Int32</span></span>|<span data-ttu-id="14d13-133">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="14d13-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="14d13-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="14d13-134">installedUserCount</span></span>|<span data-ttu-id="14d13-135">Int32</span><span class="sxs-lookup"><span data-stu-id="14d13-135">Int32</span></span>|<span data-ttu-id="14d13-136">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="14d13-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="14d13-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="14d13-137">failedUserCount</span></span>|<span data-ttu-id="14d13-138">Int32</span><span class="sxs-lookup"><span data-stu-id="14d13-138">Int32</span></span>|<span data-ttu-id="14d13-139">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="14d13-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="14d13-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="14d13-140">notInstalledUserCount</span></span>|<span data-ttu-id="14d13-141">Int32</span><span class="sxs-lookup"><span data-stu-id="14d13-141">Int32</span></span>|<span data-ttu-id="14d13-142">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="14d13-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14d13-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="14d13-143">Relationships</span></span>
<span data-ttu-id="14d13-144">Keine</span><span class="sxs-lookup"><span data-stu-id="14d13-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="14d13-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="14d13-145">JSON Representation</span></span>
<span data-ttu-id="14d13-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="14d13-146">Here is a JSON representation of the resource.</span></span>
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





