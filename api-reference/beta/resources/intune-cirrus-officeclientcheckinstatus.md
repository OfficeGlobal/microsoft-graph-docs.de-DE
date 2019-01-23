---
title: Ressourcentyp officeClientCheckinStatus
description: Entität, die Mandanten Einchecken Stats beschreibt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebc534a6c424a9dac4316d0029e2fd35839f0a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403259"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="45a54-103">Ressourcentyp officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="45a54-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="45a54-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="45a54-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45a54-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="45a54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45a54-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="45a54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45a54-107">Entität, die Mandanten Einchecken Stats beschreibt.</span><span class="sxs-lookup"><span data-stu-id="45a54-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="45a54-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="45a54-108">Properties</span></span>
|<span data-ttu-id="45a54-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="45a54-109">Property</span></span>|<span data-ttu-id="45a54-110">Typ</span><span class="sxs-lookup"><span data-stu-id="45a54-110">Type</span></span>|<span data-ttu-id="45a54-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45a54-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a54-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="45a54-112">userPrincipalName</span></span>|<span data-ttu-id="45a54-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="45a54-113">String</span></span>|<span data-ttu-id="45a54-114">Benutzerprinzipalname des Geräts.</span><span class="sxs-lookup"><span data-stu-id="45a54-114">User principal name using the device.</span></span>|
|<span data-ttu-id="45a54-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="45a54-115">deviceName</span></span>|<span data-ttu-id="45a54-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="45a54-116">String</span></span>|<span data-ttu-id="45a54-117">Name des Aufnahmegeräts einchecken möchten.</span><span class="sxs-lookup"><span data-stu-id="45a54-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="45a54-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="45a54-118">devicePlatform</span></span>|<span data-ttu-id="45a54-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="45a54-119">String</span></span>|<span data-ttu-id="45a54-120">Geräteplattform einchecken möchten.</span><span class="sxs-lookup"><span data-stu-id="45a54-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="45a54-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="45a54-121">devicePlatformVersion</span></span>|<span data-ttu-id="45a54-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="45a54-122">String</span></span>|<span data-ttu-id="45a54-123">Gerät Plattformversion einchecken möchten.</span><span class="sxs-lookup"><span data-stu-id="45a54-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="45a54-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="45a54-124">wasSuccessful</span></span>|<span data-ttu-id="45a54-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="45a54-125">Boolean</span></span>|<span data-ttu-id="45a54-126">Wenn das letzte Einchecken erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="45a54-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="45a54-127">userId</span><span class="sxs-lookup"><span data-stu-id="45a54-127">userId</span></span>|<span data-ttu-id="45a54-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="45a54-128">String</span></span>|<span data-ttu-id="45a54-129">Benutzer-ID des Geräts.</span><span class="sxs-lookup"><span data-stu-id="45a54-129">User identifier using the device.</span></span>|
|<span data-ttu-id="45a54-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="45a54-130">checkinDateTime</span></span>|<span data-ttu-id="45a54-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45a54-131">DateTimeOffset</span></span>|<span data-ttu-id="45a54-132">Letzte Gerät Einchecken Zeitpunkt in UTC.</span><span class="sxs-lookup"><span data-stu-id="45a54-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="45a54-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="45a54-133">errorMessage</span></span>|<span data-ttu-id="45a54-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="45a54-134">String</span></span>|<span data-ttu-id="45a54-135">Fehlermeldung, wenn alle zugeordneten für das letzte einchecken.</span><span class="sxs-lookup"><span data-stu-id="45a54-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="45a54-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="45a54-136">appliedPolicies</span></span>|<span data-ttu-id="45a54-137">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="45a54-137">String collection</span></span>|<span data-ttu-id="45a54-138">Liste der Richtlinien an das Gerät als letzten Checkin übermittelt wurden.</span><span class="sxs-lookup"><span data-stu-id="45a54-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45a54-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="45a54-139">Relationships</span></span>
<span data-ttu-id="45a54-140">Keine</span><span class="sxs-lookup"><span data-stu-id="45a54-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45a54-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="45a54-141">JSON Representation</span></span>
<span data-ttu-id="45a54-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="45a54-142">Here is a JSON representation of the resource.</span></span>
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



