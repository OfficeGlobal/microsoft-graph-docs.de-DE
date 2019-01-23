---
title: deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp
description: Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c65a1c60a77ba196448dd626b345c69c71f16de6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399276"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="b4cac-103">deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b4cac-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="b4cac-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b4cac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4cac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4cac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4cac-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4cac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4cac-107">Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="b4cac-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="b4cac-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b4cac-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4cac-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4cac-109">Properties</span></span>
|<span data-ttu-id="b4cac-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4cac-110">Property</span></span>|<span data-ttu-id="b4cac-111">Typ</span><span class="sxs-lookup"><span data-stu-id="b4cac-111">Type</span></span>|<span data-ttu-id="b4cac-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4cac-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4cac-113">actionName</span><span class="sxs-lookup"><span data-stu-id="b4cac-113">actionName</span></span>|<span data-ttu-id="b4cac-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4cac-114">String</span></span>|<span data-ttu-id="b4cac-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b4cac-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b4cac-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b4cac-116">actionState</span></span>|[<span data-ttu-id="b4cac-117">actionState</span><span class="sxs-lookup"><span data-stu-id="b4cac-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b4cac-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b4cac-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b4cac-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b4cac-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b4cac-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b4cac-120">startDateTime</span></span>|<span data-ttu-id="b4cac-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4cac-121">DateTimeOffset</span></span>|<span data-ttu-id="b4cac-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b4cac-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b4cac-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4cac-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="b4cac-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4cac-124">DateTimeOffset</span></span>|<span data-ttu-id="b4cac-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b4cac-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b4cac-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b4cac-126">userPrincipalName</span></span>|<span data-ttu-id="b4cac-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4cac-127">String</span></span>|<span data-ttu-id="b4cac-128">Benutzerprinzipalnamen für den Benutzer, der gelöscht werden soll</span><span class="sxs-lookup"><span data-stu-id="b4cac-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4cac-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b4cac-129">Relationships</span></span>
<span data-ttu-id="b4cac-130">Keine</span><span class="sxs-lookup"><span data-stu-id="b4cac-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4cac-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4cac-131">JSON Representation</span></span>
<span data-ttu-id="b4cac-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4cac-132">Here is a JSON representation of the resource.</span></span>
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




