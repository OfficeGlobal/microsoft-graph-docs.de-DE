---
title: Ressourcentyp revokeAppleVppLicensesActionResult
description: Apple Vpp Lizenzen Aktionsergebnis widerrufen
ms.openlocfilehash: f751f90b90bbf282fa05a59a4a1c59d04ccfbb99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061420"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="3ee4f-103">Ressourcentyp revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="3ee4f-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="3ee4f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3ee4f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ee4f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ee4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ee4f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3ee4f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ee4f-107">Apple Vpp Lizenzen Aktionsergebnis widerrufen</span><span class="sxs-lookup"><span data-stu-id="3ee4f-107">Revoke Apple Vpp licenses action result</span></span>

<span data-ttu-id="3ee4f-108">Erbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3ee4f-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ee4f-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3ee4f-109">Properties</span></span>
|<span data-ttu-id="3ee4f-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ee4f-110">Property</span></span>|<span data-ttu-id="3ee4f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="3ee4f-111">Type</span></span>|<span data-ttu-id="3ee4f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ee4f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ee4f-113">actionName</span><span class="sxs-lookup"><span data-stu-id="3ee4f-113">actionName</span></span>|<span data-ttu-id="3ee4f-114">String</span><span class="sxs-lookup"><span data-stu-id="3ee4f-114">String</span></span>|<span data-ttu-id="3ee4f-115">Aktionsname, geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3ee4f-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3ee4f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="3ee4f-116">actionState</span></span>|[<span data-ttu-id="3ee4f-117">actionState</span><span class="sxs-lookup"><span data-stu-id="3ee4f-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="3ee4f-118">Status der Aktion Inherited aus [DeviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3ee4f-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3ee4f-119">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3ee4f-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3ee4f-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3ee4f-120">startDateTime</span></span>|<span data-ttu-id="3ee4f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ee4f-121">DateTimeOffset</span></span>|<span data-ttu-id="3ee4f-122">Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3ee4f-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3ee4f-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ee4f-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="3ee4f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ee4f-124">DateTimeOffset</span></span>|<span data-ttu-id="3ee4f-125">Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3ee4f-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3ee4f-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="3ee4f-126">totalLicensesCount</span></span>|<span data-ttu-id="3ee4f-127">Int32</span><span class="sxs-lookup"><span data-stu-id="3ee4f-127">Int32</span></span>|<span data-ttu-id="3ee4f-128">Gesamtzahl der Apple Vpp Lizenzen verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="3ee4f-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="3ee4f-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="3ee4f-129">failedLicensesCount</span></span>|<span data-ttu-id="3ee4f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="3ee4f-130">Int32</span></span>|<span data-ttu-id="3ee4f-131">Gesamtzahl der Apple Vpp-Lizenzen, die nicht widerrufen</span><span class="sxs-lookup"><span data-stu-id="3ee4f-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ee4f-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3ee4f-132">Relationships</span></span>
<span data-ttu-id="3ee4f-133">Keine</span><span class="sxs-lookup"><span data-stu-id="3ee4f-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3ee4f-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3ee4f-134">JSON Representation</span></span>
<span data-ttu-id="3ee4f-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3ee4f-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```





