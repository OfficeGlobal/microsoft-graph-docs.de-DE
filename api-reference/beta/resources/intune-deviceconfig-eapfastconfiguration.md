---
title: EapFastConfiguration Enum-Typ
description: Verfügbaren Einstellungen für EAP-FAST-Konfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65165929d388ed57f2651a0d277996e56d2f046e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954456"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="03f66-103">EapFastConfiguration Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="03f66-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="03f66-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="03f66-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03f66-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="03f66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03f66-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="03f66-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03f66-107">Verfügbaren Einstellungen für EAP-FAST-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="03f66-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="03f66-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="03f66-108">Members</span></span>
|<span data-ttu-id="03f66-109">Element</span><span class="sxs-lookup"><span data-stu-id="03f66-109">Member</span></span>|<span data-ttu-id="03f66-110">Wert</span><span class="sxs-lookup"><span data-stu-id="03f66-110">Value</span></span>|<span data-ttu-id="03f66-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03f66-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03f66-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="03f66-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="03f66-113">0</span><span class="sxs-lookup"><span data-stu-id="03f66-113">0</span></span>|<span data-ttu-id="03f66-114">EAP-FAST ohne geschützte Zugriffsberechtigung (PAC) verwenden.</span><span class="sxs-lookup"><span data-stu-id="03f66-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="03f66-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="03f66-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="03f66-116">1</span><span class="sxs-lookup"><span data-stu-id="03f66-116">1</span></span>|<span data-ttu-id="03f66-117">Verwenden Sie geschützte Zugriffsinformationen (PAC).</span><span class="sxs-lookup"><span data-stu-id="03f66-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="03f66-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="03f66-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="03f66-119">2</span><span class="sxs-lookup"><span data-stu-id="03f66-119">2</span></span>|<span data-ttu-id="03f66-120">Verwendung geschützt Access Anmeldeinformationen (PAC) und Provision PAC</span><span class="sxs-lookup"><span data-stu-id="03f66-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="03f66-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="03f66-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="03f66-122">3</span><span class="sxs-lookup"><span data-stu-id="03f66-122">3</span></span>|<span data-ttu-id="03f66-123">Verwenden Sie geschützte Zugriffsberechtigung (PAC), PAC bereitgestellt werden soll, und dazu anonym.</span><span class="sxs-lookup"><span data-stu-id="03f66-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





