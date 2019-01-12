---
title: organization-Ressourcentyp
description: Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8bc7a0fba8c5ecdc2b2a88062855e8b279721c45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990768"
---
# <a name="organization-resource-type"></a><span data-ttu-id="8c2e5-103">organization-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8c2e5-103">organization resource type</span></span>

> <span data-ttu-id="8c2e5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c2e5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c2e5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c2e5-107">Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="8c2e5-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="8c2e5-108">Methods</span></span>
|<span data-ttu-id="8c2e5-109">Methode</span><span class="sxs-lookup"><span data-stu-id="8c2e5-109">Method</span></span>|<span data-ttu-id="8c2e5-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8c2e5-110">Return Type</span></span>|<span data-ttu-id="8c2e5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c2e5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8c2e5-112">Organisationen auflisten</span><span class="sxs-lookup"><span data-stu-id="8c2e5-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="8c2e5-113">[organization](../resources/intune-onboarding-organization.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8c2e5-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="8c2e5-114">Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune-onboarding-organization.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="8c2e5-115">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="8c2e5-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="8c2e5-116">organization</span><span class="sxs-lookup"><span data-stu-id="8c2e5-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="8c2e5-117">Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="8c2e5-118">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8c2e5-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="8c2e5-119">organization</span><span class="sxs-lookup"><span data-stu-id="8c2e5-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="8c2e5-120">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="8c2e5-121">setMobileDeviceManagementAuthority-Aktion</span><span class="sxs-lookup"><span data-stu-id="8c2e5-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="8c2e5-122">Int32</span><span class="sxs-lookup"><span data-stu-id="8c2e5-122">Int32</span></span>|<span data-ttu-id="8c2e5-123">Autorität für die Verwaltung mobiler Geräte festlegen</span><span class="sxs-lookup"><span data-stu-id="8c2e5-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="8c2e5-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8c2e5-124">Properties</span></span>
|<span data-ttu-id="8c2e5-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c2e5-125">Property</span></span>|<span data-ttu-id="8c2e5-126">Typ</span><span class="sxs-lookup"><span data-stu-id="8c2e5-126">Type</span></span>|<span data-ttu-id="8c2e5-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c2e5-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c2e5-128">id</span><span class="sxs-lookup"><span data-stu-id="8c2e5-128">id</span></span>|<span data-ttu-id="8c2e5-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8c2e5-129">String</span></span>|<span data-ttu-id="8c2e5-130">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-130">The GUID for the object.</span></span>|
|<span data-ttu-id="8c2e5-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="8c2e5-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="8c2e5-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="8c2e5-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="8c2e5-133">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-133">Mobile device management authority.</span></span> <span data-ttu-id="8c2e5-134">Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="8c2e5-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="8c2e5-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="8c2e5-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="8c2e5-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="8c2e5-137">Connector-Einstellung Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c2e5-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8c2e5-138">Relationships</span></span>
<span data-ttu-id="8c2e5-139">Keine</span><span class="sxs-lookup"><span data-stu-id="8c2e5-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c2e5-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8c2e5-140">JSON Representation</span></span>
<span data-ttu-id="8c2e5-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8c2e5-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```





