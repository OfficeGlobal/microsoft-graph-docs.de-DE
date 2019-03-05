---
title: safeSearchFilterType-Enumerationstyp
description: Gibt an, welche Ebene der sicheren Suche (Filterung von Erwachseneninhalten) erforderlich ist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c82f80f6081f57a88fcdf26f7639277d72b5e0d8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250586"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="db934-103">safeSearchFilterType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="db934-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="db934-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="db934-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db934-105">Gibt an, welche Ebene der sicheren Suche (Filterung von Erwachseneninhalten) erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="db934-105">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="db934-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="db934-106">Members</span></span>
|<span data-ttu-id="db934-107">Element</span><span class="sxs-lookup"><span data-stu-id="db934-107">Member</span></span>|<span data-ttu-id="db934-108">Wert</span><span class="sxs-lookup"><span data-stu-id="db934-108">Value</span></span>|<span data-ttu-id="db934-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="db934-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db934-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="db934-110">userDefined</span></span>|<span data-ttu-id="db934-111">0</span><span class="sxs-lookup"><span data-stu-id="db934-111">0</span></span>|<span data-ttu-id="db934-112">Benutzerdefiniert, Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="db934-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="db934-113">Strict</span><span class="sxs-lookup"><span data-stu-id="db934-113">strict</span></span>|<span data-ttu-id="db934-114">1</span><span class="sxs-lookup"><span data-stu-id="db934-114">1</span></span>|<span data-ttu-id="db934-115">Strenge, höchste Filterung bei Erwachseneninhalten.</span><span class="sxs-lookup"><span data-stu-id="db934-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="db934-116">Moderate</span><span class="sxs-lookup"><span data-stu-id="db934-116">moderate</span></span>|<span data-ttu-id="db934-117">2</span><span class="sxs-lookup"><span data-stu-id="db934-117">2</span></span>|<span data-ttu-id="db934-118">Moderate Filterung mit Adult-Inhalten (gültige Suchergebnisse werden nicht gefiltert).</span><span class="sxs-lookup"><span data-stu-id="db934-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



