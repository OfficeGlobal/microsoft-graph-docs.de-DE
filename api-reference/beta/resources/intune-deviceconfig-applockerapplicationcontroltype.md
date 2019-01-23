---
title: AppLockerApplicationControlType Enum-Typ
description: Mögliche Werte Anwendungstypen AppLocker-Steuerelement
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3bc89620a6dd13a65cfe40f37ba2f775e6a9c83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425722"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="3b30a-103">AppLockerApplicationControlType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="3b30a-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="3b30a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3b30a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3b30a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b30a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b30a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b30a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b30a-107">Mögliche Werte Anwendungstypen AppLocker-Steuerelement</span><span class="sxs-lookup"><span data-stu-id="3b30a-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="3b30a-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="3b30a-108">Members</span></span>
|<span data-ttu-id="3b30a-109">Member</span><span class="sxs-lookup"><span data-stu-id="3b30a-109">Member</span></span>|<span data-ttu-id="3b30a-110">Wert</span><span class="sxs-lookup"><span data-stu-id="3b30a-110">Value</span></span>|<span data-ttu-id="3b30a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b30a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b30a-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="3b30a-112">notConfigured</span></span>|<span data-ttu-id="3b30a-113">0</span><span class="sxs-lookup"><span data-stu-id="3b30a-113">0</span></span>|<span data-ttu-id="3b30a-114">Gerät Standardwert, keine Anwendung Steuerelementtyp ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="3b30a-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="3b30a-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="3b30a-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="3b30a-116">1</span><span class="sxs-lookup"><span data-stu-id="3b30a-116">1</span></span>|<span data-ttu-id="3b30a-117">Windows-Komponente und Store-apps zu erzwingen.</span><span class="sxs-lookup"><span data-stu-id="3b30a-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="3b30a-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="3b30a-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="3b30a-119">2</span><span class="sxs-lookup"><span data-stu-id="3b30a-119">2</span></span>|<span data-ttu-id="3b30a-120">Überwachen Sie Windows-Komponente und Store-apps.</span><span class="sxs-lookup"><span data-stu-id="3b30a-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="3b30a-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="3b30a-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="3b30a-122">3</span><span class="sxs-lookup"><span data-stu-id="3b30a-122">3</span></span>|<span data-ttu-id="3b30a-123">Erzwingen Sie Windows-Komponenten zu, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="3b30a-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="3b30a-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="3b30a-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="3b30a-125">4</span><span class="sxs-lookup"><span data-stu-id="3b30a-125">4</span></span>|<span data-ttu-id="3b30a-126">Überwachen von Windows-Komponenten, apps und intelligente Locker.</span><span class="sxs-lookup"><span data-stu-id="3b30a-126">Audit Windows components, store apps and smart locker.</span></span>|




