---
title: SafeSearchFilterType Enum-Typ
description: Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 477f0b52342ca1b27d844a5f03aedd806cdd8b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875831"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="b3197-103">SafeSearchFilterType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b3197-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="b3197-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b3197-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3197-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3197-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3197-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b3197-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3197-107">Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="b3197-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="b3197-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b3197-108">Members</span></span>
|<span data-ttu-id="b3197-109">Element</span><span class="sxs-lookup"><span data-stu-id="b3197-109">Member</span></span>|<span data-ttu-id="b3197-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b3197-110">Value</span></span>|<span data-ttu-id="b3197-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3197-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3197-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="b3197-112">userDefined</span></span>|<span data-ttu-id="b3197-113">0</span><span class="sxs-lookup"><span data-stu-id="b3197-113">0</span></span>|<span data-ttu-id="b3197-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="b3197-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b3197-115">Strict</span><span class="sxs-lookup"><span data-stu-id="b3197-115">strict</span></span>|<span data-ttu-id="b3197-116">1</span><span class="sxs-lookup"><span data-stu-id="b3197-116">1</span></span>|<span data-ttu-id="b3197-117">Strict, höchsten Filtern anhand der Versender nicht jugendfreier Inhalte.</span><span class="sxs-lookup"><span data-stu-id="b3197-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="b3197-118">Moderater</span><span class="sxs-lookup"><span data-stu-id="b3197-118">moderate</span></span>|<span data-ttu-id="b3197-119">2</span><span class="sxs-lookup"><span data-stu-id="b3197-119">2</span></span>|<span data-ttu-id="b3197-120">Moderater Filtern anhand der Versender nicht jugendfreier Inhalte (gültige Suchergebnisse werden nicht gefiltert).</span><span class="sxs-lookup"><span data-stu-id="b3197-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





