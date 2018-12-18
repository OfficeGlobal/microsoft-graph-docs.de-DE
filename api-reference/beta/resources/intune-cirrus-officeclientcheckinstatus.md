---
title: Ressourcentyp officeClientCheckinStatus
description: Entität, die Mandanten Einchecken Stats beschreibt.
author: tfitzmac
ms.openlocfilehash: 0c6359d3cb6c776d0f26fdaf88ce7f2f03e5f8c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331717"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="9cd75-103">Ressourcentyp officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="9cd75-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="9cd75-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9cd75-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9cd75-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9cd75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cd75-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9cd75-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9cd75-107">Entität, die Mandanten Einchecken Stats beschreibt.</span><span class="sxs-lookup"><span data-stu-id="9cd75-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="9cd75-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9cd75-108">Properties</span></span>
|<span data-ttu-id="9cd75-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9cd75-109">Property</span></span>|<span data-ttu-id="9cd75-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9cd75-110">Type</span></span>|<span data-ttu-id="9cd75-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9cd75-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cd75-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9cd75-112">userPrincipalName</span></span>|<span data-ttu-id="9cd75-113">String</span><span class="sxs-lookup"><span data-stu-id="9cd75-113">String</span></span>|<span data-ttu-id="9cd75-114">Benutzerprinzipalname des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9cd75-114">User principal name using the device.</span></span>|
|<span data-ttu-id="9cd75-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="9cd75-115">deviceName</span></span>|<span data-ttu-id="9cd75-116">String</span><span class="sxs-lookup"><span data-stu-id="9cd75-116">String</span></span>|<span data-ttu-id="9cd75-117">Name des Aufnahmegeräts einchecken möchten.</span><span class="sxs-lookup"><span data-stu-id="9cd75-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="9cd75-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="9cd75-118">devicePlatform</span></span>|<span data-ttu-id="9cd75-119">String</span><span class="sxs-lookup"><span data-stu-id="9cd75-119">String</span></span>|<span data-ttu-id="9cd75-120">Geräteplattform einchecken möchten.</span><span class="sxs-lookup"><span data-stu-id="9cd75-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="9cd75-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="9cd75-121">devicePlatformVersion</span></span>|<span data-ttu-id="9cd75-122">String</span><span class="sxs-lookup"><span data-stu-id="9cd75-122">String</span></span>|<span data-ttu-id="9cd75-123">Gerät Plattformversion einchecken möchten.</span><span class="sxs-lookup"><span data-stu-id="9cd75-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="9cd75-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="9cd75-124">wasSuccessful</span></span>|<span data-ttu-id="9cd75-125">Boolesch</span><span class="sxs-lookup"><span data-stu-id="9cd75-125">Boolean</span></span>|<span data-ttu-id="9cd75-126">Wenn das letzte Einchecken erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="9cd75-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="9cd75-127">userId</span><span class="sxs-lookup"><span data-stu-id="9cd75-127">userId</span></span>|<span data-ttu-id="9cd75-128">String</span><span class="sxs-lookup"><span data-stu-id="9cd75-128">String</span></span>|<span data-ttu-id="9cd75-129">Benutzer-ID des Geräts.</span><span class="sxs-lookup"><span data-stu-id="9cd75-129">User identifier using the device.</span></span>|
|<span data-ttu-id="9cd75-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="9cd75-130">checkinDateTime</span></span>|<span data-ttu-id="9cd75-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cd75-131">DateTimeOffset</span></span>|<span data-ttu-id="9cd75-132">Letzte Gerät Einchecken Zeitpunkt in UTC.</span><span class="sxs-lookup"><span data-stu-id="9cd75-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="9cd75-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="9cd75-133">errorMessage</span></span>|<span data-ttu-id="9cd75-134">String</span><span class="sxs-lookup"><span data-stu-id="9cd75-134">String</span></span>|<span data-ttu-id="9cd75-135">Fehlermeldung, wenn alle zugeordneten für das letzte einchecken.</span><span class="sxs-lookup"><span data-stu-id="9cd75-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="9cd75-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="9cd75-136">appliedPolicies</span></span>|<span data-ttu-id="9cd75-137">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="9cd75-137">String collection</span></span>|<span data-ttu-id="9cd75-138">Liste der Richtlinien an das Gerät als letzten Checkin übermittelt wurden.</span><span class="sxs-lookup"><span data-stu-id="9cd75-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cd75-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9cd75-139">Relationships</span></span>
<span data-ttu-id="9cd75-140">Keine</span><span class="sxs-lookup"><span data-stu-id="9cd75-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9cd75-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9cd75-141">JSON Representation</span></span>
<span data-ttu-id="9cd75-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9cd75-142">Here is a JSON representation of the resource.</span></span>
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



