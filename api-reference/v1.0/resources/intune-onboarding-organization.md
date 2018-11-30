---
title: organization-Ressourcentyp
description: Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.
ms.openlocfilehash: ddc3b47777ea586a0f31c0d1d18aaa5727c828e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018083"
---
# <a name="organization-resource-type"></a><span data-ttu-id="ace16-103">organization-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ace16-103">organization resource type</span></span>

> <span data-ttu-id="ace16-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ace16-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ace16-105">Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="ace16-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="ace16-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="ace16-106">Methods</span></span>
|<span data-ttu-id="ace16-107">Methode</span><span class="sxs-lookup"><span data-stu-id="ace16-107">Method</span></span>|<span data-ttu-id="ace16-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ace16-108">Return Type</span></span>|<span data-ttu-id="ace16-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ace16-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ace16-110">Organisationen auflisten</span><span class="sxs-lookup"><span data-stu-id="ace16-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="ace16-111">[organization](../resources/intune-onboarding-organization.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ace16-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="ace16-112">Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune-onboarding-organization.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="ace16-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="ace16-113">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="ace16-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="ace16-114">organization</span><span class="sxs-lookup"><span data-stu-id="ace16-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="ace16-115">Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ace16-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="ace16-116">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ace16-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="ace16-117">organization</span><span class="sxs-lookup"><span data-stu-id="ace16-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="ace16-118">Aktualisieren der Eigenschaften eines [organization](../resources/intune-onboarding-organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ace16-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="ace16-119">setMobileDeviceManagementAuthority-Aktion</span><span class="sxs-lookup"><span data-stu-id="ace16-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="ace16-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ace16-120">Int32</span></span>|<span data-ttu-id="ace16-121">Autorität für die Verwaltung mobiler Geräte festlegen</span><span class="sxs-lookup"><span data-stu-id="ace16-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="ace16-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ace16-122">Properties</span></span>
|<span data-ttu-id="ace16-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ace16-123">Property</span></span>|<span data-ttu-id="ace16-124">Typ</span><span class="sxs-lookup"><span data-stu-id="ace16-124">Type</span></span>|<span data-ttu-id="ace16-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ace16-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ace16-126">id</span><span class="sxs-lookup"><span data-stu-id="ace16-126">id</span></span>|<span data-ttu-id="ace16-127">String</span><span class="sxs-lookup"><span data-stu-id="ace16-127">String</span></span>|<span data-ttu-id="ace16-128">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="ace16-128">The GUID for the object.</span></span>|
|<span data-ttu-id="ace16-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="ace16-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="ace16-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="ace16-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="ace16-131">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="ace16-131">Mobile device management authority.</span></span> <span data-ttu-id="ace16-132">Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="ace16-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ace16-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ace16-133">Relationships</span></span>
<span data-ttu-id="ace16-134">Keine</span><span class="sxs-lookup"><span data-stu-id="ace16-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ace16-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ace16-135">JSON Representation</span></span>
<span data-ttu-id="ace16-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ace16-136">Here is a JSON representation of the resource.</span></span>
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

