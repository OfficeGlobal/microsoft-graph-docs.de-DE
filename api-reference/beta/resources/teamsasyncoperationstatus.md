---
title: TeamsAsyncOperationStatus Enum-Typ
description: Wird den aktuellen Status der ein TeamsAsyncOperation beschrieben.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e136d043cf58480d93888374558a1be06ca9053d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914819"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="9b4b5-103">TeamsAsyncOperationStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="9b4b5-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="9b4b5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9b4b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b4b5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b4b5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b4b5-106">Wird den aktuellen Status der ein [TeamsAsyncOperation](teamsasyncoperation.md)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="9b4b5-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="9b4b5-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="9b4b5-107">Members</span></span>

| <span data-ttu-id="9b4b5-108">Element</span><span class="sxs-lookup"><span data-stu-id="9b4b5-108">Member</span></span> | <span data-ttu-id="9b4b5-109">Wert</span><span class="sxs-lookup"><span data-stu-id="9b4b5-109">Value</span></span>| <span data-ttu-id="9b4b5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b4b5-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9b4b5-111">Ungültig</span><span class="sxs-lookup"><span data-stu-id="9b4b5-111">invalid</span></span>|<span data-ttu-id="9b4b5-112">0</span><span class="sxs-lookup"><span data-stu-id="9b4b5-112">0</span></span>|<span data-ttu-id="9b4b5-113">Ungültiger Wert.</span><span class="sxs-lookup"><span data-stu-id="9b4b5-113">Invalid value.</span></span>|
|<span data-ttu-id="9b4b5-114">nicht gestartet</span><span class="sxs-lookup"><span data-stu-id="9b4b5-114">notStarted</span></span>|<span data-ttu-id="9b4b5-115">1</span><span class="sxs-lookup"><span data-stu-id="9b4b5-115">1</span></span>|<span data-ttu-id="9b4b5-116">Der Vorgang wurde nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="9b4b5-116">The operation has not started.</span></span>|
|<span data-ttu-id="9b4b5-117">in Bearbeitung</span><span class="sxs-lookup"><span data-stu-id="9b4b5-117">inProgress</span></span>|<span data-ttu-id="9b4b5-118">2</span><span class="sxs-lookup"><span data-stu-id="9b4b5-118">2</span></span>|<span data-ttu-id="9b4b5-119">Der Vorgang wird ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9b4b5-119">The operation is running.</span></span>|
|<span data-ttu-id="9b4b5-120">succeeded</span><span class="sxs-lookup"><span data-stu-id="9b4b5-120">succeeded</span></span>|<span data-ttu-id="9b4b5-121">3</span><span class="sxs-lookup"><span data-stu-id="9b4b5-121">3</span></span>|<span data-ttu-id="9b4b5-122">Der Vorgang erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="9b4b5-122">The operation succeeded.</span></span>|
|<span data-ttu-id="9b4b5-123">failed</span><span class="sxs-lookup"><span data-stu-id="9b4b5-123">failed</span></span>|<span data-ttu-id="9b4b5-124">4</span><span class="sxs-lookup"><span data-stu-id="9b4b5-124">4</span></span>|<span data-ttu-id="9b4b5-125">Dieser Vorgang ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="9b4b5-125">The operation failed.</span></span>|
