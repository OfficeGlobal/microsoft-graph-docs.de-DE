---
title: groupPolicyConfigurationType-Enumerationstyp
description: Gruppenrichtlinien-Konfigurationstyp
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0d3a0daa73fef30e5425e188958bdc54e61778d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164687"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="78697-103">groupPolicyConfigurationType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="78697-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="78697-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78697-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78697-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="78697-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78697-106">Gruppenrichtlinien-Konfigurationstyp</span><span class="sxs-lookup"><span data-stu-id="78697-106">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="78697-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="78697-107">Members</span></span>
|<span data-ttu-id="78697-108">Element</span><span class="sxs-lookup"><span data-stu-id="78697-108">Member</span></span>|<span data-ttu-id="78697-109">Wert</span><span class="sxs-lookup"><span data-stu-id="78697-109">Value</span></span>|<span data-ttu-id="78697-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78697-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78697-111">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="78697-111">policy</span></span>|<span data-ttu-id="78697-112">0</span><span class="sxs-lookup"><span data-stu-id="78697-112">0</span></span>|<span data-ttu-id="78697-113">Der Richtlinientyp tätowiert den Wert nicht, was bedeutet, dass der Wert entfernt wird, sodass der ursprüngliche Konfigurationswert verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="78697-113">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="78697-114">Der Richtlinientyp überschreitet die Anwendungs Konfigurationseinstellung, sodass die Anwendung den Wert immer erkennt.</span><span class="sxs-lookup"><span data-stu-id="78697-114">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="78697-115">Der Richtlinientyp verhindert, dass der Benutzer den Wert über die Benutzeroberfläche der Anwendung ändert.</span><span class="sxs-lookup"><span data-stu-id="78697-115">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="78697-116">preference</span><span class="sxs-lookup"><span data-stu-id="78697-116">preference</span></span>|<span data-ttu-id="78697-117">1</span><span class="sxs-lookup"><span data-stu-id="78697-117">1</span></span>|<span data-ttu-id="78697-118">Der Einstellungstyp verwendet Tattoo als Wert, was bedeutet, dass der Wert nicht aus der Registrierung entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="78697-118">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="78697-119">Der Einstellungstyp überschreibt den Benutzer konfiguriert-Wert und behält nicht den vorherigen Wert bei.</span><span class="sxs-lookup"><span data-stu-id="78697-119">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="78697-120">Der Einstellungstyp verhindert nicht, dass der Benutzer den Wert über die Benutzeroberfläche der Anwendung ändert.</span><span class="sxs-lookup"><span data-stu-id="78697-120">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|




