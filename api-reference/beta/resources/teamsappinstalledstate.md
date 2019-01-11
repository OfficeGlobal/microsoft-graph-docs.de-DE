---
title: Mitglieder
description: Wird den aktuelle Installationsstatus von einer TeamsApp beschrieben.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 4e453a28b0c3ebc2957cf7e1a92a846e8e4758e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847572"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="23eec-103">TeamsAppInstalledState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="23eec-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="23eec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23eec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23eec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23eec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23eec-106">Wird den aktuelle Installationsstatus von einer [TeamsApp](teamsapp.md)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="23eec-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="23eec-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="23eec-107">Members</span></span>

| <span data-ttu-id="23eec-108">Element</span><span class="sxs-lookup"><span data-stu-id="23eec-108">Member</span></span> | <span data-ttu-id="23eec-109">Wert</span><span class="sxs-lookup"><span data-stu-id="23eec-109">Value</span></span>| <span data-ttu-id="23eec-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23eec-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="23eec-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="23eec-111">notInstalled</span></span>|<span data-ttu-id="23eec-112">0</span><span class="sxs-lookup"><span data-stu-id="23eec-112">0</span></span>|<span data-ttu-id="23eec-113">App wird an das Team nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="23eec-113">App is not installed to team.</span></span>|
|<span data-ttu-id="23eec-114">installiert</span><span class="sxs-lookup"><span data-stu-id="23eec-114">installed</span></span>|<span data-ttu-id="23eec-115">1</span><span class="sxs-lookup"><span data-stu-id="23eec-115">1</span></span>|<span data-ttu-id="23eec-116">App wird normalerweise installiert.</span><span class="sxs-lookup"><span data-stu-id="23eec-116">App is installed normally.</span></span>|
|<span data-ttu-id="23eec-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="23eec-117">installedAndHidden</span></span>|<span data-ttu-id="23eec-118">2</span><span class="sxs-lookup"><span data-stu-id="23eec-118">2</span></span>|<span data-ttu-id="23eec-119">App wird installiert, jedoch ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="23eec-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="23eec-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="23eec-120">installedAndPermanent</span></span>|<span data-ttu-id="23eec-121">3</span><span class="sxs-lookup"><span data-stu-id="23eec-121">3</span></span>|<span data-ttu-id="23eec-122">App wird dauerhaft installiert und kann nicht entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="23eec-122">App is permanently installed and may not be removed.</span></span>|
