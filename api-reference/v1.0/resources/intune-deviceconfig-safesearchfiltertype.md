---
title: SafeSearchFilterType Enum-Typ
description: Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist
ms.openlocfilehash: cf4f61e1b9e4e9f4fcfd94e6372ce517f3b735e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017812"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="ac2c1-103">SafeSearchFilterType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ac2c1-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="ac2c1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ac2c1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac2c1-105">Gibt an, welche sicheres Suchen (Filterung Versender nicht jugendfreier Inhalte) erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="ac2c1-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="ac2c1-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="ac2c1-106">Members</span></span>
|<span data-ttu-id="ac2c1-107">Element</span><span class="sxs-lookup"><span data-stu-id="ac2c1-107">Member</span></span>|<span data-ttu-id="ac2c1-108">Wert</span><span class="sxs-lookup"><span data-stu-id="ac2c1-108">Value</span></span>|<span data-ttu-id="ac2c1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac2c1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac2c1-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="ac2c1-110">userDefined</span></span>|<span data-ttu-id="ac2c1-111">0</span><span class="sxs-lookup"><span data-stu-id="ac2c1-111">0</span></span>|<span data-ttu-id="ac2c1-112">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="ac2c1-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ac2c1-113">Strict</span><span class="sxs-lookup"><span data-stu-id="ac2c1-113">strict</span></span>|<span data-ttu-id="ac2c1-114">1</span><span class="sxs-lookup"><span data-stu-id="ac2c1-114">1</span></span>|<span data-ttu-id="ac2c1-115">Strict, höchsten Filtern anhand der Versender nicht jugendfreier Inhalte.</span><span class="sxs-lookup"><span data-stu-id="ac2c1-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="ac2c1-116">Moderater</span><span class="sxs-lookup"><span data-stu-id="ac2c1-116">moderate</span></span>|<span data-ttu-id="ac2c1-117">2</span><span class="sxs-lookup"><span data-stu-id="ac2c1-117">2</span></span>|<span data-ttu-id="ac2c1-118">Moderater Filtern anhand der Versender nicht jugendfreier Inhalte (gültige Suchergebnisse werden nicht gefiltert).</span><span class="sxs-lookup"><span data-stu-id="ac2c1-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



