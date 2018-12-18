---
title: AppLockerApplicationControlType Enum-Typ
description: Mögliche Werte Anwendungstypen AppLocker-Steuerelement
author: tfitzmac
ms.openlocfilehash: 0d6190170d6f6695a3303047f9ccb193afd248f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330205"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="b9b68-103">AppLockerApplicationControlType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b9b68-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="b9b68-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9b68-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9b68-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9b68-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9b68-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b9b68-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9b68-107">Mögliche Werte Anwendungstypen AppLocker-Steuerelement</span><span class="sxs-lookup"><span data-stu-id="b9b68-107">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="b9b68-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b9b68-108">Members</span></span>
|<span data-ttu-id="b9b68-109">Member</span><span class="sxs-lookup"><span data-stu-id="b9b68-109">Member</span></span>|<span data-ttu-id="b9b68-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b9b68-110">Value</span></span>|<span data-ttu-id="b9b68-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9b68-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9b68-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="b9b68-112">notConfigured</span></span>|<span data-ttu-id="b9b68-113">0</span><span class="sxs-lookup"><span data-stu-id="b9b68-113">0</span></span>|<span data-ttu-id="b9b68-114">Gerät Standardwert, keine Anwendung Steuerelementtyp ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="b9b68-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="b9b68-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="b9b68-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="b9b68-116">1</span><span class="sxs-lookup"><span data-stu-id="b9b68-116">1</span></span>|<span data-ttu-id="b9b68-117">Windows-Komponente und Store-apps zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="b9b68-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="b9b68-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="b9b68-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="b9b68-119">2</span><span class="sxs-lookup"><span data-stu-id="b9b68-119">2</span></span>|<span data-ttu-id="b9b68-120">Überwachen Sie Windows-Komponente und Store-apps.</span><span class="sxs-lookup"><span data-stu-id="b9b68-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="b9b68-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="b9b68-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="b9b68-122">3</span><span class="sxs-lookup"><span data-stu-id="b9b68-122">3</span></span>|<span data-ttu-id="b9b68-123">Erzwingen Sie Windows-Komponenten zu, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="b9b68-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="b9b68-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="b9b68-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="b9b68-125">4</span><span class="sxs-lookup"><span data-stu-id="b9b68-125">4</span></span>|<span data-ttu-id="b9b68-126">Überwachen von Windows-Komponenten, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="b9b68-126">Audit Windows components, store apps and smart locker.</span></span>|





