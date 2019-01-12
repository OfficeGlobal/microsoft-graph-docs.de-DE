---
title: deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp
description: Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 997b9d9339abe44f8bc7427d9533b43066eac3b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975456"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="9dff1-103">deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9dff1-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="9dff1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9dff1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9dff1-105">Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="9dff1-105">Delete user from shared apple device action result</span></span>

<span data-ttu-id="9dff1-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9dff1-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9dff1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9dff1-107">Properties</span></span>
|<span data-ttu-id="9dff1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9dff1-108">Property</span></span>|<span data-ttu-id="9dff1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9dff1-109">Type</span></span>|<span data-ttu-id="9dff1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9dff1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dff1-111">actionName</span><span class="sxs-lookup"><span data-stu-id="9dff1-111">actionName</span></span>|<span data-ttu-id="9dff1-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9dff1-112">String</span></span>|<span data-ttu-id="9dff1-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9dff1-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9dff1-114">actionState</span><span class="sxs-lookup"><span data-stu-id="9dff1-114">actionState</span></span>|[<span data-ttu-id="9dff1-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9dff1-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="9dff1-116">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9dff1-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9dff1-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9dff1-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9dff1-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9dff1-118">startDateTime</span></span>|<span data-ttu-id="9dff1-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dff1-119">DateTimeOffset</span></span>|<span data-ttu-id="9dff1-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9dff1-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9dff1-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9dff1-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="9dff1-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dff1-122">DateTimeOffset</span></span>|<span data-ttu-id="9dff1-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9dff1-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9dff1-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9dff1-124">userPrincipalName</span></span>|<span data-ttu-id="9dff1-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9dff1-125">String</span></span>|<span data-ttu-id="9dff1-126">Benutzerprinzipalnamen für den Benutzer, der gelöscht werden soll</span><span class="sxs-lookup"><span data-stu-id="9dff1-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dff1-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9dff1-127">Relationships</span></span>
<span data-ttu-id="9dff1-128">Keine</span><span class="sxs-lookup"><span data-stu-id="9dff1-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9dff1-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9dff1-129">JSON Representation</span></span>
<span data-ttu-id="9dff1-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9dff1-130">Here is a JSON representation of the resource.</span></span>
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



