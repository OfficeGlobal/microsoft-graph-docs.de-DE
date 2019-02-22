---
title: defenderPotentiallyUnwantedAppAction-Enumerationstyp
description: Die Aktion des Verteidigers zur Übernahme erkannter potenziell unerwünschter Anwendungen (PUA).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02ac5da63c2787c2b87479a23899c9d2980c54c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173353"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="8fe87-103">defenderPotentiallyUnwantedAppAction-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="8fe87-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="8fe87-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8fe87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fe87-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8fe87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fe87-106">Die Aktion des Verteidigers zur Übernahme erkannter potenziell unerwünschter Anwendungen (PUA).</span><span class="sxs-lookup"><span data-stu-id="8fe87-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="8fe87-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="8fe87-107">Members</span></span>
|<span data-ttu-id="8fe87-108">Element</span><span class="sxs-lookup"><span data-stu-id="8fe87-108">Member</span></span>|<span data-ttu-id="8fe87-109">Wert</span><span class="sxs-lookup"><span data-stu-id="8fe87-109">Value</span></span>|<span data-ttu-id="8fe87-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fe87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fe87-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="8fe87-111">deviceDefault</span></span>|<span data-ttu-id="8fe87-112">0</span><span class="sxs-lookup"><span data-stu-id="8fe87-112">0</span></span>|<span data-ttu-id="8fe87-113">PUA-Schutz ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="8fe87-113">PUA Protection is off.</span></span> <span data-ttu-id="8fe87-114">Defender schützt nicht vor potenziell unerwünschten Anwendungen.</span><span class="sxs-lookup"><span data-stu-id="8fe87-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="8fe87-115">Block</span><span class="sxs-lookup"><span data-stu-id="8fe87-115">block</span></span>|<span data-ttu-id="8fe87-116">1</span><span class="sxs-lookup"><span data-stu-id="8fe87-116">1</span></span>|<span data-ttu-id="8fe87-117">PUA-Schutz ist eingeschaltet.</span><span class="sxs-lookup"><span data-stu-id="8fe87-117">PUA Protection is on.</span></span> <span data-ttu-id="8fe87-118">Erkannte Elemente werden blockiert.</span><span class="sxs-lookup"><span data-stu-id="8fe87-118">Detected items are blocked.</span></span> <span data-ttu-id="8fe87-119">Sie werden im Verlauf zusammen mit anderen Bedrohungen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8fe87-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="8fe87-120">Audit</span><span class="sxs-lookup"><span data-stu-id="8fe87-120">audit</span></span>|<span data-ttu-id="8fe87-121">2</span><span class="sxs-lookup"><span data-stu-id="8fe87-121">2</span></span>|<span data-ttu-id="8fe87-122">Überwachungsmodus.</span><span class="sxs-lookup"><span data-stu-id="8fe87-122">Audit mode.</span></span> <span data-ttu-id="8fe87-123">Defender ermittelt potenziell unerwünschte Anwendungen, aber keine Aktionen.</span><span class="sxs-lookup"><span data-stu-id="8fe87-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="8fe87-124">Sie können Informationen zu Anwendungen, die Defender ergriffen haben, durchsuchen nach von Defender erstellten Ereignissen in der Ereignisanzeige lesen.</span><span class="sxs-lookup"><span data-stu-id="8fe87-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|




