---
title: eBookInstallSummary-Ressourcentyp
description: Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.
ms.openlocfilehash: 59754a8b925f573e44abd9ae1f674ab3f08f51c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019463"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="e3e44-103">eBookInstallSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e3e44-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="e3e44-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e3e44-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3e44-105">Enthält Eigenschaften für die Installationszusammenfassung eines Buchs für ein Gerät.</span><span class="sxs-lookup"><span data-stu-id="e3e44-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="e3e44-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="e3e44-106">Methods</span></span>
|<span data-ttu-id="e3e44-107">Methode</span><span class="sxs-lookup"><span data-stu-id="e3e44-107">Method</span></span>|<span data-ttu-id="e3e44-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e3e44-108">Return Type</span></span>|<span data-ttu-id="e3e44-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3e44-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e3e44-110">eBookInstallSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="e3e44-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="e3e44-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e3e44-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="e3e44-112">Lesen der Eigenschaften und Beziehungen von [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekten.</span><span class="sxs-lookup"><span data-stu-id="e3e44-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="e3e44-113">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e3e44-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="e3e44-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e3e44-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="e3e44-115">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3e44-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3e44-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3e44-116">Properties</span></span>
|<span data-ttu-id="e3e44-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3e44-117">Property</span></span>|<span data-ttu-id="e3e44-118">Typ</span><span class="sxs-lookup"><span data-stu-id="e3e44-118">Type</span></span>|<span data-ttu-id="e3e44-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3e44-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e44-120">id</span><span class="sxs-lookup"><span data-stu-id="e3e44-120">id</span></span>|<span data-ttu-id="e3e44-121">String</span><span class="sxs-lookup"><span data-stu-id="e3e44-121">String</span></span>|<span data-ttu-id="e3e44-122">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e3e44-122">Key of the entity.</span></span>|
|<span data-ttu-id="e3e44-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3e44-123">installedDeviceCount</span></span>|<span data-ttu-id="e3e44-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e44-124">Int32</span></span>|<span data-ttu-id="e3e44-125">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="e3e44-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="e3e44-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3e44-126">failedDeviceCount</span></span>|<span data-ttu-id="e3e44-127">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e44-127">Int32</span></span>|<span data-ttu-id="e3e44-128">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="e3e44-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="e3e44-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3e44-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="e3e44-130">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e44-130">Int32</span></span>|<span data-ttu-id="e3e44-131">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="e3e44-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="e3e44-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="e3e44-132">installedUserCount</span></span>|<span data-ttu-id="e3e44-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e44-133">Int32</span></span>|<span data-ttu-id="e3e44-134">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="e3e44-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="e3e44-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="e3e44-135">failedUserCount</span></span>|<span data-ttu-id="e3e44-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e44-136">Int32</span></span>|<span data-ttu-id="e3e44-137">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="e3e44-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="e3e44-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="e3e44-138">notInstalledUserCount</span></span>|<span data-ttu-id="e3e44-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e44-139">Int32</span></span>|<span data-ttu-id="e3e44-140">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="e3e44-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3e44-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e3e44-141">Relationships</span></span>
<span data-ttu-id="e3e44-142">Keine</span><span class="sxs-lookup"><span data-stu-id="e3e44-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e3e44-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3e44-143">JSON Representation</span></span>
<span data-ttu-id="e3e44-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3e44-144">Here is a JSON representation of the resource.</span></span>
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



