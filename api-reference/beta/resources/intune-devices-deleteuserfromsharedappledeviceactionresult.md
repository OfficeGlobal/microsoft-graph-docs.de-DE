---
title: deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp
description: Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ed004ad8c02d18c19df7be0f819658603fb4fc0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861908"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="bd1f0-103">deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bd1f0-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="bd1f0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bd1f0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd1f0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd1f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd1f0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bd1f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd1f0-107">Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="bd1f0-107">Delete user from shared apple device action result</span></span>

<span data-ttu-id="bd1f0-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd1f0-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd1f0-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd1f0-109">Properties</span></span>
|<span data-ttu-id="bd1f0-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd1f0-110">Property</span></span>|<span data-ttu-id="bd1f0-111">Typ</span><span class="sxs-lookup"><span data-stu-id="bd1f0-111">Type</span></span>|<span data-ttu-id="bd1f0-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd1f0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd1f0-113">actionName</span><span class="sxs-lookup"><span data-stu-id="bd1f0-113">actionName</span></span>|<span data-ttu-id="bd1f0-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd1f0-114">String</span></span>|<span data-ttu-id="bd1f0-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd1f0-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bd1f0-116">actionState</span><span class="sxs-lookup"><span data-stu-id="bd1f0-116">actionState</span></span>|[<span data-ttu-id="bd1f0-117">actionState</span><span class="sxs-lookup"><span data-stu-id="bd1f0-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bd1f0-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bd1f0-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="bd1f0-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bd1f0-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bd1f0-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bd1f0-120">startDateTime</span></span>|<span data-ttu-id="bd1f0-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd1f0-121">DateTimeOffset</span></span>|<span data-ttu-id="bd1f0-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd1f0-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bd1f0-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd1f0-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="bd1f0-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd1f0-124">DateTimeOffset</span></span>|<span data-ttu-id="bd1f0-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd1f0-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bd1f0-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bd1f0-126">userPrincipalName</span></span>|<span data-ttu-id="bd1f0-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bd1f0-127">String</span></span>|<span data-ttu-id="bd1f0-128">Benutzerprinzipalnamen für den Benutzer, der gelöscht werden soll</span><span class="sxs-lookup"><span data-stu-id="bd1f0-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd1f0-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bd1f0-129">Relationships</span></span>
<span data-ttu-id="bd1f0-130">Keine</span><span class="sxs-lookup"><span data-stu-id="bd1f0-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bd1f0-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd1f0-131">JSON Representation</span></span>
<span data-ttu-id="bd1f0-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd1f0-132">Here is a JSON representation of the resource.</span></span>
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





