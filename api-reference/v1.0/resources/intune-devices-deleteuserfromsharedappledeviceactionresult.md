---
title: deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp
description: Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis
ms.openlocfilehash: dc21e22ca2e819835178a7cb2ed3aa824cd40004
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016072"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="23435-103">deleteUserFromSharedAppleDeviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="23435-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="23435-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23435-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23435-105">Benutzer von freigegebenem Apple-Gerät löschen – Aktionsergebnis</span><span class="sxs-lookup"><span data-stu-id="23435-105">Delete user from shared apple device action result</span></span>

<span data-ttu-id="23435-106">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23435-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23435-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23435-107">Properties</span></span>
|<span data-ttu-id="23435-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23435-108">Property</span></span>|<span data-ttu-id="23435-109">Typ</span><span class="sxs-lookup"><span data-stu-id="23435-109">Type</span></span>|<span data-ttu-id="23435-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23435-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23435-111">actionName</span><span class="sxs-lookup"><span data-stu-id="23435-111">actionName</span></span>|<span data-ttu-id="23435-112">String</span><span class="sxs-lookup"><span data-stu-id="23435-112">String</span></span>|<span data-ttu-id="23435-113">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23435-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="23435-114">actionState</span><span class="sxs-lookup"><span data-stu-id="23435-114">actionState</span></span>|[<span data-ttu-id="23435-115">actionState</span><span class="sxs-lookup"><span data-stu-id="23435-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="23435-116">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="23435-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="23435-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="23435-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="23435-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="23435-118">startDateTime</span></span>|<span data-ttu-id="23435-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23435-119">DateTimeOffset</span></span>|<span data-ttu-id="23435-120">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23435-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="23435-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="23435-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="23435-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23435-122">DateTimeOffset</span></span>|<span data-ttu-id="23435-123">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="23435-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="23435-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23435-124">userPrincipalName</span></span>|<span data-ttu-id="23435-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23435-125">String</span></span>|<span data-ttu-id="23435-126">Benutzerprinzipalnamen für den Benutzer, der gelöscht werden soll</span><span class="sxs-lookup"><span data-stu-id="23435-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="23435-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="23435-127">Relationships</span></span>
<span data-ttu-id="23435-128">Keine</span><span class="sxs-lookup"><span data-stu-id="23435-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23435-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23435-129">JSON Representation</span></span>
<span data-ttu-id="23435-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23435-130">Here is a JSON representation of the resource.</span></span>
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



