---
title: deviceCategory-Ressourcentyp
description: Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden. Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.
author: tfitzmac
ms.openlocfilehash: 9e40f656a7ce4d511cdb4c597c2419e8cf886c12
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353613"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="c9fea-104">deviceCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c9fea-104">deviceCategory resource type</span></span>

> <span data-ttu-id="c9fea-105">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9fea-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9fea-106">Gerätekategorien bieten eine Möglichkeit zum Organisieren Ihrer Geräte.</span><span class="sxs-lookup"><span data-stu-id="c9fea-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="c9fea-107">Mithilfe von Gerätekategorien können Unternehmensadministratoren eigene Kategorien definieren, die für ihr Unternehmen sinnvoll sind.</span><span class="sxs-lookup"><span data-stu-id="c9fea-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="c9fea-108">Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="c9fea-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="c9fea-109">Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.</span><span class="sxs-lookup"><span data-stu-id="c9fea-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="c9fea-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="c9fea-110">Methods</span></span>
|<span data-ttu-id="c9fea-111">Methode</span><span class="sxs-lookup"><span data-stu-id="c9fea-111">Method</span></span>|<span data-ttu-id="c9fea-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c9fea-112">Return Type</span></span>|<span data-ttu-id="c9fea-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9fea-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9fea-114">[Liste DeviceCategories](../api/intune-shared-devicecategory-list.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c9fea-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="c9fea-115">Auflisten von Eigenschaften und Beziehungen der [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="c9fea-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="c9fea-116">deviceCategory abrufen</span><span class="sxs-lookup"><span data-stu-id="c9fea-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="c9fea-117">Lesen von Eigenschaften und Beziehungen des [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9fea-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="c9fea-118">deviceCategory erstellen</span><span class="sxs-lookup"><span data-stu-id="c9fea-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="c9fea-119">Erstellen eines neuen [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c9fea-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="c9fea-120">[DeviceCategory löschen](../api/intune-shared-devicecategory-delete.md).</span><span class="sxs-lookup"><span data-stu-id="c9fea-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="c9fea-121">deviceCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c9fea-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="c9fea-122">Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts</span><span class="sxs-lookup"><span data-stu-id="c9fea-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c9fea-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9fea-123">Properties</span></span>
|<span data-ttu-id="c9fea-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9fea-124">Property</span></span>|<span data-ttu-id="c9fea-125">Typ</span><span class="sxs-lookup"><span data-stu-id="c9fea-125">Type</span></span>|<span data-ttu-id="c9fea-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9fea-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9fea-127">id</span><span class="sxs-lookup"><span data-stu-id="c9fea-127">id</span></span>|<span data-ttu-id="c9fea-128">String</span><span class="sxs-lookup"><span data-stu-id="c9fea-128">String</span></span>|<span data-ttu-id="c9fea-129">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="c9fea-129">Unique identifier for the device category.</span></span> <span data-ttu-id="c9fea-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c9fea-130">Read-only.</span></span>|
|<span data-ttu-id="c9fea-131">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="c9fea-131">**Onboarding**</span></span>|
|<span data-ttu-id="c9fea-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c9fea-132">displayName</span></span>|<span data-ttu-id="c9fea-133">String</span><span class="sxs-lookup"><span data-stu-id="c9fea-133">String</span></span>|<span data-ttu-id="c9fea-134">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="c9fea-134">Display name for the device category.</span></span>|
|<span data-ttu-id="c9fea-135">description</span><span class="sxs-lookup"><span data-stu-id="c9fea-135">description</span></span>|<span data-ttu-id="c9fea-136">String</span><span class="sxs-lookup"><span data-stu-id="c9fea-136">String</span></span>|<span data-ttu-id="c9fea-137">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="c9fea-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9fea-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c9fea-138">Relationships</span></span>
<span data-ttu-id="c9fea-139">Keine</span><span class="sxs-lookup"><span data-stu-id="c9fea-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9fea-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9fea-140">JSON Representation</span></span>
<span data-ttu-id="c9fea-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c9fea-141">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



