---
title: TeamsAsyncOperationStatus Enum-Typ
description: Wird den aktuellen Status der ein TeamsAsyncOperation beschrieben.
ms.openlocfilehash: f553242ace983651b8d4fda77370de712f9d08b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059097"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="59e95-103">TeamsAsyncOperationStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="59e95-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="59e95-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="59e95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59e95-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="59e95-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59e95-106">Wird den aktuellen Status der ein [TeamsAsyncOperation](teamsasyncoperation.md)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="59e95-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="59e95-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="59e95-107">Members</span></span>

| <span data-ttu-id="59e95-108">Element</span><span class="sxs-lookup"><span data-stu-id="59e95-108">Member</span></span> | <span data-ttu-id="59e95-109">Wert</span><span class="sxs-lookup"><span data-stu-id="59e95-109">Value</span></span>| <span data-ttu-id="59e95-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59e95-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="59e95-111">Ungültig</span><span class="sxs-lookup"><span data-stu-id="59e95-111">invalid</span></span>|<span data-ttu-id="59e95-112">0</span><span class="sxs-lookup"><span data-stu-id="59e95-112">0</span></span>|<span data-ttu-id="59e95-113">Ungültiger Wert.</span><span class="sxs-lookup"><span data-stu-id="59e95-113">Invalid value.</span></span>|
|<span data-ttu-id="59e95-114">nicht gestartet</span><span class="sxs-lookup"><span data-stu-id="59e95-114">notStarted</span></span>|<span data-ttu-id="59e95-115">1</span><span class="sxs-lookup"><span data-stu-id="59e95-115">1</span></span>|<span data-ttu-id="59e95-116">Der Vorgang wurde nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="59e95-116">The operation has not started.</span></span>|
|<span data-ttu-id="59e95-117">in Bearbeitung</span><span class="sxs-lookup"><span data-stu-id="59e95-117">inProgress</span></span>|<span data-ttu-id="59e95-118">2</span><span class="sxs-lookup"><span data-stu-id="59e95-118">2</span></span>|<span data-ttu-id="59e95-119">Der Vorgang wird ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="59e95-119">The operation is running.</span></span>|
|<span data-ttu-id="59e95-120">succeeded</span><span class="sxs-lookup"><span data-stu-id="59e95-120">succeeded</span></span>|<span data-ttu-id="59e95-121">3</span><span class="sxs-lookup"><span data-stu-id="59e95-121">3</span></span>|<span data-ttu-id="59e95-122">Der Vorgang erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="59e95-122">The operation succeeded.</span></span>|
|<span data-ttu-id="59e95-123">failed</span><span class="sxs-lookup"><span data-stu-id="59e95-123">failed</span></span>|<span data-ttu-id="59e95-124">4</span><span class="sxs-lookup"><span data-stu-id="59e95-124">4</span></span>|<span data-ttu-id="59e95-125">Dieser Vorgang ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="59e95-125">The operation failed.</span></span>|