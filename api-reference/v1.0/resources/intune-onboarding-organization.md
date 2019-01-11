---
title: organization-Ressourcentyp
description: Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b87866520e62850f169861f4fac0a9a2454ea3d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814434"
---
# <a name="organization-resource-type"></a><span data-ttu-id="84980-103">organization-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="84980-103">organization resource type</span></span>

> <span data-ttu-id="84980-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="84980-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84980-105">Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="84980-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="84980-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="84980-106">Methods</span></span>
|<span data-ttu-id="84980-107">Methode</span><span class="sxs-lookup"><span data-stu-id="84980-107">Method</span></span>|<span data-ttu-id="84980-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="84980-108">Return Type</span></span>|<span data-ttu-id="84980-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84980-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84980-110">Organisationen auflisten</span><span class="sxs-lookup"><span data-stu-id="84980-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="84980-111">[organization](../resources/intune-onboarding-organization.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="84980-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="84980-112">Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune-onboarding-organization.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="84980-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="84980-113">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="84980-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="84980-114">organization</span><span class="sxs-lookup"><span data-stu-id="84980-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="84980-115">Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="84980-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="84980-116">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="84980-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="84980-117">organization</span><span class="sxs-lookup"><span data-stu-id="84980-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="84980-118">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="84980-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="84980-119">setMobileDeviceManagementAuthority-Aktion</span><span class="sxs-lookup"><span data-stu-id="84980-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="84980-120">Int32</span><span class="sxs-lookup"><span data-stu-id="84980-120">Int32</span></span>|<span data-ttu-id="84980-121">Autorität für die Verwaltung mobiler Geräte festlegen</span><span class="sxs-lookup"><span data-stu-id="84980-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="84980-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="84980-122">Properties</span></span>
|<span data-ttu-id="84980-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="84980-123">Property</span></span>|<span data-ttu-id="84980-124">Typ</span><span class="sxs-lookup"><span data-stu-id="84980-124">Type</span></span>|<span data-ttu-id="84980-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84980-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84980-126">id</span><span class="sxs-lookup"><span data-stu-id="84980-126">id</span></span>|<span data-ttu-id="84980-127">String</span><span class="sxs-lookup"><span data-stu-id="84980-127">String</span></span>|<span data-ttu-id="84980-128">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="84980-128">The GUID for the object.</span></span>|
|<span data-ttu-id="84980-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="84980-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="84980-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="84980-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="84980-131">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="84980-131">Mobile device management authority.</span></span> <span data-ttu-id="84980-132">Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="84980-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84980-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="84980-133">Relationships</span></span>
<span data-ttu-id="84980-134">Keine</span><span class="sxs-lookup"><span data-stu-id="84980-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="84980-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="84980-135">JSON Representation</span></span>
<span data-ttu-id="84980-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="84980-136">Here is a JSON representation of the resource.</span></span>
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
  "mobileDeviceManagementAuthority": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->

