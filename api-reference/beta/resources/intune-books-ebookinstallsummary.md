---
title: eBookInstallSummary-Ressourcentyp
description: Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 41e9752707cfdca974162b097ad4e6fc96b3b43a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815890"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="aedc8-103">eBookInstallSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aedc8-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="aedc8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aedc8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aedc8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aedc8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aedc8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aedc8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aedc8-107">Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.</span><span class="sxs-lookup"><span data-stu-id="aedc8-107">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="aedc8-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="aedc8-108">Methods</span></span>
|<span data-ttu-id="aedc8-109">Methode</span><span class="sxs-lookup"><span data-stu-id="aedc8-109">Method</span></span>|<span data-ttu-id="aedc8-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="aedc8-110">Return Type</span></span>|<span data-ttu-id="aedc8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aedc8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aedc8-112">eBookInstallSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="aedc8-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="aedc8-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="aedc8-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="aedc8-114">Lesen der Eigenschaften und Beziehungen von [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekten.</span><span class="sxs-lookup"><span data-stu-id="aedc8-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="aedc8-115">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="aedc8-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="aedc8-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="aedc8-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="aedc8-117">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aedc8-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aedc8-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aedc8-118">Properties</span></span>
|<span data-ttu-id="aedc8-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aedc8-119">Property</span></span>|<span data-ttu-id="aedc8-120">Typ</span><span class="sxs-lookup"><span data-stu-id="aedc8-120">Type</span></span>|<span data-ttu-id="aedc8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aedc8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aedc8-122">id</span><span class="sxs-lookup"><span data-stu-id="aedc8-122">id</span></span>|<span data-ttu-id="aedc8-123">String</span><span class="sxs-lookup"><span data-stu-id="aedc8-123">String</span></span>|<span data-ttu-id="aedc8-124">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="aedc8-124">Key of the entity.</span></span>|
|<span data-ttu-id="aedc8-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aedc8-125">installedDeviceCount</span></span>|<span data-ttu-id="aedc8-126">Int32</span><span class="sxs-lookup"><span data-stu-id="aedc8-126">Int32</span></span>|<span data-ttu-id="aedc8-127">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="aedc8-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="aedc8-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aedc8-128">failedDeviceCount</span></span>|<span data-ttu-id="aedc8-129">Int32</span><span class="sxs-lookup"><span data-stu-id="aedc8-129">Int32</span></span>|<span data-ttu-id="aedc8-130">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="aedc8-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="aedc8-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aedc8-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="aedc8-132">Int32</span><span class="sxs-lookup"><span data-stu-id="aedc8-132">Int32</span></span>|<span data-ttu-id="aedc8-133">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="aedc8-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="aedc8-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="aedc8-134">installedUserCount</span></span>|<span data-ttu-id="aedc8-135">Int32</span><span class="sxs-lookup"><span data-stu-id="aedc8-135">Int32</span></span>|<span data-ttu-id="aedc8-136">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="aedc8-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="aedc8-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="aedc8-137">failedUserCount</span></span>|<span data-ttu-id="aedc8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="aedc8-138">Int32</span></span>|<span data-ttu-id="aedc8-139">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="aedc8-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="aedc8-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="aedc8-140">notInstalledUserCount</span></span>|<span data-ttu-id="aedc8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="aedc8-141">Int32</span></span>|<span data-ttu-id="aedc8-142">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="aedc8-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aedc8-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aedc8-143">Relationships</span></span>
<span data-ttu-id="aedc8-144">Keine</span><span class="sxs-lookup"><span data-stu-id="aedc8-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aedc8-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aedc8-145">JSON Representation</span></span>
<span data-ttu-id="aedc8-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aedc8-146">Here is a JSON representation of the resource.</span></span>
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





