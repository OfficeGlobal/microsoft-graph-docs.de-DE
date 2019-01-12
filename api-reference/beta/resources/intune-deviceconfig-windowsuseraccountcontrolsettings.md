---
title: WindowsUserAccountControlSettings Enum-Typ
description: Mögliche Werte für Windows-Benutzerkonto steuern Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd16db4236096687ddcc9f169dd657c938fd6815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911812"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="d8184-103">WindowsUserAccountControlSettings Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="d8184-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="d8184-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d8184-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8184-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8184-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8184-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d8184-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8184-107">Mögliche Werte für Windows-Benutzerkonto steuern Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="d8184-107">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="d8184-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="d8184-108">Members</span></span>
|<span data-ttu-id="d8184-109">Element</span><span class="sxs-lookup"><span data-stu-id="d8184-109">Member</span></span>|<span data-ttu-id="d8184-110">Wert</span><span class="sxs-lookup"><span data-stu-id="d8184-110">Value</span></span>|<span data-ttu-id="d8184-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8184-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8184-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="d8184-112">userDefined</span></span>|<span data-ttu-id="d8184-113">0</span><span class="sxs-lookup"><span data-stu-id="d8184-113">0</span></span>|<span data-ttu-id="d8184-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="d8184-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d8184-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="d8184-115">alwaysNotify</span></span>|<span data-ttu-id="d8184-116">1</span><span class="sxs-lookup"><span data-stu-id="d8184-116">1</span></span>|<span data-ttu-id="d8184-117">Immer benachrichtigen.</span><span class="sxs-lookup"><span data-stu-id="d8184-117">Always notify.</span></span>|
|<span data-ttu-id="d8184-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="d8184-118">notifyOnAppChanges</span></span>|<span data-ttu-id="d8184-119">2</span><span class="sxs-lookup"><span data-stu-id="d8184-119">2</span></span>|<span data-ttu-id="d8184-120">Benachrichtigen Sie app geändert wird.</span><span class="sxs-lookup"><span data-stu-id="d8184-120">Notify on app changes.</span></span>|
|<span data-ttu-id="d8184-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="d8184-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="d8184-122">3</span><span class="sxs-lookup"><span data-stu-id="d8184-122">3</span></span>|<span data-ttu-id="d8184-123">Benachrichtigen Sie ohne Abblenden Desktop app geändert wird.</span><span class="sxs-lookup"><span data-stu-id="d8184-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="d8184-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="d8184-124">neverNotify</span></span>|<span data-ttu-id="d8184-125">4</span><span class="sxs-lookup"><span data-stu-id="d8184-125">4</span></span>|<span data-ttu-id="d8184-126">Nie benachrichtigen.</span><span class="sxs-lookup"><span data-stu-id="d8184-126">Never notify.</span></span>|





