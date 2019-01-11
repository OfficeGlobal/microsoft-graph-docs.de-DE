---
title: organization-Ressourcentyp
description: Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7c6f99c378bc7fd53f473419a5ca4f4350f7c57b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812047"
---
# <a name="organization-resource-type"></a><span data-ttu-id="e901b-103">organization-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e901b-103">organization resource type</span></span>

> <span data-ttu-id="e901b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e901b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e901b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e901b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e901b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e901b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e901b-107">Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="e901b-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="e901b-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="e901b-108">Methods</span></span>
|<span data-ttu-id="e901b-109">Methode</span><span class="sxs-lookup"><span data-stu-id="e901b-109">Method</span></span>|<span data-ttu-id="e901b-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e901b-110">Return Type</span></span>|<span data-ttu-id="e901b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e901b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e901b-112">Organisationen auflisten</span><span class="sxs-lookup"><span data-stu-id="e901b-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="e901b-113">[organization](../resources/intune-onboarding-organization.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e901b-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="e901b-114">Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune-onboarding-organization.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="e901b-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="e901b-115">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="e901b-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="e901b-116">organization</span><span class="sxs-lookup"><span data-stu-id="e901b-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="e901b-117">Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e901b-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="e901b-118">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e901b-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="e901b-119">organization</span><span class="sxs-lookup"><span data-stu-id="e901b-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="e901b-120">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e901b-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="e901b-121">setMobileDeviceManagementAuthority-Aktion</span><span class="sxs-lookup"><span data-stu-id="e901b-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="e901b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e901b-122">Int32</span></span>|<span data-ttu-id="e901b-123">Autorität für die Verwaltung mobiler Geräte festlegen</span><span class="sxs-lookup"><span data-stu-id="e901b-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="e901b-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e901b-124">Properties</span></span>
|<span data-ttu-id="e901b-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e901b-125">Property</span></span>|<span data-ttu-id="e901b-126">Typ</span><span class="sxs-lookup"><span data-stu-id="e901b-126">Type</span></span>|<span data-ttu-id="e901b-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e901b-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e901b-128">id</span><span class="sxs-lookup"><span data-stu-id="e901b-128">id</span></span>|<span data-ttu-id="e901b-129">String</span><span class="sxs-lookup"><span data-stu-id="e901b-129">String</span></span>|<span data-ttu-id="e901b-130">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="e901b-130">The GUID for the object.</span></span>|
|<span data-ttu-id="e901b-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e901b-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="e901b-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="e901b-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="e901b-133">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="e901b-133">Mobile device management authority.</span></span> <span data-ttu-id="e901b-134">Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="e901b-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="e901b-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="e901b-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="e901b-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="e901b-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="e901b-137">Connector-Einstellung Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="e901b-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e901b-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e901b-138">Relationships</span></span>
<span data-ttu-id="e901b-139">Keine</span><span class="sxs-lookup"><span data-stu-id="e901b-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e901b-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e901b-140">JSON Representation</span></span>
<span data-ttu-id="e901b-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e901b-141">Here is a JSON representation of the resource.</span></span>
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





