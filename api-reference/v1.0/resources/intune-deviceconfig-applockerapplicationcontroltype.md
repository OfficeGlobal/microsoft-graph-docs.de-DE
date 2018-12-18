---
title: AppLockerApplicationControlType Enum-Typ
description: Mögliche Werte Anwendungstypen AppLocker-Steuerelement
author: tfitzmac
ms.openlocfilehash: d53c2d0f7996edfab610e4206f4d2815ba4000b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310262"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="3661d-103">AppLockerApplicationControlType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="3661d-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="3661d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3661d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3661d-105">Mögliche Werte Anwendungstypen AppLocker-Steuerelement</span><span class="sxs-lookup"><span data-stu-id="3661d-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="3661d-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="3661d-106">Members</span></span>
|<span data-ttu-id="3661d-107">Member</span><span class="sxs-lookup"><span data-stu-id="3661d-107">Member</span></span>|<span data-ttu-id="3661d-108">Wert</span><span class="sxs-lookup"><span data-stu-id="3661d-108">Value</span></span>|<span data-ttu-id="3661d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3661d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3661d-110">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="3661d-110">notConfigured</span></span>|<span data-ttu-id="3661d-111">0</span><span class="sxs-lookup"><span data-stu-id="3661d-111">0</span></span>|<span data-ttu-id="3661d-112">Gerät Standardwert, keine Anwendung Steuerelementtyp ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="3661d-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="3661d-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="3661d-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="3661d-114">1</span><span class="sxs-lookup"><span data-stu-id="3661d-114">1</span></span>|<span data-ttu-id="3661d-115">Windows-Komponente und Store-apps zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="3661d-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="3661d-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="3661d-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="3661d-117">2</span><span class="sxs-lookup"><span data-stu-id="3661d-117">2</span></span>|<span data-ttu-id="3661d-118">Überwachen Sie Windows-Komponente und Store-apps.</span><span class="sxs-lookup"><span data-stu-id="3661d-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="3661d-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="3661d-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="3661d-120">3</span><span class="sxs-lookup"><span data-stu-id="3661d-120">3</span></span>|<span data-ttu-id="3661d-121">Erzwingen Sie Windows-Komponenten zu, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="3661d-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="3661d-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="3661d-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="3661d-123">4</span><span class="sxs-lookup"><span data-stu-id="3661d-123">4</span></span>|<span data-ttu-id="3661d-124">Überwachen von Windows-Komponenten, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="3661d-124">Audit Windows components, store apps and smart locker.</span></span>|



