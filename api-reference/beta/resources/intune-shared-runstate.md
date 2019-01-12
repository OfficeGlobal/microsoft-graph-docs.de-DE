---
title: RunState Enum-Typ
description: Gibt den Typ des Ausführungsstatus des Skripts Management Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c2178d492b7c341ffc8f5b7af85c78f46bd3f733
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956031"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="f7ac7-103">RunState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="f7ac7-103">runState enum type</span></span>

> <span data-ttu-id="f7ac7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7ac7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7ac7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7ac7-107">Gibt den Typ des Ausführungsstatus des Skripts Management Gerät.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-107">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="f7ac7-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="f7ac7-108">Members</span></span>
|<span data-ttu-id="f7ac7-109">Element</span><span class="sxs-lookup"><span data-stu-id="f7ac7-109">Member</span></span>|<span data-ttu-id="f7ac7-110">Wert</span><span class="sxs-lookup"><span data-stu-id="f7ac7-110">Value</span></span>|<span data-ttu-id="f7ac7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7ac7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7ac7-112">unknown</span><span class="sxs-lookup"><span data-stu-id="f7ac7-112">unknown</span></span>|<span data-ttu-id="f7ac7-113">0</span><span class="sxs-lookup"><span data-stu-id="f7ac7-113">0</span></span>|<span data-ttu-id="f7ac7-114">Unbekanntes Ergebnis.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-114">Unknown result.</span></span>|
|<span data-ttu-id="f7ac7-115">Erfolgreich</span><span class="sxs-lookup"><span data-stu-id="f7ac7-115">success</span></span>|<span data-ttu-id="f7ac7-116">1</span><span class="sxs-lookup"><span data-stu-id="f7ac7-116">1</span></span>|<span data-ttu-id="f7ac7-117">Skript wird erfolgreich ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-117">Script is run successfully.</span></span>|
|<span data-ttu-id="f7ac7-118">ein Fehler auftritt</span><span class="sxs-lookup"><span data-stu-id="f7ac7-118">fail</span></span>|<span data-ttu-id="f7ac7-119">2</span><span class="sxs-lookup"><span data-stu-id="f7ac7-119">2</span></span>|<span data-ttu-id="f7ac7-120">Skript konnte nicht ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="f7ac7-120">Script failed to run.</span></span>|





