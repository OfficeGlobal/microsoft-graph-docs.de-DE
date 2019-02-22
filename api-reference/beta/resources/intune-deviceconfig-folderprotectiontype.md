---
title: folderProtectionType-Enumerationstyp
description: Mögliche Werte für den Ordnerschutz
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0682f5bfbef65b982762e10a9425a8381d645d7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170336"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="0ee89-103">folderProtectionType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="0ee89-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="0ee89-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ee89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ee89-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0ee89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee89-106">Mögliche Werte für den Ordnerschutz</span><span class="sxs-lookup"><span data-stu-id="0ee89-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="0ee89-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="0ee89-107">Members</span></span>
|<span data-ttu-id="0ee89-108">Element</span><span class="sxs-lookup"><span data-stu-id="0ee89-108">Member</span></span>|<span data-ttu-id="0ee89-109">Wert</span><span class="sxs-lookup"><span data-stu-id="0ee89-109">Value</span></span>|<span data-ttu-id="0ee89-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ee89-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee89-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="0ee89-111">userDefined</span></span>|<span data-ttu-id="0ee89-112">0</span><span class="sxs-lookup"><span data-stu-id="0ee89-112">0</span></span>|<span data-ttu-id="0ee89-113">Geräte-Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="0ee89-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="0ee89-114">Aktivieren</span><span class="sxs-lookup"><span data-stu-id="0ee89-114">enable</span></span>|<span data-ttu-id="0ee89-115">1</span><span class="sxs-lookup"><span data-stu-id="0ee89-115">1</span></span>|<span data-ttu-id="0ee89-116">Blockieren der Funktionalität.</span><span class="sxs-lookup"><span data-stu-id="0ee89-116">Block functionality.</span></span>|
|<span data-ttu-id="0ee89-117">auditMode</span><span class="sxs-lookup"><span data-stu-id="0ee89-117">auditMode</span></span>|<span data-ttu-id="0ee89-118">2</span><span class="sxs-lookup"><span data-stu-id="0ee89-118">2</span></span>|<span data-ttu-id="0ee89-119">Funktionalität zulassen, aber Protokolle generieren.</span><span class="sxs-lookup"><span data-stu-id="0ee89-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="0ee89-120">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="0ee89-120">blockDiskModification</span></span>|<span data-ttu-id="0ee89-121">3</span><span class="sxs-lookup"><span data-stu-id="0ee89-121">3</span></span>|<span data-ttu-id="0ee89-122">Blockieren Sie nicht vertrauenswürdige apps vor dem Schreiben in Datenträgersektoren.</span><span class="sxs-lookup"><span data-stu-id="0ee89-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="0ee89-123">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="0ee89-123">auditDiskModification</span></span>|<span data-ttu-id="0ee89-124">4</span><span class="sxs-lookup"><span data-stu-id="0ee89-124">4</span></span>|<span data-ttu-id="0ee89-125">Generieren von Protokollen, wenn nicht vertrauenswürdige apps in Datenträgersektoren schreiben</span><span class="sxs-lookup"><span data-stu-id="0ee89-125">Generate logs when untrusted apps write to disk sectors.</span></span>|




