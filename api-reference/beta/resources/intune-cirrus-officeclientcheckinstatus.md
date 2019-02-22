---
title: officeClientCheckinStatus-Ressourcentyp
description: Entität, die den Eincheckstatus für Mandanten beschreibt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 465b07ba286b9ee3a58132424be2a25b1c7e564e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156056"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="9ef5e-103">officeClientCheckinStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9ef5e-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="9ef5e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ef5e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ef5e-106">Entität, die den Eincheckstatus für Mandanten beschreibt.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-106">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="9ef5e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9ef5e-107">Properties</span></span>
|<span data-ttu-id="9ef5e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ef5e-108">Property</span></span>|<span data-ttu-id="9ef5e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9ef5e-109">Type</span></span>|<span data-ttu-id="9ef5e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ef5e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef5e-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9ef5e-111">userPrincipalName</span></span>|<span data-ttu-id="9ef5e-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ef5e-112">String</span></span>|<span data-ttu-id="9ef5e-113">Benutzerprinzipalname, der das Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-113">User principal name using the device.</span></span>|
|<span data-ttu-id="9ef5e-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="9ef5e-114">deviceName</span></span>|<span data-ttu-id="9ef5e-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ef5e-115">String</span></span>|<span data-ttu-id="9ef5e-116">Gerätename, der versucht einzuchecken.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-116">Device name trying to check-in.</span></span>|
|<span data-ttu-id="9ef5e-117">Deviceplatform wurde</span><span class="sxs-lookup"><span data-stu-id="9ef5e-117">devicePlatform</span></span>|<span data-ttu-id="9ef5e-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ef5e-118">String</span></span>|<span data-ttu-id="9ef5e-119">Geräteplattform, die versucht, einzuchecken.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-119">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="9ef5e-120">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="9ef5e-120">devicePlatformVersion</span></span>|<span data-ttu-id="9ef5e-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ef5e-121">String</span></span>|<span data-ttu-id="9ef5e-122">Geräte Plattformversion, die versucht, einzuchecken.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-122">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="9ef5e-123">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="9ef5e-123">wasSuccessful</span></span>|<span data-ttu-id="9ef5e-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9ef5e-124">Boolean</span></span>|<span data-ttu-id="9ef5e-125">Wenn das letzte Einchecken erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-125">If the last checkin was successful.</span></span>|
|<span data-ttu-id="9ef5e-126">userId</span><span class="sxs-lookup"><span data-stu-id="9ef5e-126">userId</span></span>|<span data-ttu-id="9ef5e-127">String</span><span class="sxs-lookup"><span data-stu-id="9ef5e-127">String</span></span>|<span data-ttu-id="9ef5e-128">Benutzer-ID, die das Gerät verwendet.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-128">User identifier using the device.</span></span>|
|<span data-ttu-id="9ef5e-129">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="9ef5e-129">checkinDateTime</span></span>|<span data-ttu-id="9ef5e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ef5e-130">DateTimeOffset</span></span>|<span data-ttu-id="9ef5e-131">Zeitpunkt der letzten Geräteüberprüfung in UTC.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-131">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="9ef5e-132">errorMessage</span><span class="sxs-lookup"><span data-stu-id="9ef5e-132">errorMessage</span></span>|<span data-ttu-id="9ef5e-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ef5e-133">String</span></span>|<span data-ttu-id="9ef5e-134">Fehlermeldung, wenn für das letzte Einchecken verknüpft.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-134">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="9ef5e-135">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="9ef5e-135">appliedPolicies</span></span>|<span data-ttu-id="9ef5e-136">String collection</span><span class="sxs-lookup"><span data-stu-id="9ef5e-136">String collection</span></span>|<span data-ttu-id="9ef5e-137">Liste der Richtlinien, die beim letzten Einchecken an das Gerät übermittelt wurden.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-137">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ef5e-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9ef5e-138">Relationships</span></span>
<span data-ttu-id="9ef5e-139">Keine</span><span class="sxs-lookup"><span data-stu-id="9ef5e-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ef5e-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9ef5e-140">JSON Representation</span></span>
<span data-ttu-id="9ef5e-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9ef5e-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```



