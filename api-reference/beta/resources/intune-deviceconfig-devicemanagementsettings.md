---
title: deviceManagementSettings-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4f676eed1acbf6711f526e612bd6c073b749607d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417665"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="a8fc4-103">deviceManagementSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a8fc4-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="a8fc4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8fc4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8fc4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8fc4-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a8fc4-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a8fc4-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8fc4-108">Properties</span></span>
|<span data-ttu-id="a8fc4-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8fc4-109">Property</span></span>|<span data-ttu-id="a8fc4-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a8fc4-110">Type</span></span>|<span data-ttu-id="a8fc4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8fc4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8fc4-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="a8fc4-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="a8fc4-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a8fc4-113">Int32</span></span>|<span data-ttu-id="a8fc4-114">Die Anzahl von Tagen, die ein Gerät ohne Einchecken konform bleiben kann.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="a8fc4-115">Gültige Werte: 0 bis 120</span><span class="sxs-lookup"><span data-stu-id="a8fc4-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="a8fc4-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="a8fc4-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="a8fc4-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8fc4-117">Boolean</span></span>|<span data-ttu-id="a8fc4-118">Gibt an, ob das Feature für eine geplante Aktion für die Regel aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="a8fc4-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="a8fc4-119">secureByDefault</span></span>|<span data-ttu-id="a8fc4-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8fc4-120">Boolean</span></span>|<span data-ttu-id="a8fc4-121">Ist dies auf „true“ gesetzt, sollte das Gerät als nicht konform gelten, wenn keine Konformitätsrichtlinie verfolgt wird.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="a8fc4-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="a8fc4-122">enhancedJailBreak</span></span>|<span data-ttu-id="a8fc4-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8fc4-123">Boolean</span></span>|<span data-ttu-id="a8fc4-124">Ist Feature aktiviert ist oder nicht erweiterten Jailbreak Erkennung.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="a8fc4-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="a8fc4-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="a8fc4-126">Int32</span><span class="sxs-lookup"><span data-stu-id="a8fc4-126">Int32</span></span>|<span data-ttu-id="a8fc4-127">Wenn das Gerät nicht prüft für die angegebene Anzahl von Tagen, möglicherweise die Mandantendaten entfernt, und das Gerät werden nicht in die Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="a8fc4-128">Gültige Werte 30 bis 270</span><span class="sxs-lookup"><span data-stu-id="a8fc4-128">Valid values 30 to 270</span></span>|
|<span data-ttu-id="a8fc4-129">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="a8fc4-129">derivedCredentialProvider</span></span>|[<span data-ttu-id="a8fc4-130">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="a8fc4-130">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="a8fc4-131">Der abgeleitete Anmeldeinformationsanbieter für dieses Konto verwenden.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-131">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="a8fc4-132">Mögliche Werte sind: `notConfigured`, `entrustDataCard`, `purebred`, `xTec` und `intercede`.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-132">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="a8fc4-133">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="a8fc4-133">derivedCredentialUrl</span></span>|<span data-ttu-id="a8fc4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8fc4-134">String</span></span>|<span data-ttu-id="a8fc4-135">Der Anmeldeinformationsanbieter abgeleitete Self-service-URI.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-135">The Derived Credential Provider self-service URI.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8fc4-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a8fc4-136">Relationships</span></span>
<span data-ttu-id="a8fc4-137">Keine</span><span class="sxs-lookup"><span data-stu-id="a8fc4-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8fc4-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a8fc4-138">JSON Representation</span></span>
<span data-ttu-id="a8fc4-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8fc4-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String"
}
```




