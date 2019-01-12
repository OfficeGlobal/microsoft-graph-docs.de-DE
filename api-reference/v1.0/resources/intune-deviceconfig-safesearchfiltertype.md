---
title: SafeSearchFilterType Enum-Typ
description: Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 788a266cdd0161ce1cfef426a7fcf4d9726e3324
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964613"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="283eb-103">SafeSearchFilterType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="283eb-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="283eb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="283eb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="283eb-105">Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="283eb-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="283eb-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="283eb-106">Members</span></span>
|<span data-ttu-id="283eb-107">Element</span><span class="sxs-lookup"><span data-stu-id="283eb-107">Member</span></span>|<span data-ttu-id="283eb-108">Wert</span><span class="sxs-lookup"><span data-stu-id="283eb-108">Value</span></span>|<span data-ttu-id="283eb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="283eb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="283eb-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="283eb-110">userDefined</span></span>|<span data-ttu-id="283eb-111">0</span><span class="sxs-lookup"><span data-stu-id="283eb-111">0</span></span>|<span data-ttu-id="283eb-112">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="283eb-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="283eb-113">Strict</span><span class="sxs-lookup"><span data-stu-id="283eb-113">strict</span></span>|<span data-ttu-id="283eb-114">1</span><span class="sxs-lookup"><span data-stu-id="283eb-114">1</span></span>|<span data-ttu-id="283eb-115">Strict, höchsten Filtern anhand der Versender nicht jugendfreier Inhalte.</span><span class="sxs-lookup"><span data-stu-id="283eb-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="283eb-116">Moderater</span><span class="sxs-lookup"><span data-stu-id="283eb-116">moderate</span></span>|<span data-ttu-id="283eb-117">2</span><span class="sxs-lookup"><span data-stu-id="283eb-117">2</span></span>|<span data-ttu-id="283eb-118">Moderater Filtern anhand der Versender nicht jugendfreier Inhalte (gültige Suchergebnisse werden nicht gefiltert).</span><span class="sxs-lookup"><span data-stu-id="283eb-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



