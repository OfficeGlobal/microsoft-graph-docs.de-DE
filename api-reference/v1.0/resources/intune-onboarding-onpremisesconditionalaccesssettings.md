---
title: onPremisesConditionalAccessSettings-Ressourcentyp
description: Einzelne Entität, die die Exchange-Einstellungen für lokalen bedingten Zugriff für einen Mandanten darstellt.
ms.openlocfilehash: 903a3e6a3fafd837fc8c5caf55eb57d23ddd0d2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018082"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="480f8-103">onPremisesConditionalAccessSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="480f8-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="480f8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="480f8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="480f8-105">Einzelne Entität, die die Exchange-Einstellungen für lokalen bedingten Zugriff für einen Mandanten darstellt.</span><span class="sxs-lookup"><span data-stu-id="480f8-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="480f8-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="480f8-106">Methods</span></span>
|<span data-ttu-id="480f8-107">Methode</span><span class="sxs-lookup"><span data-stu-id="480f8-107">Method</span></span>|<span data-ttu-id="480f8-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="480f8-108">Return Type</span></span>|<span data-ttu-id="480f8-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="480f8-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="480f8-110">onpremisesConditionalAccessSettings abrufen</span><span class="sxs-lookup"><span data-stu-id="480f8-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="480f8-111">onpremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="480f8-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="480f8-112">Lesen von Eigenschaften und Beziehungen des [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="480f8-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="480f8-113">onPremisesConditionalAccessSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="480f8-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="480f8-114">onpremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="480f8-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="480f8-115">Aktualisieren der Eigenschaften eines [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="480f8-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="480f8-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="480f8-116">Properties</span></span>
|<span data-ttu-id="480f8-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="480f8-117">Property</span></span>|<span data-ttu-id="480f8-118">Typ</span><span class="sxs-lookup"><span data-stu-id="480f8-118">Type</span></span>|<span data-ttu-id="480f8-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="480f8-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="480f8-120">id</span><span class="sxs-lookup"><span data-stu-id="480f8-120">id</span></span>|<span data-ttu-id="480f8-121">String</span><span class="sxs-lookup"><span data-stu-id="480f8-121">String</span></span>|<span data-ttu-id="480f8-122">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="480f8-122">Not yet documented</span></span>|
|<span data-ttu-id="480f8-123">enabled</span><span class="sxs-lookup"><span data-stu-id="480f8-123">enabled</span></span>|<span data-ttu-id="480f8-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="480f8-124">Boolean</span></span>|<span data-ttu-id="480f8-125">Gibt an, ob lokaler bedingter Zugriff für diese Organisation aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="480f8-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="480f8-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="480f8-126">includedGroups</span></span>|<span data-ttu-id="480f8-127">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="480f8-127">Guid collection</span></span>|<span data-ttu-id="480f8-128">Benutzergruppen, für die der lokale bedingte Zugriff gilt.</span><span class="sxs-lookup"><span data-stu-id="480f8-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="480f8-129">Alle Benutzer in diesen Gruppen müssen verwaltete und für den E-Mail-Zugriff kompatible Mobilgeräte verwenden.</span><span class="sxs-lookup"><span data-stu-id="480f8-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="480f8-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="480f8-130">excludedGroups</span></span>|<span data-ttu-id="480f8-131">GUID-Sammlung</span><span class="sxs-lookup"><span data-stu-id="480f8-131">Guid collection</span></span>|<span data-ttu-id="480f8-132">Benutzergruppen, die vom lokalen bedingten Zugriff ausgenommen werden.</span><span class="sxs-lookup"><span data-stu-id="480f8-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="480f8-133">Alle Benutzer in diesen Gruppen werden von der Richtlinie zu bedingtem Zugriff ausgenommen.</span><span class="sxs-lookup"><span data-stu-id="480f8-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="480f8-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="480f8-134">overrideDefaultRule</span></span>|<span data-ttu-id="480f8-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="480f8-135">Boolean</span></span>|<span data-ttu-id="480f8-136">Überschreibt die Standardzugriffsregel, wenn zugelassen wird, dass einem Gerät Zugriff gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="480f8-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="480f8-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="480f8-137">Relationships</span></span>
<span data-ttu-id="480f8-138">Keine</span><span class="sxs-lookup"><span data-stu-id="480f8-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="480f8-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="480f8-139">JSON Representation</span></span>
<span data-ttu-id="480f8-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="480f8-140">Here is a JSON representation of the resource.</span></span>
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



