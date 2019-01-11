---
title: SafeSearchFilterType Enum-Typ
description: Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 28aea918c35bb9d90f514e4a8838f219c212405b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830856"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="6704c-103">SafeSearchFilterType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="6704c-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="6704c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6704c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6704c-105">Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="6704c-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="6704c-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="6704c-106">Members</span></span>
|<span data-ttu-id="6704c-107">Element</span><span class="sxs-lookup"><span data-stu-id="6704c-107">Member</span></span>|<span data-ttu-id="6704c-108">Wert</span><span class="sxs-lookup"><span data-stu-id="6704c-108">Value</span></span>|<span data-ttu-id="6704c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6704c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6704c-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="6704c-110">userDefined</span></span>|<span data-ttu-id="6704c-111">0</span><span class="sxs-lookup"><span data-stu-id="6704c-111">0</span></span>|<span data-ttu-id="6704c-112">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="6704c-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="6704c-113">Strict</span><span class="sxs-lookup"><span data-stu-id="6704c-113">strict</span></span>|<span data-ttu-id="6704c-114">1</span><span class="sxs-lookup"><span data-stu-id="6704c-114">1</span></span>|<span data-ttu-id="6704c-115">Strict, höchsten Filtern anhand der Versender nicht jugendfreier Inhalte.</span><span class="sxs-lookup"><span data-stu-id="6704c-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="6704c-116">Moderater</span><span class="sxs-lookup"><span data-stu-id="6704c-116">moderate</span></span>|<span data-ttu-id="6704c-117">2</span><span class="sxs-lookup"><span data-stu-id="6704c-117">2</span></span>|<span data-ttu-id="6704c-118">Moderater Filtern anhand der Versender nicht jugendfreier Inhalte (gültige Suchergebnisse werden nicht gefiltert).</span><span class="sxs-lookup"><span data-stu-id="6704c-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



