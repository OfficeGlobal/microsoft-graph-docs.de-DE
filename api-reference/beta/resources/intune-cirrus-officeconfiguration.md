---
title: Ressourcentyp officeConfiguration
description: Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 767782e26dd203e2ab5488b30520d8cbcf44d1e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921360"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="86367-103">Ressourcentyp officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="86367-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="86367-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="86367-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86367-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="86367-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86367-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="86367-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86367-107">Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="86367-107">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="86367-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="86367-108">Methods</span></span>
|<span data-ttu-id="86367-109">Methode</span><span class="sxs-lookup"><span data-stu-id="86367-109">Method</span></span>|<span data-ttu-id="86367-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="86367-110">Return Type</span></span>|<span data-ttu-id="86367-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86367-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86367-112">Abrufen von officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="86367-112">Get officeConfiguration</span></span>|[<span data-ttu-id="86367-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="86367-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="86367-114">Lesen Sie Eigenschaften und Beziehungen des [OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="86367-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="86367-115">OfficeConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="86367-115">Update officeConfiguration</span></span>|[<span data-ttu-id="86367-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="86367-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="86367-117">Aktualisieren Sie die Eigenschaften eines [OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="86367-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="86367-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="86367-118">Properties</span></span>
|<span data-ttu-id="86367-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86367-119">Property</span></span>|<span data-ttu-id="86367-120">Typ</span><span class="sxs-lookup"><span data-stu-id="86367-120">Type</span></span>|<span data-ttu-id="86367-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86367-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86367-122">id</span><span class="sxs-lookup"><span data-stu-id="86367-122">id</span></span>|<span data-ttu-id="86367-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86367-123">String</span></span>|<span data-ttu-id="86367-124">ID des Office-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="86367-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="86367-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="86367-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="86367-126">[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="86367-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="86367-127">Liste der Office-Client Einchecken Status.</span><span class="sxs-lookup"><span data-stu-id="86367-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="86367-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="86367-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="86367-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="86367-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="86367-130">Entität, die Mandanten Einchecken Statuen beschreibt.</span><span class="sxs-lookup"><span data-stu-id="86367-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="86367-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="86367-131">Relationships</span></span>
|<span data-ttu-id="86367-132">Beziehung</span><span class="sxs-lookup"><span data-stu-id="86367-132">Relationship</span></span>|<span data-ttu-id="86367-133">Typ</span><span class="sxs-lookup"><span data-stu-id="86367-133">Type</span></span>|<span data-ttu-id="86367-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86367-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86367-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="86367-135">clientConfigurations</span></span>|<span data-ttu-id="86367-136">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="86367-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="86367-137">Liste der Office-Client-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="86367-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86367-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="86367-138">JSON Representation</span></span>
<span data-ttu-id="86367-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="86367-139">Here is a JSON representation of the resource.</span></span>
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



