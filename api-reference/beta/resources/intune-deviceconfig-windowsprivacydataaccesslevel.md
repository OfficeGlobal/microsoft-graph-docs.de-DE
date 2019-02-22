---
title: windowsPrivacyDataAccessLevel-Enumerationstyp
description: Bestimmen Sie die Zugriffsebene für bestimmte Windows-Datenschutzkategorien.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2cdf124d3da6bf2c08954365a87ae0a97b05267
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159066"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="4be92-103">windowsPrivacyDataAccessLevel-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="4be92-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="4be92-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4be92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4be92-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4be92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4be92-106">Bestimmen Sie die Zugriffsebene für bestimmte Windows-Datenschutzkategorien.</span><span class="sxs-lookup"><span data-stu-id="4be92-106">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="4be92-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="4be92-107">Members</span></span>
|<span data-ttu-id="4be92-108">Element</span><span class="sxs-lookup"><span data-stu-id="4be92-108">Member</span></span>|<span data-ttu-id="4be92-109">Wert</span><span class="sxs-lookup"><span data-stu-id="4be92-109">Value</span></span>|<span data-ttu-id="4be92-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4be92-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4be92-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4be92-111">notConfigured</span></span>|<span data-ttu-id="4be92-112">0</span><span class="sxs-lookup"><span data-stu-id="4be92-112">0</span></span>|<span data-ttu-id="4be92-113">Keine Zugriffsebene angegeben, keine Absichten.</span><span class="sxs-lookup"><span data-stu-id="4be92-113">No access level specified, no intents.</span></span> <span data-ttu-id="4be92-114">Das Gerät kann sich entweder wie in UserInControl oder in ForceAllow Verhalten.</span><span class="sxs-lookup"><span data-stu-id="4be92-114">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="4be92-115">Es kann davon abhängen, auf welche Daten auf dem Datenschutz zugegriffen wurde, wie Windows-Versionen und andere Faktoren.</span><span class="sxs-lookup"><span data-stu-id="4be92-115">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="4be92-116">forceAllow</span><span class="sxs-lookup"><span data-stu-id="4be92-116">forceAllow</span></span>|<span data-ttu-id="4be92-117">1</span><span class="sxs-lookup"><span data-stu-id="4be92-117">1</span></span>|<span data-ttu-id="4be92-118">Apps können auf die angegebenen Datenschutz Daten zugreifen.</span><span class="sxs-lookup"><span data-stu-id="4be92-118">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="4be92-119">forceDeny</span><span class="sxs-lookup"><span data-stu-id="4be92-119">forceDeny</span></span>|<span data-ttu-id="4be92-120">2</span><span class="sxs-lookup"><span data-stu-id="4be92-120">2</span></span>|<span data-ttu-id="4be92-121">Apps wird der Zugriff auf die angegebenen Datenschutz Daten verweigert.</span><span class="sxs-lookup"><span data-stu-id="4be92-121">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="4be92-122">userInControl</span><span class="sxs-lookup"><span data-stu-id="4be92-122">userInControl</span></span>|<span data-ttu-id="4be92-123">3</span><span class="sxs-lookup"><span data-stu-id="4be92-123">3</span></span>|<span data-ttu-id="4be92-124">Benutzer werden aufgefordert, wenn apps versuchen, auf die angegebenen Datenschutz Daten zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="4be92-124">Users will be prompted when apps try to access specified privacy data.</span></span>|




