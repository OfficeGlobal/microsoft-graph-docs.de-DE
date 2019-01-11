---
title: onPremisesConditionalAccessSettings-Ressourcentyp
description: Einzelne Entität, die die Exchange-Einstellungen für lokalen bedingten Zugriff für einen Mandanten darstellt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 88d513cc59b9570b355e67fa417a9856519cf551
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875992"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="9e097-103">onPremisesConditionalAccessSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e097-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="9e097-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9e097-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e097-105">Einzelne Entität, die die Exchange-Einstellungen für lokalen bedingten Zugriff für einen Mandanten darstellt.</span><span class="sxs-lookup"><span data-stu-id="9e097-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="9e097-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="9e097-106">Methods</span></span>
|<span data-ttu-id="9e097-107">Methode</span><span class="sxs-lookup"><span data-stu-id="9e097-107">Method</span></span>|<span data-ttu-id="9e097-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9e097-108">Return Type</span></span>|<span data-ttu-id="9e097-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e097-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e097-110">onpremisesConditionalAccessSettings abrufen</span><span class="sxs-lookup"><span data-stu-id="9e097-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="9e097-111">onpremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="9e097-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="9e097-112">Lesen von Eigenschaften und Beziehungen des [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9e097-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="9e097-113">onPremisesConditionalAccessSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9e097-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="9e097-114">onpremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="9e097-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="9e097-115">Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9e097-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e097-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e097-116">Properties</span></span>
|<span data-ttu-id="9e097-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e097-117">Property</span></span>|<span data-ttu-id="9e097-118">Typ</span><span class="sxs-lookup"><span data-stu-id="9e097-118">Type</span></span>|<span data-ttu-id="9e097-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e097-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e097-120">id</span><span class="sxs-lookup"><span data-stu-id="9e097-120">id</span></span>|<span data-ttu-id="9e097-121">String</span><span class="sxs-lookup"><span data-stu-id="9e097-121">String</span></span>|<span data-ttu-id="9e097-122">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9e097-122">Not yet documented</span></span>|
|<span data-ttu-id="9e097-123">enabled</span><span class="sxs-lookup"><span data-stu-id="9e097-123">enabled</span></span>|<span data-ttu-id="9e097-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e097-124">Boolean</span></span>|<span data-ttu-id="9e097-125">Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="9e097-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="9e097-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="9e097-126">includedGroups</span></span>|<span data-ttu-id="9e097-127">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9e097-127">Guid collection</span></span>|<span data-ttu-id="9e097-128">Benutzergruppen, für die der lokale bedingte Zugriff gilt.</span><span class="sxs-lookup"><span data-stu-id="9e097-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="9e097-129">Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.</span><span class="sxs-lookup"><span data-stu-id="9e097-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="9e097-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="9e097-130">excludedGroups</span></span>|<span data-ttu-id="9e097-131">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9e097-131">Guid collection</span></span>|<span data-ttu-id="9e097-132">Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="9e097-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="9e097-133">Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="9e097-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="9e097-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="9e097-134">overrideDefaultRule</span></span>|<span data-ttu-id="9e097-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e097-135">Boolean</span></span>|<span data-ttu-id="9e097-136">Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="9e097-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e097-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9e097-137">Relationships</span></span>
<span data-ttu-id="9e097-138">Keine</span><span class="sxs-lookup"><span data-stu-id="9e097-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e097-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e097-139">JSON Representation</span></span>
<span data-ttu-id="9e097-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e097-140">Here is a JSON representation of the resource.</span></span>
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



