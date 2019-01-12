---
title: Mitglieder
description: Wird den aktuelle Installationsstatus von einer TeamsApp beschrieben.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ca42b56e2c374dbaea1df676e3a84569b192e78c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937173"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="90739-103">TeamsAppInstalledState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="90739-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="90739-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="90739-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90739-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="90739-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90739-106">Wird den aktuelle Installationsstatus von einer [TeamsApp](teamsapp.md)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="90739-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="90739-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="90739-107">Members</span></span>

| <span data-ttu-id="90739-108">Element</span><span class="sxs-lookup"><span data-stu-id="90739-108">Member</span></span> | <span data-ttu-id="90739-109">Wert</span><span class="sxs-lookup"><span data-stu-id="90739-109">Value</span></span>| <span data-ttu-id="90739-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90739-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="90739-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="90739-111">notInstalled</span></span>|<span data-ttu-id="90739-112">0</span><span class="sxs-lookup"><span data-stu-id="90739-112">0</span></span>|<span data-ttu-id="90739-113">App wird an das Team nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="90739-113">App is not installed to team.</span></span>|
|<span data-ttu-id="90739-114">installiert</span><span class="sxs-lookup"><span data-stu-id="90739-114">installed</span></span>|<span data-ttu-id="90739-115">1</span><span class="sxs-lookup"><span data-stu-id="90739-115">1</span></span>|<span data-ttu-id="90739-116">App wird normalerweise installiert.</span><span class="sxs-lookup"><span data-stu-id="90739-116">App is installed normally.</span></span>|
|<span data-ttu-id="90739-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="90739-117">installedAndHidden</span></span>|<span data-ttu-id="90739-118">2</span><span class="sxs-lookup"><span data-stu-id="90739-118">2</span></span>|<span data-ttu-id="90739-119">App wird installiert, jedoch ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="90739-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="90739-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="90739-120">installedAndPermanent</span></span>|<span data-ttu-id="90739-121">3</span><span class="sxs-lookup"><span data-stu-id="90739-121">3</span></span>|<span data-ttu-id="90739-122">App wird dauerhaft installiert und kann nicht entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="90739-122">App is permanently installed and may not be removed.</span></span>|
