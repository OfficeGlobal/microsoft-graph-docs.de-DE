---
title: DeviceManagementExchangeConnectorSyncType Enum-Typ
description: Der Typ des Exchange-Connectors Synchronisierung angefordert.
author: tfitzmac
ms.openlocfilehash: dcad9b1455d488c9243b57f607281b39857cbf25
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316849"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="4444d-103">DeviceManagementExchangeConnectorSyncType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="4444d-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="4444d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4444d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4444d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4444d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4444d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4444d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4444d-107">Der Typ des Exchange-Connectors Synchronisierung angefordert.</span><span class="sxs-lookup"><span data-stu-id="4444d-107">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="4444d-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="4444d-108">Members</span></span>
|<span data-ttu-id="4444d-109">Member</span><span class="sxs-lookup"><span data-stu-id="4444d-109">Member</span></span>|<span data-ttu-id="4444d-110">Wert</span><span class="sxs-lookup"><span data-stu-id="4444d-110">Value</span></span>|<span data-ttu-id="4444d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4444d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4444d-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="4444d-112">fullSync</span></span>|<span data-ttu-id="4444d-113">0</span><span class="sxs-lookup"><span data-stu-id="4444d-113">0</span></span>|<span data-ttu-id="4444d-114">Entdecken Sie das Gerät im Exchange.</span><span class="sxs-lookup"><span data-stu-id="4444d-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="4444d-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="4444d-115">deltaSync</span></span>|<span data-ttu-id="4444d-116">1</span><span class="sxs-lookup"><span data-stu-id="4444d-116">1</span></span>|<span data-ttu-id="4444d-117">Entdecken Sie nur das Gerät in Exchange die während des Delta Sync-Fensters aktualisiert haben.</span><span class="sxs-lookup"><span data-stu-id="4444d-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





