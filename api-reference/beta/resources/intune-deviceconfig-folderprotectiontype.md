---
title: FolderProtectionType Enum-Typ
description: Mögliche Werte für Ordnerschutz
author: tfitzmac
ms.openlocfilehash: 93df62da9bb5d849cba86b52384f45bfe7bd760f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350603"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="92ec0-103">FolderProtectionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="92ec0-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="92ec0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="92ec0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92ec0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92ec0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92ec0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="92ec0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92ec0-107">Mögliche Werte für Ordnerschutz</span><span class="sxs-lookup"><span data-stu-id="92ec0-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="92ec0-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="92ec0-108">Members</span></span>
|<span data-ttu-id="92ec0-109">Member</span><span class="sxs-lookup"><span data-stu-id="92ec0-109">Member</span></span>|<span data-ttu-id="92ec0-110">Wert</span><span class="sxs-lookup"><span data-stu-id="92ec0-110">Value</span></span>|<span data-ttu-id="92ec0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92ec0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92ec0-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="92ec0-112">userDefined</span></span>|<span data-ttu-id="92ec0-113">0</span><span class="sxs-lookup"><span data-stu-id="92ec0-113">0</span></span>|<span data-ttu-id="92ec0-114">Gerät Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="92ec0-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="92ec0-115">Aktivieren</span><span class="sxs-lookup"><span data-stu-id="92ec0-115">enable</span></span>|<span data-ttu-id="92ec0-116">1</span><span class="sxs-lookup"><span data-stu-id="92ec0-116">1</span></span>|<span data-ttu-id="92ec0-117">Blockiert Funktionalität.</span><span class="sxs-lookup"><span data-stu-id="92ec0-117">Block functionality.</span></span>|
|<span data-ttu-id="92ec0-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="92ec0-118">auditMode</span></span>|<span data-ttu-id="92ec0-119">2</span><span class="sxs-lookup"><span data-stu-id="92ec0-119">2</span></span>|<span data-ttu-id="92ec0-120">Ermöglicht die Funktionalität, aber Protokolle zu generieren.</span><span class="sxs-lookup"><span data-stu-id="92ec0-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="92ec0-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="92ec0-121">blockDiskModification</span></span>|<span data-ttu-id="92ec0-122">3</span><span class="sxs-lookup"><span data-stu-id="92ec0-122">3</span></span>|<span data-ttu-id="92ec0-123">Blockieren von nicht vertrauenswürdigen apps auf Bereiche Datenträger schreiben.</span><span class="sxs-lookup"><span data-stu-id="92ec0-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="92ec0-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="92ec0-124">auditDiskModification</span></span>|<span data-ttu-id="92ec0-125">4</span><span class="sxs-lookup"><span data-stu-id="92ec0-125">4</span></span>|<span data-ttu-id="92ec0-126">Generieren Sie Protokolle Schreiben von nicht vertrauenswürdigen apps auf Datenträger Bereiche.</span><span class="sxs-lookup"><span data-stu-id="92ec0-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





