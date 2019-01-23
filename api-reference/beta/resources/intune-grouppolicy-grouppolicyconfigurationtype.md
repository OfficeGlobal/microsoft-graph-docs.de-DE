---
title: GroupPolicyConfigurationType Enum-Typ
description: Gruppe Richtlinientyp Konfiguration
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 372a5bd5656510c43b388bac128cba4bc46c0988
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430058"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="feaf8-103">GroupPolicyConfigurationType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="feaf8-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="feaf8-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="feaf8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="feaf8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="feaf8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="feaf8-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="feaf8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feaf8-107">Gruppe Richtlinientyp Konfiguration</span><span class="sxs-lookup"><span data-stu-id="feaf8-107">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="feaf8-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="feaf8-108">Members</span></span>
|<span data-ttu-id="feaf8-109">Member</span><span class="sxs-lookup"><span data-stu-id="feaf8-109">Member</span></span>|<span data-ttu-id="feaf8-110">Wert</span><span class="sxs-lookup"><span data-stu-id="feaf8-110">Value</span></span>|<span data-ttu-id="feaf8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="feaf8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feaf8-112">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="feaf8-112">policy</span></span>|<span data-ttu-id="feaf8-113">0</span><span class="sxs-lookup"><span data-stu-id="feaf8-113">0</span></span>|<span data-ttu-id="feaf8-114">Der Richtlinientyp ist nicht den Wert verunreinigen mit diesen Werten bedeutet, dass der Wert entfernt wird den Originalwert der Konfiguration verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="feaf8-114">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="feaf8-115">Der Richtlinientyp ersetzt Einstellung für die Konfiguration, damit die Anwendung immer den Wert bekannt sind.</span><span class="sxs-lookup"><span data-stu-id="feaf8-115">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="feaf8-116">Der Richtlinientyp verhindert, dass den Benutzer den Wert den über die Benutzeroberfläche der Anwendung ändern.</span><span class="sxs-lookup"><span data-stu-id="feaf8-116">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="feaf8-117">preference</span><span class="sxs-lookup"><span data-stu-id="feaf8-117">preference</span></span>|<span data-ttu-id="feaf8-118">1</span><span class="sxs-lookup"><span data-stu-id="feaf8-118">1</span></span>|<span data-ttu-id="feaf8-119">Der Typ der Einstellung den Wert verunreinigen mit diesen Werten bedeutet, dass der Wert nicht aus der Registrierung entfernt wird.</span><span class="sxs-lookup"><span data-stu-id="feaf8-119">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="feaf8-120">Der Typ der Einstellung überschreibt den Benutzer konfiguriert-Wert und den vorherigen Wert nicht beibehalten.</span><span class="sxs-lookup"><span data-stu-id="feaf8-120">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="feaf8-121">Welche Option Sie bevorzugen es wird nicht verhindert, dass den Benutzer den Wert den über die Benutzeroberfläche der Anwendung ändern.</span><span class="sxs-lookup"><span data-stu-id="feaf8-121">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|




