---
title: deviceManagementSettings-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8238ec075189a138552cb524a22facd99f4d5401
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164267"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="e3564-103">deviceManagementSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e3564-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="e3564-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3564-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3564-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e3564-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3564-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e3564-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e3564-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3564-107">Properties</span></span>
|<span data-ttu-id="e3564-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3564-108">Property</span></span>|<span data-ttu-id="e3564-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e3564-109">Type</span></span>|<span data-ttu-id="e3564-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3564-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3564-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="e3564-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="e3564-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e3564-112">Int32</span></span>|<span data-ttu-id="e3564-113">Die Anzahl von Tagen, die ein Gerät ohne Einchecken konform bleiben kann.</span><span class="sxs-lookup"><span data-stu-id="e3564-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="e3564-114">Gültige Werte: 0 bis 120</span><span class="sxs-lookup"><span data-stu-id="e3564-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="e3564-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="e3564-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="e3564-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e3564-116">Boolean</span></span>|<span data-ttu-id="e3564-117">Gibt an, ob das Feature für eine geplante Aktion für die Regel aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="e3564-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="e3564-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="e3564-118">secureByDefault</span></span>|<span data-ttu-id="e3564-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3564-119">Boolean</span></span>|<span data-ttu-id="e3564-120">Ist dies auf „true“ gesetzt, sollte das Gerät als nicht konform gelten, wenn keine Konformitätsrichtlinie verfolgt wird.</span><span class="sxs-lookup"><span data-stu-id="e3564-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="e3564-121">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="e3564-121">enhancedJailBreak</span></span>|<span data-ttu-id="e3564-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e3564-122">Boolean</span></span>|<span data-ttu-id="e3564-123">Ist Funktion aktiviert oder nicht für eine verbesserte Jailbreak-Erkennung.</span><span class="sxs-lookup"><span data-stu-id="e3564-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="e3564-124">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="e3564-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="e3564-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e3564-125">Int32</span></span>|<span data-ttu-id="e3564-126">Wenn das Gerät für die angegebene Anzahl von Tagen nicht eincheckt, werden die Unternehmensdaten möglicherweise entfernt, und das Gerät wird nicht verwaltet.</span><span class="sxs-lookup"><span data-stu-id="e3564-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="e3564-127">Gültige Werte 30 bis 270</span><span class="sxs-lookup"><span data-stu-id="e3564-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="e3564-128">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="e3564-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="e3564-129">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="e3564-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="e3564-130">Der abgeleitete Anmeldeinformationsanbieter, der für dieses Konto verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e3564-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="e3564-131">Mögliche Werte: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="e3564-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="e3564-132">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="e3564-132">derivedCredentialUrl</span></span>|<span data-ttu-id="e3564-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3564-133">String</span></span>|<span data-ttu-id="e3564-134">Der Self-Service-URI des abgeleiteten Anmeldeinformationen Anbieters.</span><span class="sxs-lookup"><span data-stu-id="e3564-134">The Derived Credential Provider self-service URI.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3564-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e3564-135">Relationships</span></span>
<span data-ttu-id="e3564-136">Keine</span><span class="sxs-lookup"><span data-stu-id="e3564-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3564-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3564-137">JSON Representation</span></span>
<span data-ttu-id="e3564-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3564-138">Here is a JSON representation of the resource.</span></span>
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




