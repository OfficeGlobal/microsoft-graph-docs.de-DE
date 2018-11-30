---
title: Ressourcentyp officeConfiguration
description: Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.
ms.openlocfilehash: 4a3657153ead53a5367c23cdc51b0e40a8efe535
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060420"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="5f91a-103">Ressourcentyp officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="5f91a-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="5f91a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5f91a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f91a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f91a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f91a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5f91a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f91a-107">Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="5f91a-107">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="5f91a-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="5f91a-108">Methods</span></span>
|<span data-ttu-id="5f91a-109">Methode</span><span class="sxs-lookup"><span data-stu-id="5f91a-109">Method</span></span>|<span data-ttu-id="5f91a-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5f91a-110">Return Type</span></span>|<span data-ttu-id="5f91a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f91a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f91a-112">Abrufen von officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="5f91a-112">Get officeConfiguration</span></span>|[<span data-ttu-id="5f91a-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="5f91a-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="5f91a-114">Lesen Sie Eigenschaften und Beziehungen des [OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f91a-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="5f91a-115">OfficeConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5f91a-115">Update officeConfiguration</span></span>|[<span data-ttu-id="5f91a-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="5f91a-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="5f91a-117">Aktualisieren Sie die Eigenschaften eines [OfficeConfiguration](../resources/intune-cirrus-officeconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f91a-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f91a-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5f91a-118">Properties</span></span>
|<span data-ttu-id="5f91a-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f91a-119">Property</span></span>|<span data-ttu-id="5f91a-120">Typ</span><span class="sxs-lookup"><span data-stu-id="5f91a-120">Type</span></span>|<span data-ttu-id="5f91a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f91a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f91a-122">id</span><span class="sxs-lookup"><span data-stu-id="5f91a-122">id</span></span>|<span data-ttu-id="5f91a-123">String</span><span class="sxs-lookup"><span data-stu-id="5f91a-123">String</span></span>|<span data-ttu-id="5f91a-124">ID des Office-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="5f91a-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="5f91a-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="5f91a-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="5f91a-126">[OfficeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5f91a-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="5f91a-127">Liste der Office-Client Einchecken Status.</span><span class="sxs-lookup"><span data-stu-id="5f91a-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="5f91a-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="5f91a-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="5f91a-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="5f91a-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="5f91a-130">Entität, die Mandanten Einchecken Statuen beschreibt.</span><span class="sxs-lookup"><span data-stu-id="5f91a-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f91a-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5f91a-131">Relationships</span></span>
|<span data-ttu-id="5f91a-132">Beziehung</span><span class="sxs-lookup"><span data-stu-id="5f91a-132">Relationship</span></span>|<span data-ttu-id="5f91a-133">Typ</span><span class="sxs-lookup"><span data-stu-id="5f91a-133">Type</span></span>|<span data-ttu-id="5f91a-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f91a-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f91a-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="5f91a-135">clientConfigurations</span></span>|<span data-ttu-id="5f91a-136">[OfficeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="5f91a-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="5f91a-137">Liste der Office-Client-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="5f91a-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f91a-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5f91a-138">JSON Representation</span></span>
<span data-ttu-id="5f91a-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5f91a-139">Here is a JSON representation of the resource.</span></span>
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



