---
title: SafeSearchFilterType Enum-Typ
description: Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4493c71b48a0f5ff4b0c48307504087c722393e1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403483"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="943b9-103">SafeSearchFilterType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="943b9-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="943b9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="943b9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="943b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="943b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="943b9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="943b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="943b9-107">Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="943b9-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="943b9-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="943b9-108">Members</span></span>
|<span data-ttu-id="943b9-109">Member</span><span class="sxs-lookup"><span data-stu-id="943b9-109">Member</span></span>|<span data-ttu-id="943b9-110">Wert</span><span class="sxs-lookup"><span data-stu-id="943b9-110">Value</span></span>|<span data-ttu-id="943b9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="943b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="943b9-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="943b9-112">userDefined</span></span>|<span data-ttu-id="943b9-113">0</span><span class="sxs-lookup"><span data-stu-id="943b9-113">0</span></span>|<span data-ttu-id="943b9-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="943b9-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="943b9-115">Strict</span><span class="sxs-lookup"><span data-stu-id="943b9-115">strict</span></span>|<span data-ttu-id="943b9-116">1</span><span class="sxs-lookup"><span data-stu-id="943b9-116">1</span></span>|<span data-ttu-id="943b9-117">Strict, höchsten Filtern anhand der Versender nicht jugendfreier Inhalte.</span><span class="sxs-lookup"><span data-stu-id="943b9-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="943b9-118">Moderater</span><span class="sxs-lookup"><span data-stu-id="943b9-118">moderate</span></span>|<span data-ttu-id="943b9-119">2</span><span class="sxs-lookup"><span data-stu-id="943b9-119">2</span></span>|<span data-ttu-id="943b9-120">Moderater Filtern anhand der Versender nicht jugendfreier Inhalte (gültige Suchergebnisse werden nicht gefiltert).</span><span class="sxs-lookup"><span data-stu-id="943b9-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




