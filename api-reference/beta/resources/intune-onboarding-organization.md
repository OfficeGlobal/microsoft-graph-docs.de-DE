---
title: organization-Ressourcentyp
description: Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6de006bf465546fdb00769f5d3541a65a6b5580b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167508"
---
# <a name="organization-resource-type"></a><span data-ttu-id="56e94-103">organization-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="56e94-103">organization resource type</span></span>

> <span data-ttu-id="56e94-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56e94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56e94-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="56e94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56e94-106">Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="56e94-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="56e94-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="56e94-107">Methods</span></span>
|<span data-ttu-id="56e94-108">Methode</span><span class="sxs-lookup"><span data-stu-id="56e94-108">Method</span></span>|<span data-ttu-id="56e94-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="56e94-109">Return Type</span></span>|<span data-ttu-id="56e94-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56e94-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56e94-111">Organisationen auflisten</span><span class="sxs-lookup"><span data-stu-id="56e94-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="56e94-112">[organization](../resources/intune-onboarding-organization.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="56e94-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="56e94-113">Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune-onboarding-organization.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="56e94-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="56e94-114">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="56e94-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="56e94-115">organization</span><span class="sxs-lookup"><span data-stu-id="56e94-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="56e94-116">Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="56e94-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="56e94-117">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="56e94-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="56e94-118">organization</span><span class="sxs-lookup"><span data-stu-id="56e94-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="56e94-119">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="56e94-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="56e94-120">setMobileDeviceManagementAuthority-Aktion</span><span class="sxs-lookup"><span data-stu-id="56e94-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="56e94-121">Int32</span><span class="sxs-lookup"><span data-stu-id="56e94-121">Int32</span></span>|<span data-ttu-id="56e94-122">Autorität für die Verwaltung mobiler Geräte festlegen</span><span class="sxs-lookup"><span data-stu-id="56e94-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="56e94-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="56e94-123">Properties</span></span>
|<span data-ttu-id="56e94-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56e94-124">Property</span></span>|<span data-ttu-id="56e94-125">Typ</span><span class="sxs-lookup"><span data-stu-id="56e94-125">Type</span></span>|<span data-ttu-id="56e94-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56e94-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56e94-127">id</span><span class="sxs-lookup"><span data-stu-id="56e94-127">id</span></span>|<span data-ttu-id="56e94-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56e94-128">String</span></span>|<span data-ttu-id="56e94-129">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="56e94-129">The GUID for the object.</span></span>|
|<span data-ttu-id="56e94-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="56e94-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="56e94-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="56e94-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="56e94-132">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="56e94-132">Mobile device management authority.</span></span> <span data-ttu-id="56e94-133">Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="56e94-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="56e94-134">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="56e94-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="56e94-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="56e94-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="56e94-136">Zertifikat-Connector-Einstellung.</span><span class="sxs-lookup"><span data-stu-id="56e94-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56e94-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="56e94-137">Relationships</span></span>
<span data-ttu-id="56e94-138">Keine</span><span class="sxs-lookup"><span data-stu-id="56e94-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56e94-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="56e94-139">JSON Representation</span></span>
<span data-ttu-id="56e94-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="56e94-140">Here is a JSON representation of the resource.</span></span>
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




