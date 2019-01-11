---
title: WindowsPrivacyDataAccessLevel Enum-Typ
description: Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74ab32a703422203fec7a6c9ed1bc035e01949a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888774"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="160eb-103">WindowsPrivacyDataAccessLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="160eb-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="160eb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="160eb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="160eb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="160eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="160eb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="160eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="160eb-107">Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.</span><span class="sxs-lookup"><span data-stu-id="160eb-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="160eb-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="160eb-108">Members</span></span>
|<span data-ttu-id="160eb-109">Element</span><span class="sxs-lookup"><span data-stu-id="160eb-109">Member</span></span>|<span data-ttu-id="160eb-110">Wert</span><span class="sxs-lookup"><span data-stu-id="160eb-110">Value</span></span>|<span data-ttu-id="160eb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="160eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="160eb-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="160eb-112">notConfigured</span></span>|<span data-ttu-id="160eb-113">0</span><span class="sxs-lookup"><span data-stu-id="160eb-113">0</span></span>|<span data-ttu-id="160eb-114">Keine Zugriffsebene angegeben, keine Intents.</span><span class="sxs-lookup"><span data-stu-id="160eb-114">No access level specified, no intents.</span></span> <span data-ttu-id="160eb-115">Gerät kann entweder wie in UserInControl oder ForceAllow Verhalten.</span><span class="sxs-lookup"><span data-stu-id="160eb-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="160eb-116">Es kann die private Daten abhängen wurde Zugriff auf Windows-Versionen und anderen Faktoren.</span><span class="sxs-lookup"><span data-stu-id="160eb-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="160eb-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="160eb-117">forceAllow</span></span>|<span data-ttu-id="160eb-118">1</span><span class="sxs-lookup"><span data-stu-id="160eb-118">1</span></span>|<span data-ttu-id="160eb-119">Apps dürfen die angegebenen private Daten zugreifen.</span><span class="sxs-lookup"><span data-stu-id="160eb-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="160eb-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="160eb-120">forceDeny</span></span>|<span data-ttu-id="160eb-121">2</span><span class="sxs-lookup"><span data-stu-id="160eb-121">2</span></span>|<span data-ttu-id="160eb-122">Apps werden für den angegebenen Datenschutzinformationen Zugriff auf verweigert.</span><span class="sxs-lookup"><span data-stu-id="160eb-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="160eb-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="160eb-123">userInControl</span></span>|<span data-ttu-id="160eb-124">3</span><span class="sxs-lookup"><span data-stu-id="160eb-124">3</span></span>|<span data-ttu-id="160eb-125">Benutzer werden aufgefordert, wenn apps auf angegebenen Datenschutzinformationen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="160eb-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





