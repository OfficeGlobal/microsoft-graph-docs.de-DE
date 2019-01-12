---
title: AppLockerApplicationControlType Enum-Typ
description: Mögliche Werte Anwendungstypen AppLocker-Steuerelement
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cb1fbb6ffe2ffc1841ebb4aa5ac1df91b762a788
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933575"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="30685-103">AppLockerApplicationControlType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="30685-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="30685-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="30685-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30685-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="30685-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30685-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="30685-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30685-107">Mögliche Werte Anwendungstypen AppLocker-Steuerelement</span><span class="sxs-lookup"><span data-stu-id="30685-107">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="30685-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="30685-108">Members</span></span>
|<span data-ttu-id="30685-109">Element</span><span class="sxs-lookup"><span data-stu-id="30685-109">Member</span></span>|<span data-ttu-id="30685-110">Wert</span><span class="sxs-lookup"><span data-stu-id="30685-110">Value</span></span>|<span data-ttu-id="30685-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30685-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30685-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="30685-112">notConfigured</span></span>|<span data-ttu-id="30685-113">0</span><span class="sxs-lookup"><span data-stu-id="30685-113">0</span></span>|<span data-ttu-id="30685-114">Gerät Standardwert, keine Anwendung Steuerelementtyp ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="30685-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="30685-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="30685-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="30685-116">1</span><span class="sxs-lookup"><span data-stu-id="30685-116">1</span></span>|<span data-ttu-id="30685-117">Windows-Komponente und Store-apps zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="30685-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="30685-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="30685-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="30685-119">2</span><span class="sxs-lookup"><span data-stu-id="30685-119">2</span></span>|<span data-ttu-id="30685-120">Überwachen Sie Windows-Komponente und Store-apps.</span><span class="sxs-lookup"><span data-stu-id="30685-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="30685-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="30685-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="30685-122">3</span><span class="sxs-lookup"><span data-stu-id="30685-122">3</span></span>|<span data-ttu-id="30685-123">Erzwingen Sie Windows-Komponenten zu, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="30685-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="30685-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="30685-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="30685-125">4</span><span class="sxs-lookup"><span data-stu-id="30685-125">4</span></span>|<span data-ttu-id="30685-126">Überwachen von Windows-Komponenten, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="30685-126">Audit Windows components, store apps and smart locker.</span></span>|





