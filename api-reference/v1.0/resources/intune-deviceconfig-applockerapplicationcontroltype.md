---
title: AppLockerApplicationControlType Enum-Typ
description: Mögliche Werte Anwendungstypen AppLocker-Steuerelement
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 258a98b9ec4945c807a6aae2b34a178628952ac4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937957"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="c953f-103">AppLockerApplicationControlType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c953f-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="c953f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c953f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c953f-105">Mögliche Werte Anwendungstypen AppLocker-Steuerelement</span><span class="sxs-lookup"><span data-stu-id="c953f-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="c953f-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="c953f-106">Members</span></span>
|<span data-ttu-id="c953f-107">Element</span><span class="sxs-lookup"><span data-stu-id="c953f-107">Member</span></span>|<span data-ttu-id="c953f-108">Wert</span><span class="sxs-lookup"><span data-stu-id="c953f-108">Value</span></span>|<span data-ttu-id="c953f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c953f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c953f-110">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="c953f-110">notConfigured</span></span>|<span data-ttu-id="c953f-111">0</span><span class="sxs-lookup"><span data-stu-id="c953f-111">0</span></span>|<span data-ttu-id="c953f-112">Gerät Standardwert, keine Anwendung Steuerelementtyp ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="c953f-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="c953f-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="c953f-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="c953f-114">1</span><span class="sxs-lookup"><span data-stu-id="c953f-114">1</span></span>|<span data-ttu-id="c953f-115">Windows-Komponente und Store-apps zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="c953f-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="c953f-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="c953f-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="c953f-117">2</span><span class="sxs-lookup"><span data-stu-id="c953f-117">2</span></span>|<span data-ttu-id="c953f-118">Überwachen Sie Windows-Komponente und Store-apps.</span><span class="sxs-lookup"><span data-stu-id="c953f-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="c953f-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="c953f-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c953f-120">3</span><span class="sxs-lookup"><span data-stu-id="c953f-120">3</span></span>|<span data-ttu-id="c953f-121">Erzwingen Sie Windows-Komponenten zu, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="c953f-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="c953f-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="c953f-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c953f-123">4</span><span class="sxs-lookup"><span data-stu-id="c953f-123">4</span></span>|<span data-ttu-id="c953f-124">Überwachen von Windows-Komponenten, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="c953f-124">Audit Windows components, store apps and smart locker.</span></span>|



