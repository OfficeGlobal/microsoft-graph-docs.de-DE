---
title: VppTokenActionFailureReason Enum-Typ
description: Möglichen Typen der Gründe für ein Apple Volume Purchase Program token Aktion Fehler aufgetreten.
ms.openlocfilehash: 0fece0417a5585540f15e3f8a8631fd30eaa414e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060749"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="65b0c-103">VppTokenActionFailureReason Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="65b0c-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="65b0c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="65b0c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65b0c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65b0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65b0c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="65b0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65b0c-107">Möglichen Typen der Gründe für ein Apple Volume Purchase Program token Aktion Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="65b0c-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>
## <a name="members"></a><span data-ttu-id="65b0c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="65b0c-108">Members</span></span>
|<span data-ttu-id="65b0c-109">Element</span><span class="sxs-lookup"><span data-stu-id="65b0c-109">Member</span></span>|<span data-ttu-id="65b0c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="65b0c-110">Value</span></span>|<span data-ttu-id="65b0c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65b0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65b0c-112">n/v</span><span class="sxs-lookup"><span data-stu-id="65b0c-112">none</span></span>|<span data-ttu-id="65b0c-113">0</span><span class="sxs-lookup"><span data-stu-id="65b0c-113">0</span></span>|<span data-ttu-id="65b0c-114">Keine.</span><span class="sxs-lookup"><span data-stu-id="65b0c-114">None.</span></span>|
|<span data-ttu-id="65b0c-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="65b0c-115">appleFailure</span></span>|<span data-ttu-id="65b0c-116">1</span><span class="sxs-lookup"><span data-stu-id="65b0c-116">1</span></span>|<span data-ttu-id="65b0c-117">Apple Dienst ist ein Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="65b0c-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="65b0c-118">internalError</span><span class="sxs-lookup"><span data-stu-id="65b0c-118">internalError</span></span>|<span data-ttu-id="65b0c-119">2</span><span class="sxs-lookup"><span data-stu-id="65b0c-119">2</span></span>|<span data-ttu-id="65b0c-120">Ein interner Fehler ist aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="65b0c-120">There was an internal error.</span></span>|
|<span data-ttu-id="65b0c-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="65b0c-121">expiredVppToken</span></span>|<span data-ttu-id="65b0c-122">3</span><span class="sxs-lookup"><span data-stu-id="65b0c-122">3</span></span>|<span data-ttu-id="65b0c-123">Ein Fehler aufgetreten, da das Token Apple Volume Purchase Program abgelaufen wurde.</span><span class="sxs-lookup"><span data-stu-id="65b0c-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="65b0c-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="65b0c-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="65b0c-125">4</span><span class="sxs-lookup"><span data-stu-id="65b0c-125">4</span></span>|<span data-ttu-id="65b0c-126">Ein Fehler aufgetreten, da das Apple Volume Purchase Programm Pushbenachrichtigung Zertifikat ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="65b0c-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





