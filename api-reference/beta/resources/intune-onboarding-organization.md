---
title: organization-Ressourcentyp
description: Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
author: tfitzmac
ms.openlocfilehash: 447ad5bb87c3c5783ba9097097fbc08281442a0b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323429"
---
# <a name="organization-resource-type"></a><span data-ttu-id="7089a-103">organization-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7089a-103">organization resource type</span></span>

> <span data-ttu-id="7089a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7089a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7089a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7089a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7089a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7089a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7089a-107">Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="7089a-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="7089a-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="7089a-108">Methods</span></span>
|<span data-ttu-id="7089a-109">Methode</span><span class="sxs-lookup"><span data-stu-id="7089a-109">Method</span></span>|<span data-ttu-id="7089a-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7089a-110">Return Type</span></span>|<span data-ttu-id="7089a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7089a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7089a-112">Organisationen auflisten</span><span class="sxs-lookup"><span data-stu-id="7089a-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="7089a-113">[organization](../resources/intune-onboarding-organization.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="7089a-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="7089a-114">Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune-onboarding-organization.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="7089a-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="7089a-115">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="7089a-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="7089a-116">organization</span><span class="sxs-lookup"><span data-stu-id="7089a-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="7089a-117">Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7089a-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="7089a-118">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7089a-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="7089a-119">organization</span><span class="sxs-lookup"><span data-stu-id="7089a-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="7089a-120">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7089a-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="7089a-121">setMobileDeviceManagementAuthority-Aktion</span><span class="sxs-lookup"><span data-stu-id="7089a-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="7089a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="7089a-122">Int32</span></span>|<span data-ttu-id="7089a-123">Autorität für die Verwaltung mobiler Geräte festlegen</span><span class="sxs-lookup"><span data-stu-id="7089a-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="7089a-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7089a-124">Properties</span></span>
|<span data-ttu-id="7089a-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7089a-125">Property</span></span>|<span data-ttu-id="7089a-126">Typ</span><span class="sxs-lookup"><span data-stu-id="7089a-126">Type</span></span>|<span data-ttu-id="7089a-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7089a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7089a-128">id</span><span class="sxs-lookup"><span data-stu-id="7089a-128">id</span></span>|<span data-ttu-id="7089a-129">String</span><span class="sxs-lookup"><span data-stu-id="7089a-129">String</span></span>|<span data-ttu-id="7089a-130">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="7089a-130">The GUID for the object.</span></span>|
|<span data-ttu-id="7089a-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="7089a-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="7089a-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="7089a-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="7089a-133">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="7089a-133">Mobile device management authority.</span></span> <span data-ttu-id="7089a-134">Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="7089a-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="7089a-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="7089a-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="7089a-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="7089a-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="7089a-137">Connector-Einstellung Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="7089a-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7089a-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7089a-138">Relationships</span></span>
<span data-ttu-id="7089a-139">Keine</span><span class="sxs-lookup"><span data-stu-id="7089a-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7089a-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7089a-140">JSON Representation</span></span>
<span data-ttu-id="7089a-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7089a-141">Here is a JSON representation of the resource.</span></span>
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





