---
title: deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp
description: Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5071c0c9168cfedbbaa527f82241c80b4ad53705
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261523"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="c672e-103">deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c672e-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="c672e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c672e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c672e-105">Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="c672e-105">Delete user from shared apple device action result</span></span>


<span data-ttu-id="c672e-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c672e-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c672e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c672e-107">Properties</span></span>
|<span data-ttu-id="c672e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c672e-108">Property</span></span>|<span data-ttu-id="c672e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c672e-109">Type</span></span>|<span data-ttu-id="c672e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c672e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c672e-111">actionName</span><span class="sxs-lookup"><span data-stu-id="c672e-111">actionName</span></span>|<span data-ttu-id="c672e-112">String</span><span class="sxs-lookup"><span data-stu-id="c672e-112">String</span></span>|<span data-ttu-id="c672e-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c672e-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c672e-114">actionState</span><span class="sxs-lookup"><span data-stu-id="c672e-114">actionState</span></span>|[<span data-ttu-id="c672e-115">actionState</span><span class="sxs-lookup"><span data-stu-id="c672e-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="c672e-116">Status der von [DeviceActionResult](../resources/intune-devices-deviceactionresult.md)geerbten Aktion.</span><span class="sxs-lookup"><span data-stu-id="c672e-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c672e-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c672e-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c672e-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c672e-118">startDateTime</span></span>|<span data-ttu-id="c672e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c672e-119">DateTimeOffset</span></span>|<span data-ttu-id="c672e-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c672e-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c672e-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c672e-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="c672e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c672e-122">DateTimeOffset</span></span>|<span data-ttu-id="c672e-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c672e-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c672e-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c672e-124">userPrincipalName</span></span>|<span data-ttu-id="c672e-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c672e-125">String</span></span>|<span data-ttu-id="c672e-126">Benutzerprinzipalnamen für den Benutzer, der gelöscht werden soll</span><span class="sxs-lookup"><span data-stu-id="c672e-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="c672e-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c672e-127">Relationships</span></span>
<span data-ttu-id="c672e-128">Keine</span><span class="sxs-lookup"><span data-stu-id="c672e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c672e-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c672e-129">JSON Representation</span></span>
<span data-ttu-id="c672e-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c672e-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



