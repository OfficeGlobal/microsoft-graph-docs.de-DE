---
title: TeamsAsyncOperationStatus Enum-Typ
description: Wird den aktuellen Status der ein TeamsAsyncOperation beschrieben.
author: nkramer
ms.openlocfilehash: 49b5b81999714627b1a1acd42df208594123b262
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332004"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="868f4-103">TeamsAsyncOperationStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="868f4-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="868f4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="868f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="868f4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="868f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="868f4-106">Wird den aktuellen Status der ein [TeamsAsyncOperation](teamsasyncoperation.md)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="868f4-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="868f4-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="868f4-107">Members</span></span>

| <span data-ttu-id="868f4-108">Member</span><span class="sxs-lookup"><span data-stu-id="868f4-108">Member</span></span> | <span data-ttu-id="868f4-109">Wert</span><span class="sxs-lookup"><span data-stu-id="868f4-109">Value</span></span>| <span data-ttu-id="868f4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="868f4-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="868f4-111">Ungültig</span><span class="sxs-lookup"><span data-stu-id="868f4-111">invalid</span></span>|<span data-ttu-id="868f4-112">0</span><span class="sxs-lookup"><span data-stu-id="868f4-112">0</span></span>|<span data-ttu-id="868f4-113">Ungültiger Wert.</span><span class="sxs-lookup"><span data-stu-id="868f4-113">Invalid value.</span></span>|
|<span data-ttu-id="868f4-114">nicht gestartet</span><span class="sxs-lookup"><span data-stu-id="868f4-114">notStarted</span></span>|<span data-ttu-id="868f4-115">1</span><span class="sxs-lookup"><span data-stu-id="868f4-115">1</span></span>|<span data-ttu-id="868f4-116">Der Vorgang wurde nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="868f4-116">The operation has not started.</span></span>|
|<span data-ttu-id="868f4-117">in Bearbeitung</span><span class="sxs-lookup"><span data-stu-id="868f4-117">inProgress</span></span>|<span data-ttu-id="868f4-118">2</span><span class="sxs-lookup"><span data-stu-id="868f4-118">2</span></span>|<span data-ttu-id="868f4-119">Der Vorgang wird ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="868f4-119">The operation is running.</span></span>|
|<span data-ttu-id="868f4-120">succeeded</span><span class="sxs-lookup"><span data-stu-id="868f4-120">succeeded</span></span>|<span data-ttu-id="868f4-121">3</span><span class="sxs-lookup"><span data-stu-id="868f4-121">3</span></span>|<span data-ttu-id="868f4-122">Der Vorgang erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="868f4-122">The operation succeeded.</span></span>|
|<span data-ttu-id="868f4-123">failed</span><span class="sxs-lookup"><span data-stu-id="868f4-123">failed</span></span>|<span data-ttu-id="868f4-124">4</span><span class="sxs-lookup"><span data-stu-id="868f4-124">4</span></span>|<span data-ttu-id="868f4-125">Dieser Vorgang ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="868f4-125">The operation failed.</span></span>|