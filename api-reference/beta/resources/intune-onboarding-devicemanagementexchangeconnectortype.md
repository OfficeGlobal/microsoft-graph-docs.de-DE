---
title: DeviceManagementExchangeConnectorType Enum-Typ
description: Der Typ des Exchange-Connectors.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c05410c3b3b7c889840d0b47aca05f6457564eb4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934953"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="b0879-103">DeviceManagementExchangeConnectorType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b0879-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="b0879-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b0879-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0879-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b0879-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0879-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b0879-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0879-107">Der Typ des Exchange-Connectors.</span><span class="sxs-lookup"><span data-stu-id="b0879-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="b0879-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b0879-108">Members</span></span>
|<span data-ttu-id="b0879-109">Element</span><span class="sxs-lookup"><span data-stu-id="b0879-109">Member</span></span>|<span data-ttu-id="b0879-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b0879-110">Value</span></span>|<span data-ttu-id="b0879-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0879-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0879-112">"lokal"</span><span class="sxs-lookup"><span data-stu-id="b0879-112">onPremises</span></span>|<span data-ttu-id="b0879-113">0</span><span class="sxs-lookup"><span data-stu-id="b0879-113">0</span></span>|<span data-ttu-id="b0879-114">Stellt eine Verbindung zum lokalen Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="b0879-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="b0879-115">gehostet</span><span class="sxs-lookup"><span data-stu-id="b0879-115">hosted</span></span>|<span data-ttu-id="b0879-116">1</span><span class="sxs-lookup"><span data-stu-id="b0879-116">1</span></span>|<span data-ttu-id="b0879-117">Stellt eine Verbindung mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="b0879-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="b0879-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="b0879-118">serviceToService</span></span>|<span data-ttu-id="b0879-119">2</span><span class="sxs-lookup"><span data-stu-id="b0879-119">2</span></span>|<span data-ttu-id="b0879-120">Intune Service verbindet direkt mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="b0879-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="b0879-121">dedizierte</span><span class="sxs-lookup"><span data-stu-id="b0879-121">dedicated</span></span>|<span data-ttu-id="b0879-122">3</span><span class="sxs-lookup"><span data-stu-id="b0879-122">3</span></span>|<span data-ttu-id="b0879-123">Stellt eine Verbindung zu Office 365 dedizierte Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="b0879-123">Connects to O365 Dedicated Exchange environment.</span></span>|





