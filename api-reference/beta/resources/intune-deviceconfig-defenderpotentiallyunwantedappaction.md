---
title: DefenderPotentiallyUnwantedAppAction Enum-Typ
description: Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 96a3dd70ae0f56f2d0d5a9d6c4f87846e10bba45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938559"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="69f8d-103">DefenderPotentiallyUnwantedAppAction Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="69f8d-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="69f8d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="69f8d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69f8d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="69f8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69f8d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="69f8d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69f8d-107">Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).</span><span class="sxs-lookup"><span data-stu-id="69f8d-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>
## <a name="members"></a><span data-ttu-id="69f8d-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="69f8d-108">Members</span></span>
|<span data-ttu-id="69f8d-109">Element</span><span class="sxs-lookup"><span data-stu-id="69f8d-109">Member</span></span>|<span data-ttu-id="69f8d-110">Wert</span><span class="sxs-lookup"><span data-stu-id="69f8d-110">Value</span></span>|<span data-ttu-id="69f8d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69f8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69f8d-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="69f8d-112">deviceDefault</span></span>|<span data-ttu-id="69f8d-113">0</span><span class="sxs-lookup"><span data-stu-id="69f8d-113">0</span></span>|<span data-ttu-id="69f8d-114">PUA Schutz ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="69f8d-114">PUA Protection is off.</span></span> <span data-ttu-id="69f8d-115">Defender bietet keinen Schutz vor unerwünschten Applications.</span><span class="sxs-lookup"><span data-stu-id="69f8d-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="69f8d-116">Blockieren</span><span class="sxs-lookup"><span data-stu-id="69f8d-116">block</span></span>|<span data-ttu-id="69f8d-117">1</span><span class="sxs-lookup"><span data-stu-id="69f8d-117">1</span></span>|<span data-ttu-id="69f8d-118">PUA Schutz ist auf.</span><span class="sxs-lookup"><span data-stu-id="69f8d-118">PUA Protection is on.</span></span> <span data-ttu-id="69f8d-119">Erkannte Elemente werden blockiert.</span><span class="sxs-lookup"><span data-stu-id="69f8d-119">Detected items are blocked.</span></span> <span data-ttu-id="69f8d-120">Sie werden im Verlauf zusammen mit anderen Bedrohungen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="69f8d-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="69f8d-121">Audit</span><span class="sxs-lookup"><span data-stu-id="69f8d-121">audit</span></span>|<span data-ttu-id="69f8d-122">2</span><span class="sxs-lookup"><span data-stu-id="69f8d-122">2</span></span>|<span data-ttu-id="69f8d-123">Überwachungsmodus aktiviert.</span><span class="sxs-lookup"><span data-stu-id="69f8d-123">Audit mode.</span></span> <span data-ttu-id="69f8d-124">Defender unerwünschte Applications erkennen, aber keine Aktionen.</span><span class="sxs-lookup"><span data-stu-id="69f8d-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="69f8d-125">Sie können Informationen zu Anwendungen, dass Defender gegen benutzt haben würde durch Suchen des Ereignisse, die in den Ereignisdetails Viewer von Defender erstellt ansehen.</span><span class="sxs-lookup"><span data-stu-id="69f8d-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





