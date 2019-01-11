---
title: deviceCategory-Ressourcentyp
description: Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden. Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b61927b5d4c6e8c85ba454d241a0d61a20185579
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888822"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="c2c26-104">deviceCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c2c26-104">deviceCategory resource type</span></span>

> <span data-ttu-id="c2c26-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c2c26-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2c26-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c2c26-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2c26-107">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c2c26-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2c26-108">Gerätekategorien bieten eine Möglichkeit, Ihre Geräte zu organisieren.</span><span class="sxs-lookup"><span data-stu-id="c2c26-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="c2c26-109">Verwenden von Gerätekategorien, können Administratoren im Unternehmen eindeutige Kategorien definieren, die das Unternehmen sinnvoll.</span><span class="sxs-lookup"><span data-stu-id="c2c26-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="c2c26-110">Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="c2c26-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="c2c26-111">Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.</span><span class="sxs-lookup"><span data-stu-id="c2c26-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="c2c26-112">Methoden</span><span class="sxs-lookup"><span data-stu-id="c2c26-112">Methods</span></span>
|<span data-ttu-id="c2c26-113">Methode</span><span class="sxs-lookup"><span data-stu-id="c2c26-113">Method</span></span>|<span data-ttu-id="c2c26-114">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c2c26-114">Return Type</span></span>|<span data-ttu-id="c2c26-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2c26-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c2c26-116">deviceCategories auflisten</span><span class="sxs-lookup"><span data-stu-id="c2c26-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="c2c26-117">[deviceCategory](../resources/intune-shared-devicecategory.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c2c26-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="c2c26-118">Auflisten von Eigenschaften und Beziehungen der [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="c2c26-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="c2c26-119">deviceCategory abrufen</span><span class="sxs-lookup"><span data-stu-id="c2c26-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="c2c26-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="c2c26-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="c2c26-121">Lesen von Eigenschaften und Beziehungen des [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c2c26-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="c2c26-122">deviceCategory erstellen</span><span class="sxs-lookup"><span data-stu-id="c2c26-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="c2c26-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="c2c26-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="c2c26-124">Erstellen eines neuen [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c2c26-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="c2c26-125">deviceCategory löschen</span><span class="sxs-lookup"><span data-stu-id="c2c26-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="c2c26-126">Keine</span><span class="sxs-lookup"><span data-stu-id="c2c26-126">None</span></span>|<span data-ttu-id="c2c26-127">Löscht ein [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="c2c26-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="c2c26-128">deviceCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c2c26-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="c2c26-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="c2c26-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="c2c26-130">Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune-shared-devicecategory.md)-Objekts</span><span class="sxs-lookup"><span data-stu-id="c2c26-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2c26-131">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c2c26-131">Properties</span></span>
|<span data-ttu-id="c2c26-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c2c26-132">Property</span></span>|<span data-ttu-id="c2c26-133">Typ</span><span class="sxs-lookup"><span data-stu-id="c2c26-133">Type</span></span>|<span data-ttu-id="c2c26-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2c26-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2c26-135">id</span><span class="sxs-lookup"><span data-stu-id="c2c26-135">id</span></span>|<span data-ttu-id="c2c26-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2c26-136">String</span></span>|<span data-ttu-id="c2c26-137">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="c2c26-137">Unique identifier for the device category.</span></span> <span data-ttu-id="c2c26-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c2c26-138">Read-only.</span></span>|
|<span data-ttu-id="c2c26-139">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="c2c26-139">**Onboarding**</span></span>|
|<span data-ttu-id="c2c26-140">displayName</span><span class="sxs-lookup"><span data-stu-id="c2c26-140">displayName</span></span>|<span data-ttu-id="c2c26-141">String</span><span class="sxs-lookup"><span data-stu-id="c2c26-141">String</span></span>|<span data-ttu-id="c2c26-142">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="c2c26-142">Display name for the device category.</span></span>|
|<span data-ttu-id="c2c26-143">description</span><span class="sxs-lookup"><span data-stu-id="c2c26-143">description</span></span>|<span data-ttu-id="c2c26-144">String</span><span class="sxs-lookup"><span data-stu-id="c2c26-144">String</span></span>|<span data-ttu-id="c2c26-145">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="c2c26-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2c26-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c2c26-146">Relationships</span></span>
<span data-ttu-id="c2c26-147">Keine</span><span class="sxs-lookup"><span data-stu-id="c2c26-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2c26-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c2c26-148">JSON Representation</span></span>
<span data-ttu-id="c2c26-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c2c26-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



