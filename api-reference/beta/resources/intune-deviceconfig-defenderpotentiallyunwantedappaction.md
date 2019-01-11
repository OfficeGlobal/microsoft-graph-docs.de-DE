---
title: DefenderPotentiallyUnwantedAppAction Enum-Typ
description: Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).
localization_priority: Normal
ms.openlocfilehash: 9b04cd6daeae303910519d0735165171575d8c44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858646"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="6fc5b-103">DefenderPotentiallyUnwantedAppAction Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="6fc5b-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="6fc5b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fc5b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fc5b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fc5b-107">Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).</span><span class="sxs-lookup"><span data-stu-id="6fc5b-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>
## <a name="members"></a><span data-ttu-id="6fc5b-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="6fc5b-108">Members</span></span>
|<span data-ttu-id="6fc5b-109">Element</span><span class="sxs-lookup"><span data-stu-id="6fc5b-109">Member</span></span>|<span data-ttu-id="6fc5b-110">Wert</span><span class="sxs-lookup"><span data-stu-id="6fc5b-110">Value</span></span>|<span data-ttu-id="6fc5b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6fc5b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc5b-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="6fc5b-112">deviceDefault</span></span>|<span data-ttu-id="6fc5b-113">0</span><span class="sxs-lookup"><span data-stu-id="6fc5b-113">0</span></span>|<span data-ttu-id="6fc5b-114">PUA Schutz ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-114">PUA Protection is off.</span></span> <span data-ttu-id="6fc5b-115">Defender bietet keinen Schutz vor unerwünschten Applications.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="6fc5b-116">Blockieren</span><span class="sxs-lookup"><span data-stu-id="6fc5b-116">block</span></span>|<span data-ttu-id="6fc5b-117">1</span><span class="sxs-lookup"><span data-stu-id="6fc5b-117">1</span></span>|<span data-ttu-id="6fc5b-118">PUA Schutz ist auf.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-118">PUA Protection is on.</span></span> <span data-ttu-id="6fc5b-119">Erkannte Elemente werden blockiert.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-119">Detected items are blocked.</span></span> <span data-ttu-id="6fc5b-120">Sie werden im Verlauf zusammen mit anderen Bedrohungen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="6fc5b-121">Audit</span><span class="sxs-lookup"><span data-stu-id="6fc5b-121">audit</span></span>|<span data-ttu-id="6fc5b-122">2</span><span class="sxs-lookup"><span data-stu-id="6fc5b-122">2</span></span>|<span data-ttu-id="6fc5b-123">Überwachungsmodus aktiviert.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-123">Audit mode.</span></span> <span data-ttu-id="6fc5b-124">Defender unerwünschte Applications erkennen, aber keine Aktionen.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="6fc5b-125">Sie können Informationen zu Anwendungen, dass Defender gegen benutzt haben würde durch Suchen des Ereignisse, die in den Ereignisdetails Viewer von Defender erstellt ansehen.</span><span class="sxs-lookup"><span data-stu-id="6fc5b-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





