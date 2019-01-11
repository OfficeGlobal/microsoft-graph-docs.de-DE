---
title: AppLockerApplicationControlType Enum-Typ
description: Mögliche Werte Anwendungstypen AppLocker-Steuerelement
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 241387f34a64b4b58d974fc21e2aa5d3af696736
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871981"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="8e6f4-103">AppLockerApplicationControlType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="8e6f4-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="8e6f4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e6f4-105">Mögliche Werte Anwendungstypen AppLocker-Steuerelement</span><span class="sxs-lookup"><span data-stu-id="8e6f4-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="8e6f4-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="8e6f4-106">Members</span></span>
|<span data-ttu-id="8e6f4-107">Element</span><span class="sxs-lookup"><span data-stu-id="8e6f4-107">Member</span></span>|<span data-ttu-id="8e6f4-108">Wert</span><span class="sxs-lookup"><span data-stu-id="8e6f4-108">Value</span></span>|<span data-ttu-id="8e6f4-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e6f4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e6f4-110">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="8e6f4-110">notConfigured</span></span>|<span data-ttu-id="8e6f4-111">0</span><span class="sxs-lookup"><span data-stu-id="8e6f4-111">0</span></span>|<span data-ttu-id="8e6f4-112">Gerät Standardwert, keine Anwendung Steuerelementtyp ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="8e6f4-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="8e6f4-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="8e6f4-114">1</span><span class="sxs-lookup"><span data-stu-id="8e6f4-114">1</span></span>|<span data-ttu-id="8e6f4-115">Windows-Komponente und Store-apps zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="8e6f4-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="8e6f4-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="8e6f4-117">2</span><span class="sxs-lookup"><span data-stu-id="8e6f4-117">2</span></span>|<span data-ttu-id="8e6f4-118">Überwachen Sie Windows-Komponente und Store-apps.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="8e6f4-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="8e6f4-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="8e6f4-120">3</span><span class="sxs-lookup"><span data-stu-id="8e6f4-120">3</span></span>|<span data-ttu-id="8e6f4-121">Erzwingen Sie Windows-Komponenten zu, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="8e6f4-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="8e6f4-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="8e6f4-123">4</span><span class="sxs-lookup"><span data-stu-id="8e6f4-123">4</span></span>|<span data-ttu-id="8e6f4-124">Überwachen von Windows-Komponenten, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="8e6f4-124">Audit Windows components, store apps and smart locker.</span></span>|



