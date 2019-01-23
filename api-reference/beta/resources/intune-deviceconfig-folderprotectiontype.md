---
title: FolderProtectionType Enum-Typ
description: Mögliche Werte für Ordnerschutz
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e2abbb719ab93b53ad276f8391d4028c4f8b40b4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405716"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="90974-103">FolderProtectionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="90974-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="90974-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="90974-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90974-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="90974-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90974-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="90974-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90974-107">Mögliche Werte für Ordnerschutz</span><span class="sxs-lookup"><span data-stu-id="90974-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="90974-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="90974-108">Members</span></span>
|<span data-ttu-id="90974-109">Member</span><span class="sxs-lookup"><span data-stu-id="90974-109">Member</span></span>|<span data-ttu-id="90974-110">Wert</span><span class="sxs-lookup"><span data-stu-id="90974-110">Value</span></span>|<span data-ttu-id="90974-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90974-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90974-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="90974-112">userDefined</span></span>|<span data-ttu-id="90974-113">0</span><span class="sxs-lookup"><span data-stu-id="90974-113">0</span></span>|<span data-ttu-id="90974-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="90974-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="90974-115">Aktivieren</span><span class="sxs-lookup"><span data-stu-id="90974-115">enable</span></span>|<span data-ttu-id="90974-116">1</span><span class="sxs-lookup"><span data-stu-id="90974-116">1</span></span>|<span data-ttu-id="90974-117">Blockiert Funktionalität.</span><span class="sxs-lookup"><span data-stu-id="90974-117">Block functionality.</span></span>|
|<span data-ttu-id="90974-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="90974-118">auditMode</span></span>|<span data-ttu-id="90974-119">2</span><span class="sxs-lookup"><span data-stu-id="90974-119">2</span></span>|<span data-ttu-id="90974-120">Ermöglicht die Funktionalität, aber Protokolle zu generieren.</span><span class="sxs-lookup"><span data-stu-id="90974-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="90974-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="90974-121">blockDiskModification</span></span>|<span data-ttu-id="90974-122">3</span><span class="sxs-lookup"><span data-stu-id="90974-122">3</span></span>|<span data-ttu-id="90974-123">Blockieren von nicht vertrauenswürdigen apps auf Bereiche Datenträger schreiben.</span><span class="sxs-lookup"><span data-stu-id="90974-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="90974-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="90974-124">auditDiskModification</span></span>|<span data-ttu-id="90974-125">4</span><span class="sxs-lookup"><span data-stu-id="90974-125">4</span></span>|<span data-ttu-id="90974-126">Generieren Sie Protokolle Schreiben von nicht vertrauenswürdigen apps auf Datenträger Bereiche.</span><span class="sxs-lookup"><span data-stu-id="90974-126">Generate logs when untrusted apps write to disk sectors.</span></span>|




