---
title: WindowsInformationProtectionEnforcementLevel Enum-Typ
description: Mögliche Werte für WIP Erzwingung Schutzebenen
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed087465d05ba91bcdc1f8cff7fec0aba567420a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913408"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="9191c-103">WindowsInformationProtectionEnforcementLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="9191c-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="9191c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9191c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9191c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9191c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9191c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9191c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9191c-107">Mögliche Werte für WIP Erzwingung Schutzebenen</span><span class="sxs-lookup"><span data-stu-id="9191c-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="9191c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="9191c-108">Members</span></span>
|<span data-ttu-id="9191c-109">Element</span><span class="sxs-lookup"><span data-stu-id="9191c-109">Member</span></span>|<span data-ttu-id="9191c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="9191c-110">Value</span></span>|<span data-ttu-id="9191c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9191c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9191c-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="9191c-112">noProtection</span></span>|<span data-ttu-id="9191c-113">0</span><span class="sxs-lookup"><span data-stu-id="9191c-113">0</span></span>|<span data-ttu-id="9191c-114">Kein Schutz Erzwingung</span><span class="sxs-lookup"><span data-stu-id="9191c-114">No protection enforcement</span></span>|
|<span data-ttu-id="9191c-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="9191c-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="9191c-116">1</span><span class="sxs-lookup"><span data-stu-id="9191c-116">1</span></span>|<span data-ttu-id="9191c-117">Verschlüsseln und überwachen nur</span><span class="sxs-lookup"><span data-stu-id="9191c-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="9191c-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="9191c-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="9191c-119">2</span><span class="sxs-lookup"><span data-stu-id="9191c-119">2</span></span>|<span data-ttu-id="9191c-120">Verschlüsseln, überwachen und auffordern</span><span class="sxs-lookup"><span data-stu-id="9191c-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="9191c-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="9191c-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="9191c-122">3</span><span class="sxs-lookup"><span data-stu-id="9191c-122">3</span></span>|<span data-ttu-id="9191c-123">Verschlüsseln, überwachen und blockieren</span><span class="sxs-lookup"><span data-stu-id="9191c-123">Encrypt, Audit and Block</span></span>|





