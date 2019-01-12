---
title: Ressourcentyp officeClientCheckinStatus
description: Entität, die Mandanten Einchecken Stats beschreibt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a387e04b9ebc15d65eb8dd883ecd4a9bae78ad6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969289"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="e7e78-103">Ressourcentyp officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="e7e78-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="e7e78-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e7e78-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7e78-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e7e78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7e78-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e7e78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7e78-107">Entität, die Mandanten Einchecken Stats beschreibt.</span><span class="sxs-lookup"><span data-stu-id="e7e78-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="e7e78-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e7e78-108">Properties</span></span>
|<span data-ttu-id="e7e78-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e7e78-109">Property</span></span>|<span data-ttu-id="e7e78-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e7e78-110">Type</span></span>|<span data-ttu-id="e7e78-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7e78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7e78-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e7e78-112">userPrincipalName</span></span>|<span data-ttu-id="e7e78-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e78-113">String</span></span>|<span data-ttu-id="e7e78-114">Benutzerprinzipalname des Geräts.</span><span class="sxs-lookup"><span data-stu-id="e7e78-114">User principal name using the device.</span></span>|
|<span data-ttu-id="e7e78-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="e7e78-115">deviceName</span></span>|<span data-ttu-id="e7e78-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e78-116">String</span></span>|<span data-ttu-id="e7e78-117">Name des Aufnahmegeräts einchecken möchten.</span><span class="sxs-lookup"><span data-stu-id="e7e78-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="e7e78-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="e7e78-118">devicePlatform</span></span>|<span data-ttu-id="e7e78-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e78-119">String</span></span>|<span data-ttu-id="e7e78-120">Geräteplattform einchecken möchten.</span><span class="sxs-lookup"><span data-stu-id="e7e78-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="e7e78-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="e7e78-121">devicePlatformVersion</span></span>|<span data-ttu-id="e7e78-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e78-122">String</span></span>|<span data-ttu-id="e7e78-123">Gerät Plattformversion einchecken möchten.</span><span class="sxs-lookup"><span data-stu-id="e7e78-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="e7e78-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="e7e78-124">wasSuccessful</span></span>|<span data-ttu-id="e7e78-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e7e78-125">Boolean</span></span>|<span data-ttu-id="e7e78-126">Wenn das letzte Einchecken erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="e7e78-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="e7e78-127">userId</span><span class="sxs-lookup"><span data-stu-id="e7e78-127">userId</span></span>|<span data-ttu-id="e7e78-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e78-128">String</span></span>|<span data-ttu-id="e7e78-129">Benutzer-ID des Geräts.</span><span class="sxs-lookup"><span data-stu-id="e7e78-129">User identifier using the device.</span></span>|
|<span data-ttu-id="e7e78-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="e7e78-130">checkinDateTime</span></span>|<span data-ttu-id="e7e78-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7e78-131">DateTimeOffset</span></span>|<span data-ttu-id="e7e78-132">Letzte Gerät Einchecken Zeitpunkt in UTC.</span><span class="sxs-lookup"><span data-stu-id="e7e78-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="e7e78-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="e7e78-133">errorMessage</span></span>|<span data-ttu-id="e7e78-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e78-134">String</span></span>|<span data-ttu-id="e7e78-135">Fehlermeldung, wenn alle zugeordneten für das letzte einchecken.</span><span class="sxs-lookup"><span data-stu-id="e7e78-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="e7e78-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="e7e78-136">appliedPolicies</span></span>|<span data-ttu-id="e7e78-137">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="e7e78-137">String collection</span></span>|<span data-ttu-id="e7e78-138">Liste der Richtlinien an das Gerät als letzten Checkin übermittelt wurden.</span><span class="sxs-lookup"><span data-stu-id="e7e78-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7e78-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e7e78-139">Relationships</span></span>
<span data-ttu-id="e7e78-140">Keine</span><span class="sxs-lookup"><span data-stu-id="e7e78-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e7e78-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e7e78-141">JSON Representation</span></span>
<span data-ttu-id="e7e78-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e7e78-142">Here is a JSON representation of the resource.</span></span>
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



