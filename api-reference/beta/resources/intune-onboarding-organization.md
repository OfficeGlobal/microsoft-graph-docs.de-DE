---
title: organization-Ressourcentyp
description: Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b47ec69063998a935640f05d04a17bfc5714c8d8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398233"
---
# <a name="organization-resource-type"></a><span data-ttu-id="0883c-103">organization-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0883c-103">organization resource type</span></span>

> <span data-ttu-id="0883c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0883c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0883c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0883c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0883c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0883c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0883c-107">Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="0883c-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="0883c-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="0883c-108">Methods</span></span>
|<span data-ttu-id="0883c-109">Methode</span><span class="sxs-lookup"><span data-stu-id="0883c-109">Method</span></span>|<span data-ttu-id="0883c-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0883c-110">Return Type</span></span>|<span data-ttu-id="0883c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0883c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0883c-112">Organisationen auflisten</span><span class="sxs-lookup"><span data-stu-id="0883c-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="0883c-113">[organization](../resources/intune-onboarding-organization.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0883c-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="0883c-114">Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune-onboarding-organization.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="0883c-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="0883c-115">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="0883c-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="0883c-116">organization</span><span class="sxs-lookup"><span data-stu-id="0883c-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="0883c-117">Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0883c-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="0883c-118">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0883c-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="0883c-119">organization</span><span class="sxs-lookup"><span data-stu-id="0883c-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="0883c-120">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0883c-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="0883c-121">setMobileDeviceManagementAuthority-Aktion</span><span class="sxs-lookup"><span data-stu-id="0883c-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="0883c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="0883c-122">Int32</span></span>|<span data-ttu-id="0883c-123">Autorität für die Verwaltung mobiler Geräte festlegen</span><span class="sxs-lookup"><span data-stu-id="0883c-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="0883c-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0883c-124">Properties</span></span>
|<span data-ttu-id="0883c-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0883c-125">Property</span></span>|<span data-ttu-id="0883c-126">Typ</span><span class="sxs-lookup"><span data-stu-id="0883c-126">Type</span></span>|<span data-ttu-id="0883c-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0883c-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0883c-128">id</span><span class="sxs-lookup"><span data-stu-id="0883c-128">id</span></span>|<span data-ttu-id="0883c-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0883c-129">String</span></span>|<span data-ttu-id="0883c-130">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="0883c-130">The GUID for the object.</span></span>|
|<span data-ttu-id="0883c-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="0883c-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="0883c-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="0883c-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="0883c-133">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="0883c-133">Mobile device management authority.</span></span> <span data-ttu-id="0883c-134">Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="0883c-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="0883c-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="0883c-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="0883c-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="0883c-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="0883c-137">Connector-Einstellung Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="0883c-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0883c-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0883c-138">Relationships</span></span>
<span data-ttu-id="0883c-139">Keine</span><span class="sxs-lookup"><span data-stu-id="0883c-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0883c-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0883c-140">JSON Representation</span></span>
<span data-ttu-id="0883c-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0883c-141">Here is a JSON representation of the resource.</span></span>
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




