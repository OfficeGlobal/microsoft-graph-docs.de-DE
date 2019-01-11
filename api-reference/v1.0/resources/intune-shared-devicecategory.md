---
title: deviceCategory-Ressourcentyp
description: Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden. Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 80f8f1f36198ecfab1021e30cb2f28fa4377852c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810836"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="c742d-104">deviceCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c742d-104">deviceCategory resource type</span></span>

> <span data-ttu-id="c742d-105">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c742d-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c742d-106">Gerätekategorien bieten eine Möglichkeit zum Organisieren Ihrer Geräte.</span><span class="sxs-lookup"><span data-stu-id="c742d-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="c742d-107">Mithilfe von Gerätekategorien können Unternehmensadministratoren eigene Kategorien definieren, die für ihr Unternehmen sinnvoll sind.</span><span class="sxs-lookup"><span data-stu-id="c742d-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="c742d-108">Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="c742d-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="c742d-109">Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.</span><span class="sxs-lookup"><span data-stu-id="c742d-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="c742d-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="c742d-110">Methods</span></span>
|<span data-ttu-id="c742d-111">Methode</span><span class="sxs-lookup"><span data-stu-id="c742d-111">Method</span></span>|<span data-ttu-id="c742d-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c742d-112">Return Type</span></span>|<span data-ttu-id="c742d-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c742d-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c742d-114">[Liste DeviceCategories](../api/intune-shared-devicecategory-list.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c742d-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="c742d-115">Auflisten von Eigenschaften und Beziehungen der [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="c742d-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="c742d-116">deviceCategory abrufen</span><span class="sxs-lookup"><span data-stu-id="c742d-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="c742d-117">Lesen von Eigenschaften und Beziehungen des [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c742d-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="c742d-118">deviceCategory erstellen</span><span class="sxs-lookup"><span data-stu-id="c742d-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="c742d-119">Erstellen eines neuen [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c742d-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="c742d-120">[DeviceCategory löschen](../api/intune-shared-devicecategory-delete.md).</span><span class="sxs-lookup"><span data-stu-id="c742d-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="c742d-121">deviceCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c742d-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="c742d-122">Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts</span><span class="sxs-lookup"><span data-stu-id="c742d-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c742d-123">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c742d-123">Properties</span></span>
|<span data-ttu-id="c742d-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c742d-124">Property</span></span>|<span data-ttu-id="c742d-125">Typ</span><span class="sxs-lookup"><span data-stu-id="c742d-125">Type</span></span>|<span data-ttu-id="c742d-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c742d-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c742d-127">id</span><span class="sxs-lookup"><span data-stu-id="c742d-127">id</span></span>|<span data-ttu-id="c742d-128">String</span><span class="sxs-lookup"><span data-stu-id="c742d-128">String</span></span>|<span data-ttu-id="c742d-129">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="c742d-129">Unique identifier for the device category.</span></span> <span data-ttu-id="c742d-130">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c742d-130">Read-only.</span></span>|
|<span data-ttu-id="c742d-131">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="c742d-131">**Onboarding**</span></span>|
|<span data-ttu-id="c742d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c742d-132">displayName</span></span>|<span data-ttu-id="c742d-133">String</span><span class="sxs-lookup"><span data-stu-id="c742d-133">String</span></span>|<span data-ttu-id="c742d-134">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="c742d-134">Display name for the device category.</span></span>|
|<span data-ttu-id="c742d-135">description</span><span class="sxs-lookup"><span data-stu-id="c742d-135">description</span></span>|<span data-ttu-id="c742d-136">String</span><span class="sxs-lookup"><span data-stu-id="c742d-136">String</span></span>|<span data-ttu-id="c742d-137">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="c742d-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c742d-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c742d-138">Relationships</span></span>
<span data-ttu-id="c742d-139">Keine</span><span class="sxs-lookup"><span data-stu-id="c742d-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c742d-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c742d-140">JSON Representation</span></span>
<span data-ttu-id="c742d-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c742d-141">Here is a JSON representation of the resource.</span></span>
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



