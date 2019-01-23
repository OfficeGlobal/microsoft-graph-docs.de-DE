---
title: DefenderPotentiallyUnwantedAppAction Enum-Typ
description: Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2ace0cc29ad284cde63b7e4934fb8cb395f27bbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422754"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="6ce6f-103">DefenderPotentiallyUnwantedAppAction Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="6ce6f-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="6ce6f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6ce6f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ce6f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ce6f-107">Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).</span><span class="sxs-lookup"><span data-stu-id="6ce6f-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="6ce6f-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="6ce6f-108">Members</span></span>
|<span data-ttu-id="6ce6f-109">Member</span><span class="sxs-lookup"><span data-stu-id="6ce6f-109">Member</span></span>|<span data-ttu-id="6ce6f-110">Wert</span><span class="sxs-lookup"><span data-stu-id="6ce6f-110">Value</span></span>|<span data-ttu-id="6ce6f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ce6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce6f-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="6ce6f-112">deviceDefault</span></span>|<span data-ttu-id="6ce6f-113">0</span><span class="sxs-lookup"><span data-stu-id="6ce6f-113">0</span></span>|<span data-ttu-id="6ce6f-114">PUA Schutz ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-114">PUA Protection is off.</span></span> <span data-ttu-id="6ce6f-115">Defender bietet keinen Schutz vor unerwünschten Applications.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="6ce6f-116">Blockieren</span><span class="sxs-lookup"><span data-stu-id="6ce6f-116">block</span></span>|<span data-ttu-id="6ce6f-117">1</span><span class="sxs-lookup"><span data-stu-id="6ce6f-117">1</span></span>|<span data-ttu-id="6ce6f-118">PUA Schutz ist auf.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-118">PUA Protection is on.</span></span> <span data-ttu-id="6ce6f-119">Erkannte Elemente werden blockiert.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-119">Detected items are blocked.</span></span> <span data-ttu-id="6ce6f-120">Sie werden im Verlauf zusammen mit anderen Bedrohungen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="6ce6f-121">Audit</span><span class="sxs-lookup"><span data-stu-id="6ce6f-121">audit</span></span>|<span data-ttu-id="6ce6f-122">2</span><span class="sxs-lookup"><span data-stu-id="6ce6f-122">2</span></span>|<span data-ttu-id="6ce6f-123">Überwachungsmodus aktiviert.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-123">Audit mode.</span></span> <span data-ttu-id="6ce6f-124">Defender unerwünschte Applications erkennen, aber keine Aktionen.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="6ce6f-125">Sie können Informationen zu Anwendungen, dass Defender gegen benutzt haben würde durch Suchen des Ereignisse, die in den Ereignisdetails Viewer von Defender erstellt ansehen.</span><span class="sxs-lookup"><span data-stu-id="6ce6f-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|




