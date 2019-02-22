---
title: officeConfiguration-Ressourcentyp
description: Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7e5c36a23be0ab32a14a08eaff297b832ba5274c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156049"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="08695-103">officeConfiguration-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="08695-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="08695-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08695-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08695-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="08695-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08695-106">Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="08695-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="08695-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="08695-107">Methods</span></span>
|<span data-ttu-id="08695-108">Methode</span><span class="sxs-lookup"><span data-stu-id="08695-108">Method</span></span>|<span data-ttu-id="08695-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="08695-109">Return Type</span></span>|<span data-ttu-id="08695-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08695-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08695-111">OfficeConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="08695-111">Get officeConfiguration</span></span>|[<span data-ttu-id="08695-112">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="08695-112">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="08695-113">Lesen von Eigenschaften und Beziehungen des [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="08695-113">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="08695-114">OfficeConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="08695-114">Update officeConfiguration</span></span>|[<span data-ttu-id="08695-115">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="08695-115">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="08695-116">Aktualisieren der Eigenschaften eines [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="08695-116">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="08695-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08695-117">Properties</span></span>
|<span data-ttu-id="08695-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08695-118">Property</span></span>|<span data-ttu-id="08695-119">Typ</span><span class="sxs-lookup"><span data-stu-id="08695-119">Type</span></span>|<span data-ttu-id="08695-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08695-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08695-121">id</span><span class="sxs-lookup"><span data-stu-id="08695-121">id</span></span>|<span data-ttu-id="08695-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08695-122">String</span></span>|<span data-ttu-id="08695-123">ID der Office-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="08695-123">Id of the office configuration.</span></span>|
|<span data-ttu-id="08695-124">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="08695-124">tenantCheckinStatuses</span></span>|<span data-ttu-id="08695-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="08695-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="08695-126">Liste der Office-Client Eincheckstatus.</span><span class="sxs-lookup"><span data-stu-id="08695-126">List of office Client check-in status.</span></span>|
|<span data-ttu-id="08695-127">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="08695-127">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="08695-128">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="08695-128">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="08695-129">Entität, die das Einchecken von Mandanten beschreibt</span><span class="sxs-lookup"><span data-stu-id="08695-129">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="08695-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="08695-130">Relationships</span></span>
|<span data-ttu-id="08695-131">Beziehung</span><span class="sxs-lookup"><span data-stu-id="08695-131">Relationship</span></span>|<span data-ttu-id="08695-132">Typ</span><span class="sxs-lookup"><span data-stu-id="08695-132">Type</span></span>|<span data-ttu-id="08695-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08695-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08695-134">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="08695-134">clientConfigurations</span></span>|<span data-ttu-id="08695-135">[für](../resources/intune-cirrus-officeclientconfiguration.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="08695-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="08695-136">Liste der Office-Client Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="08695-136">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08695-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08695-137">JSON Representation</span></span>
<span data-ttu-id="08695-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08695-138">Here is a JSON representation of the resource.</span></span>
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



