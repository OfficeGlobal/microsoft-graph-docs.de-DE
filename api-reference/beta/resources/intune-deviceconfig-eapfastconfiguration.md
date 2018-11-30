---
title: EapFastConfiguration Enum-Typ
description: Verfügbaren Einstellungen für EAP-FAST-Konfiguration.
ms.openlocfilehash: b1771668ea627d2e873d54334e388989652736d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060567"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="bc57f-103">EapFastConfiguration Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="bc57f-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="bc57f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bc57f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc57f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc57f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc57f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bc57f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc57f-107">Verfügbaren Einstellungen für EAP-FAST-Konfiguration.</span><span class="sxs-lookup"><span data-stu-id="bc57f-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="bc57f-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="bc57f-108">Members</span></span>
|<span data-ttu-id="bc57f-109">Element</span><span class="sxs-lookup"><span data-stu-id="bc57f-109">Member</span></span>|<span data-ttu-id="bc57f-110">Wert</span><span class="sxs-lookup"><span data-stu-id="bc57f-110">Value</span></span>|<span data-ttu-id="bc57f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc57f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc57f-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="bc57f-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="bc57f-113">0</span><span class="sxs-lookup"><span data-stu-id="bc57f-113">0</span></span>|<span data-ttu-id="bc57f-114">EAP-FAST ohne geschützte Zugriffsberechtigung (PAC) verwenden.</span><span class="sxs-lookup"><span data-stu-id="bc57f-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="bc57f-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="bc57f-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="bc57f-116">1</span><span class="sxs-lookup"><span data-stu-id="bc57f-116">1</span></span>|<span data-ttu-id="bc57f-117">Verwenden Sie geschützte Zugriffsinformationen (PAC).</span><span class="sxs-lookup"><span data-stu-id="bc57f-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="bc57f-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="bc57f-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="bc57f-119">2</span><span class="sxs-lookup"><span data-stu-id="bc57f-119">2</span></span>|<span data-ttu-id="bc57f-120">Verwendung geschützt Access Anmeldeinformationen (PAC) und Provision PAC</span><span class="sxs-lookup"><span data-stu-id="bc57f-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="bc57f-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="bc57f-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="bc57f-122">3</span><span class="sxs-lookup"><span data-stu-id="bc57f-122">3</span></span>|<span data-ttu-id="bc57f-123">Verwenden Sie geschützte Zugriffsberechtigung (PAC), PAC bereitgestellt werden soll, und dazu anonym.</span><span class="sxs-lookup"><span data-stu-id="bc57f-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





