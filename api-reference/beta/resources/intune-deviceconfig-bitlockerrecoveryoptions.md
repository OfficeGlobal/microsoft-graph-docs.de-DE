---
title: Ressourcentyp bitLockerRecoveryOptions
description: BitLocker Wiederherstellungsoptionen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df1a2d0a9be3f4ec52b5fa289d0315bda36e4a59
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398513"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="7adb2-103">Ressourcentyp bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="7adb2-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="7adb2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="7adb2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7adb2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7adb2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7adb2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7adb2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7adb2-107">BitLocker Wiederherstellungsoptionen.</span><span class="sxs-lookup"><span data-stu-id="7adb2-107">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="7adb2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7adb2-108">Properties</span></span>
|<span data-ttu-id="7adb2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7adb2-109">Property</span></span>|<span data-ttu-id="7adb2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7adb2-110">Type</span></span>|<span data-ttu-id="7adb2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7adb2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7adb2-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="7adb2-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="7adb2-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="7adb2-113">Boolean</span></span>|<span data-ttu-id="7adb2-114">Gibt an, ob zertifikatbasierte Datenwiederherstellungsagent blockiert.</span><span class="sxs-lookup"><span data-stu-id="7adb2-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="7adb2-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="7adb2-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="7adb2-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="7adb2-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="7adb2-117">Gibt an, ob Benutzer zugelassen oder erforderlich, um ein Wiederherstellungskennwort 48 Ziffern generieren für feste oder Systemdatenträger.</span><span class="sxs-lookup"><span data-stu-id="7adb2-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="7adb2-118">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="7adb2-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="7adb2-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="7adb2-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="7adb2-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="7adb2-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="7adb2-121">Gibt an, ob Benutzer zugelassen oder erforderlich, um eine 256-Bit-Wiederherstellungsschlüssel generieren für feste oder Systemdatenträger.</span><span class="sxs-lookup"><span data-stu-id="7adb2-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="7adb2-122">Mögliche Werte sind: `blocked`, `required` und `allowed`.</span><span class="sxs-lookup"><span data-stu-id="7adb2-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="7adb2-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="7adb2-123">hideRecoveryOptions</span></span>|<span data-ttu-id="7adb2-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="7adb2-124">Boolean</span></span>|<span data-ttu-id="7adb2-125">Gibt an, ob Wiederherstellungsoptionen BitLocker-Setup-Assistenten enthält die feste zulassen oder Systemdatenträger.</span><span class="sxs-lookup"><span data-stu-id="7adb2-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="7adb2-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="7adb2-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="7adb2-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="7adb2-127">Boolean</span></span>|<span data-ttu-id="7adb2-128">Gibt an, ob BitLocker-Wiederherstellungsinformationen in AD DS speichern können.</span><span class="sxs-lookup"><span data-stu-id="7adb2-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="7adb2-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="7adb2-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="7adb2-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="7adb2-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="7adb2-131">Konfigurieren Sie, welche Teile der BitLocker-Wiederherstellungsinformationen in AD DS gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="7adb2-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="7adb2-132">Mögliche Werte sind: `passwordAndKey` und `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="7adb2-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="7adb2-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="7adb2-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="7adb2-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="7adb2-134">Boolean</span></span>|<span data-ttu-id="7adb2-135">Gibt an, ob BitLocker aktivieren, bis Wiederherstellungsinformationen in AD DS gespeichert wird.</span><span class="sxs-lookup"><span data-stu-id="7adb2-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7adb2-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7adb2-136">Relationships</span></span>
<span data-ttu-id="7adb2-137">Keine</span><span class="sxs-lookup"><span data-stu-id="7adb2-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7adb2-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7adb2-138">JSON Representation</span></span>
<span data-ttu-id="7adb2-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7adb2-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```




