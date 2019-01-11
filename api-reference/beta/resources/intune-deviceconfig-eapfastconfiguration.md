---
title: EapFastConfiguration Enum-Typ
description: Verfügbaren Einstellungen für EAP-FAST-Konfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 499d6595980bcb6bca1ea93687399e8988a3bed7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811088"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="3aedf-103">EapFastConfiguration Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="3aedf-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="3aedf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3aedf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3aedf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3aedf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3aedf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3aedf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3aedf-107">Verfügbaren Einstellungen für EAP-FAST-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="3aedf-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="3aedf-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="3aedf-108">Members</span></span>
|<span data-ttu-id="3aedf-109">Element</span><span class="sxs-lookup"><span data-stu-id="3aedf-109">Member</span></span>|<span data-ttu-id="3aedf-110">Wert</span><span class="sxs-lookup"><span data-stu-id="3aedf-110">Value</span></span>|<span data-ttu-id="3aedf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3aedf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3aedf-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="3aedf-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="3aedf-113">0</span><span class="sxs-lookup"><span data-stu-id="3aedf-113">0</span></span>|<span data-ttu-id="3aedf-114">EAP-FAST ohne geschützte Zugriffsberechtigung (PAC) verwenden.</span><span class="sxs-lookup"><span data-stu-id="3aedf-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="3aedf-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="3aedf-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="3aedf-116">1</span><span class="sxs-lookup"><span data-stu-id="3aedf-116">1</span></span>|<span data-ttu-id="3aedf-117">Verwenden Sie geschützte Zugriffsinformationen (PAC).</span><span class="sxs-lookup"><span data-stu-id="3aedf-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="3aedf-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="3aedf-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="3aedf-119">2</span><span class="sxs-lookup"><span data-stu-id="3aedf-119">2</span></span>|<span data-ttu-id="3aedf-120">Verwendung geschützt Access Anmeldeinformationen (PAC) und Provision PAC</span><span class="sxs-lookup"><span data-stu-id="3aedf-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="3aedf-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="3aedf-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="3aedf-122">3</span><span class="sxs-lookup"><span data-stu-id="3aedf-122">3</span></span>|<span data-ttu-id="3aedf-123">Verwenden Sie geschützte Zugriffsberechtigung (PAC), PAC bereitgestellt werden soll, und dazu anonym.</span><span class="sxs-lookup"><span data-stu-id="3aedf-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





