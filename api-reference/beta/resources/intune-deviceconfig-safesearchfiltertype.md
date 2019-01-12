---
title: SafeSearchFilterType Enum-Typ
description: Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 49252525b3c6bcab6fd79a1ed7c27b3004665fe8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944796"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="57724-103">SafeSearchFilterType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="57724-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="57724-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="57724-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57724-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="57724-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57724-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="57724-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57724-107">Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="57724-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="57724-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="57724-108">Members</span></span>
|<span data-ttu-id="57724-109">Element</span><span class="sxs-lookup"><span data-stu-id="57724-109">Member</span></span>|<span data-ttu-id="57724-110">Wert</span><span class="sxs-lookup"><span data-stu-id="57724-110">Value</span></span>|<span data-ttu-id="57724-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57724-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57724-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="57724-112">userDefined</span></span>|<span data-ttu-id="57724-113">0</span><span class="sxs-lookup"><span data-stu-id="57724-113">0</span></span>|<span data-ttu-id="57724-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="57724-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="57724-115">Strict</span><span class="sxs-lookup"><span data-stu-id="57724-115">strict</span></span>|<span data-ttu-id="57724-116">1</span><span class="sxs-lookup"><span data-stu-id="57724-116">1</span></span>|<span data-ttu-id="57724-117">Strict, höchsten Filtern anhand der Versender nicht jugendfreier Inhalte.</span><span class="sxs-lookup"><span data-stu-id="57724-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="57724-118">Moderater</span><span class="sxs-lookup"><span data-stu-id="57724-118">moderate</span></span>|<span data-ttu-id="57724-119">2</span><span class="sxs-lookup"><span data-stu-id="57724-119">2</span></span>|<span data-ttu-id="57724-120">Moderater Filtern anhand der Versender nicht jugendfreier Inhalte (gültige Suchergebnisse werden nicht gefiltert).</span><span class="sxs-lookup"><span data-stu-id="57724-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





