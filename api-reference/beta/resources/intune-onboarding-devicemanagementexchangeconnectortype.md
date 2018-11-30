---
title: DeviceManagementExchangeConnectorType Enum-Typ
description: Der Typ des Exchange-Connectors.
ms.openlocfilehash: 59bc1aa080f84fdd25a2da26ec9e7ff9aba20641
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059790"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="3289e-103">DeviceManagementExchangeConnectorType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="3289e-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="3289e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3289e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3289e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3289e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3289e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3289e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3289e-107">Der Typ des Exchange-Connectors.</span><span class="sxs-lookup"><span data-stu-id="3289e-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="3289e-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="3289e-108">Members</span></span>
|<span data-ttu-id="3289e-109">Element</span><span class="sxs-lookup"><span data-stu-id="3289e-109">Member</span></span>|<span data-ttu-id="3289e-110">Wert</span><span class="sxs-lookup"><span data-stu-id="3289e-110">Value</span></span>|<span data-ttu-id="3289e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3289e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3289e-112">"lokal"</span><span class="sxs-lookup"><span data-stu-id="3289e-112">onPremises</span></span>|<span data-ttu-id="3289e-113">0</span><span class="sxs-lookup"><span data-stu-id="3289e-113">0</span></span>|<span data-ttu-id="3289e-114">Stellt eine Verbindung zum lokalen Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="3289e-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="3289e-115">gehostet</span><span class="sxs-lookup"><span data-stu-id="3289e-115">hosted</span></span>|<span data-ttu-id="3289e-116">1</span><span class="sxs-lookup"><span data-stu-id="3289e-116">1</span></span>|<span data-ttu-id="3289e-117">Stellt eine Verbindung mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="3289e-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="3289e-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="3289e-118">serviceToService</span></span>|<span data-ttu-id="3289e-119">2</span><span class="sxs-lookup"><span data-stu-id="3289e-119">2</span></span>|<span data-ttu-id="3289e-120">Intune Service verbindet direkt mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="3289e-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="3289e-121">dedizierte</span><span class="sxs-lookup"><span data-stu-id="3289e-121">dedicated</span></span>|<span data-ttu-id="3289e-122">3</span><span class="sxs-lookup"><span data-stu-id="3289e-122">3</span></span>|<span data-ttu-id="3289e-123">Stellt eine Verbindung zu Office 365 dedizierte Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="3289e-123">Connects to O365 Dedicated Exchange environment.</span></span>|





