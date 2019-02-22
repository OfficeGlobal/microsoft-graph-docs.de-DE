---
title: onPremisesConditionalAccessSettings-Ressourcentyp
description: Einzelne Entität, die die Exchange-Einstellungen für lokalen bedingten Zugriff für einen Mandanten darstellt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7463abbf44be7db8d94deac0ae22db8fe378493a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150631"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="328b5-103">onPremisesConditionalAccessSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="328b5-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="328b5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="328b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="328b5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="328b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="328b5-106">Einzelne Entität, die die Exchange-Einstellungen für lokalen bedingten Zugriff für einen Mandanten darstellt.</span><span class="sxs-lookup"><span data-stu-id="328b5-106">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="328b5-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="328b5-107">Methods</span></span>
|<span data-ttu-id="328b5-108">Methode</span><span class="sxs-lookup"><span data-stu-id="328b5-108">Method</span></span>|<span data-ttu-id="328b5-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="328b5-109">Return Type</span></span>|<span data-ttu-id="328b5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="328b5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="328b5-111">onpremisesConditionalAccessSettings abrufen</span><span class="sxs-lookup"><span data-stu-id="328b5-111">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="328b5-112">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="328b5-112">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="328b5-113">Lesen von Eigenschaften und Beziehungen des [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="328b5-113">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="328b5-114">onPremisesConditionalAccessSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="328b5-114">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="328b5-115">onpremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="328b5-115">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="328b5-116">Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="328b5-116">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="328b5-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="328b5-117">Properties</span></span>
|<span data-ttu-id="328b5-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="328b5-118">Property</span></span>|<span data-ttu-id="328b5-119">Typ</span><span class="sxs-lookup"><span data-stu-id="328b5-119">Type</span></span>|<span data-ttu-id="328b5-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="328b5-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="328b5-121">id</span><span class="sxs-lookup"><span data-stu-id="328b5-121">id</span></span>|<span data-ttu-id="328b5-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="328b5-122">String</span></span>|<span data-ttu-id="328b5-123">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="328b5-123">Not yet documented</span></span>|
|<span data-ttu-id="328b5-124">enabled</span><span class="sxs-lookup"><span data-stu-id="328b5-124">enabled</span></span>|<span data-ttu-id="328b5-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="328b5-125">Boolean</span></span>|<span data-ttu-id="328b5-126">Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="328b5-126">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="328b5-127">includedGroups</span><span class="sxs-lookup"><span data-stu-id="328b5-127">includedGroups</span></span>|<span data-ttu-id="328b5-128">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="328b5-128">Guid collection</span></span>|<span data-ttu-id="328b5-129">Benutzergruppen, für die der lokale bedingte Zugriff gilt.</span><span class="sxs-lookup"><span data-stu-id="328b5-129">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="328b5-130">Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.</span><span class="sxs-lookup"><span data-stu-id="328b5-130">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="328b5-131">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="328b5-131">excludedGroups</span></span>|<span data-ttu-id="328b5-132">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="328b5-132">Guid collection</span></span>|<span data-ttu-id="328b5-133">Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="328b5-133">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="328b5-134">Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="328b5-134">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="328b5-135">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="328b5-135">overrideDefaultRule</span></span>|<span data-ttu-id="328b5-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="328b5-136">Boolean</span></span>|<span data-ttu-id="328b5-137">Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="328b5-137">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="328b5-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="328b5-138">Relationships</span></span>
<span data-ttu-id="328b5-139">Keine</span><span class="sxs-lookup"><span data-stu-id="328b5-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="328b5-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="328b5-140">JSON Representation</span></span>
<span data-ttu-id="328b5-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="328b5-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```




