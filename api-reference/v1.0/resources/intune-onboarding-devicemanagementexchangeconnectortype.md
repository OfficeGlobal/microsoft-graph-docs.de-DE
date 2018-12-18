---
title: DeviceManagementExchangeConnectorType Enum-Typ
description: Der Typ des Exchange-Connectors.
author: tfitzmac
ms.openlocfilehash: 333a5a7c6f73fead263edbdf3edafeefc3514ed1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306734"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="b5302-103">DeviceManagementExchangeConnectorType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b5302-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="b5302-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b5302-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5302-105">Der Typ des Exchange-Connectors.</span><span class="sxs-lookup"><span data-stu-id="b5302-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="b5302-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="b5302-106">Members</span></span>
|<span data-ttu-id="b5302-107">Member</span><span class="sxs-lookup"><span data-stu-id="b5302-107">Member</span></span>|<span data-ttu-id="b5302-108">Wert</span><span class="sxs-lookup"><span data-stu-id="b5302-108">Value</span></span>|<span data-ttu-id="b5302-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5302-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5302-110">"lokal"</span><span class="sxs-lookup"><span data-stu-id="b5302-110">onPremises</span></span>|<span data-ttu-id="b5302-111">0</span><span class="sxs-lookup"><span data-stu-id="b5302-111">0</span></span>|<span data-ttu-id="b5302-112">Stellt eine Verbindung zum lokalen Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="b5302-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="b5302-113">gehostet</span><span class="sxs-lookup"><span data-stu-id="b5302-113">hosted</span></span>|<span data-ttu-id="b5302-114">1</span><span class="sxs-lookup"><span data-stu-id="b5302-114">1</span></span>|<span data-ttu-id="b5302-115">Stellt eine Verbindung mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="b5302-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="b5302-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="b5302-116">serviceToService</span></span>|<span data-ttu-id="b5302-117">2</span><span class="sxs-lookup"><span data-stu-id="b5302-117">2</span></span>|<span data-ttu-id="b5302-118">Intune Service verbindet direkt mit Office 365 mit mehreren Mandanten Exchange-Umgebung</span><span class="sxs-lookup"><span data-stu-id="b5302-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="b5302-119">dedizierte</span><span class="sxs-lookup"><span data-stu-id="b5302-119">dedicated</span></span>|<span data-ttu-id="b5302-120">3</span><span class="sxs-lookup"><span data-stu-id="b5302-120">3</span></span>|<span data-ttu-id="b5302-121">Stellt eine Verbindung zu Office 365 dedizierte Exchange-Umgebung.</span><span class="sxs-lookup"><span data-stu-id="b5302-121">Connects to O365 Dedicated Exchange environment.</span></span>|



