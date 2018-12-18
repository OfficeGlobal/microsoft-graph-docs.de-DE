---
title: VppTokenActionFailureReason Enum-Typ
description: Möglichen Typen der Gründe für ein Apple Volume Purchase Program token Aktion Fehler aufgetreten.
author: tfitzmac
ms.openlocfilehash: f36b92238b097f50990bbdb2f3c3584b2ff48901
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320964"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="ff60c-103">VppTokenActionFailureReason Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ff60c-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="ff60c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff60c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff60c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff60c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff60c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff60c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff60c-107">Möglichen Typen der Gründe für ein Apple Volume Purchase Program token Aktion Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="ff60c-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>
## <a name="members"></a><span data-ttu-id="ff60c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="ff60c-108">Members</span></span>
|<span data-ttu-id="ff60c-109">Member</span><span class="sxs-lookup"><span data-stu-id="ff60c-109">Member</span></span>|<span data-ttu-id="ff60c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="ff60c-110">Value</span></span>|<span data-ttu-id="ff60c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff60c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff60c-112">Keine</span><span class="sxs-lookup"><span data-stu-id="ff60c-112">none</span></span>|<span data-ttu-id="ff60c-113">0</span><span class="sxs-lookup"><span data-stu-id="ff60c-113">0</span></span>|<span data-ttu-id="ff60c-114">Keine.</span><span class="sxs-lookup"><span data-stu-id="ff60c-114">None.</span></span>|
|<span data-ttu-id="ff60c-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="ff60c-115">appleFailure</span></span>|<span data-ttu-id="ff60c-116">1</span><span class="sxs-lookup"><span data-stu-id="ff60c-116">1</span></span>|<span data-ttu-id="ff60c-117">Apple Dienst ist ein Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="ff60c-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="ff60c-118">internalError</span><span class="sxs-lookup"><span data-stu-id="ff60c-118">internalError</span></span>|<span data-ttu-id="ff60c-119">2</span><span class="sxs-lookup"><span data-stu-id="ff60c-119">2</span></span>|<span data-ttu-id="ff60c-120">Ein interner Fehler ist aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="ff60c-120">There was an internal error.</span></span>|
|<span data-ttu-id="ff60c-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="ff60c-121">expiredVppToken</span></span>|<span data-ttu-id="ff60c-122">3</span><span class="sxs-lookup"><span data-stu-id="ff60c-122">3</span></span>|<span data-ttu-id="ff60c-123">Ein Fehler aufgetreten, da das Token Apple Volume Purchase Program abgelaufen wurde.</span><span class="sxs-lookup"><span data-stu-id="ff60c-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="ff60c-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ff60c-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="ff60c-125">4</span><span class="sxs-lookup"><span data-stu-id="ff60c-125">4</span></span>|<span data-ttu-id="ff60c-126">Ein Fehler aufgetreten, da das Apple Volume Purchase Programm Pushbenachrichtigung Zertifikat ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="ff60c-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





