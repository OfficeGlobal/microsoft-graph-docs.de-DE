---
title: Ressourcentyp officeConfiguration
description: Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc76295b21602328689ee48f8aed8be74bd82093
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406549"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="bdf4e-103">Ressourcentyp officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdf4e-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="bdf4e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bdf4e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdf4e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdf4e-107">Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="bdf4e-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="bdf4e-108">Methods</span></span>
|<span data-ttu-id="bdf4e-109">Methode</span><span class="sxs-lookup"><span data-stu-id="bdf4e-109">Method</span></span>|<span data-ttu-id="bdf4e-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bdf4e-110">Return Type</span></span>|<span data-ttu-id="bdf4e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdf4e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdf4e-112">Abrufen von officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdf4e-112">Get officeConfiguration</span></span>|[<span data-ttu-id="bdf4e-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdf4e-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="bdf4e-114">Lesen Sie Eigenschaften und Beziehungen des [OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="bdf4e-115">OfficeConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bdf4e-115">Update officeConfiguration</span></span>|[<span data-ttu-id="bdf4e-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdf4e-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="bdf4e-117">Aktualisieren Sie die Eigenschaften eines [OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bdf4e-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bdf4e-118">Properties</span></span>
|<span data-ttu-id="bdf4e-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bdf4e-119">Property</span></span>|<span data-ttu-id="bdf4e-120">Typ</span><span class="sxs-lookup"><span data-stu-id="bdf4e-120">Type</span></span>|<span data-ttu-id="bdf4e-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdf4e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdf4e-122">id</span><span class="sxs-lookup"><span data-stu-id="bdf4e-122">id</span></span>|<span data-ttu-id="bdf4e-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bdf4e-123">String</span></span>|<span data-ttu-id="bdf4e-124">ID des Office-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="bdf4e-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="bdf4e-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="bdf4e-126">[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bdf4e-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="bdf4e-127">Liste der Office-Client Einchecken Status.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="bdf4e-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bdf4e-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="bdf4e-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="bdf4e-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="bdf4e-130">Entität, die Mandanten Einchecken Statuen beschreibt.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdf4e-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bdf4e-131">Relationships</span></span>
|<span data-ttu-id="bdf4e-132">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bdf4e-132">Relationship</span></span>|<span data-ttu-id="bdf4e-133">Typ</span><span class="sxs-lookup"><span data-stu-id="bdf4e-133">Type</span></span>|<span data-ttu-id="bdf4e-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdf4e-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdf4e-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="bdf4e-135">clientConfigurations</span></span>|<span data-ttu-id="bdf4e-136">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="bdf4e-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="bdf4e-137">Liste der Office-Client-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdf4e-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bdf4e-138">JSON Representation</span></span>
<span data-ttu-id="bdf4e-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bdf4e-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
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
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```



