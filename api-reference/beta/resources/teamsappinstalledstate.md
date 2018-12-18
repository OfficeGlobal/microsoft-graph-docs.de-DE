---
title: Members
description: Wird den aktuelle Installationsstatus von einer TeamsApp beschrieben.
author: nkramer
ms.openlocfilehash: a73c68298c4cdf65deee68fb3bd707d50bc2475a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316793"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="df4a2-103">TeamsAppInstalledState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="df4a2-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="df4a2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df4a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df4a2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df4a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df4a2-106">Wird den aktuelle Installationsstatus von einer [TeamsApp](teamsapp.md)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="df4a2-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="df4a2-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="df4a2-107">Members</span></span>

| <span data-ttu-id="df4a2-108">Member</span><span class="sxs-lookup"><span data-stu-id="df4a2-108">Member</span></span> | <span data-ttu-id="df4a2-109">Wert</span><span class="sxs-lookup"><span data-stu-id="df4a2-109">Value</span></span>| <span data-ttu-id="df4a2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df4a2-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="df4a2-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="df4a2-111">notInstalled</span></span>|<span data-ttu-id="df4a2-112">0</span><span class="sxs-lookup"><span data-stu-id="df4a2-112">0</span></span>|<span data-ttu-id="df4a2-113">App wird an das Team nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="df4a2-113">App is not installed to team.</span></span>|
|<span data-ttu-id="df4a2-114">installiert</span><span class="sxs-lookup"><span data-stu-id="df4a2-114">installed</span></span>|<span data-ttu-id="df4a2-115">1</span><span class="sxs-lookup"><span data-stu-id="df4a2-115">1</span></span>|<span data-ttu-id="df4a2-116">App wird normalerweise installiert.</span><span class="sxs-lookup"><span data-stu-id="df4a2-116">App is installed normally.</span></span>|
|<span data-ttu-id="df4a2-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="df4a2-117">installedAndHidden</span></span>|<span data-ttu-id="df4a2-118">2</span><span class="sxs-lookup"><span data-stu-id="df4a2-118">2</span></span>|<span data-ttu-id="df4a2-119">App wird installiert, jedoch ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="df4a2-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="df4a2-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="df4a2-120">installedAndPermanent</span></span>|<span data-ttu-id="df4a2-121">3</span><span class="sxs-lookup"><span data-stu-id="df4a2-121">3</span></span>|<span data-ttu-id="df4a2-122">App wird dauerhaft installiert und kann nicht entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="df4a2-122">App is permanently installed and may not be removed.</span></span>|
