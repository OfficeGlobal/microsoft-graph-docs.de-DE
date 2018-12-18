---
title: organization-Ressourcentyp
description: Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
author: tfitzmac
ms.openlocfilehash: da2d127dc5ba44187d8a3a066f5fe261d3dee859
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322848"
---
# <a name="organization-resource-type"></a><span data-ttu-id="756ee-103">organization-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="756ee-103">organization resource type</span></span>

> <span data-ttu-id="756ee-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="756ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="756ee-105">Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="756ee-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="756ee-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="756ee-106">Methods</span></span>
|<span data-ttu-id="756ee-107">Methode</span><span class="sxs-lookup"><span data-stu-id="756ee-107">Method</span></span>|<span data-ttu-id="756ee-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="756ee-108">Return Type</span></span>|<span data-ttu-id="756ee-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="756ee-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="756ee-110">Organisationen auflisten</span><span class="sxs-lookup"><span data-stu-id="756ee-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="756ee-111">[organization](../resources/intune-onboarding-organization.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="756ee-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="756ee-112">Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune-onboarding-organization.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="756ee-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="756ee-113">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="756ee-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="756ee-114">organization</span><span class="sxs-lookup"><span data-stu-id="756ee-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="756ee-115">Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="756ee-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="756ee-116">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="756ee-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="756ee-117">organization</span><span class="sxs-lookup"><span data-stu-id="756ee-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="756ee-118">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="756ee-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="756ee-119">setMobileDeviceManagementAuthority-Aktion</span><span class="sxs-lookup"><span data-stu-id="756ee-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="756ee-120">Int32</span><span class="sxs-lookup"><span data-stu-id="756ee-120">Int32</span></span>|<span data-ttu-id="756ee-121">Autorität für die Verwaltung mobiler Geräte festlegen</span><span class="sxs-lookup"><span data-stu-id="756ee-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="756ee-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="756ee-122">Properties</span></span>
|<span data-ttu-id="756ee-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="756ee-123">Property</span></span>|<span data-ttu-id="756ee-124">Typ</span><span class="sxs-lookup"><span data-stu-id="756ee-124">Type</span></span>|<span data-ttu-id="756ee-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="756ee-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="756ee-126">id</span><span class="sxs-lookup"><span data-stu-id="756ee-126">id</span></span>|<span data-ttu-id="756ee-127">String</span><span class="sxs-lookup"><span data-stu-id="756ee-127">String</span></span>|<span data-ttu-id="756ee-128">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="756ee-128">The GUID for the object.</span></span>|
|<span data-ttu-id="756ee-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="756ee-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="756ee-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="756ee-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="756ee-131">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="756ee-131">Mobile device management authority.</span></span> <span data-ttu-id="756ee-132">Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="756ee-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="756ee-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="756ee-133">Relationships</span></span>
<span data-ttu-id="756ee-134">Keine</span><span class="sxs-lookup"><span data-stu-id="756ee-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="756ee-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="756ee-135">JSON Representation</span></span>
<span data-ttu-id="756ee-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="756ee-136">Here is a JSON representation of the resource.</span></span>
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

