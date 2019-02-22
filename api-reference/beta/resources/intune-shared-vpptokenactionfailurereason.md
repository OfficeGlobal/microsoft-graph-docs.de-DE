---
title: vppTokenActionFailureReason-Enumerationstyp
description: Mögliche Ursachen für ein Apple Volume Purchase Program Token Action-Fehlers.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05d3137bb5aac2aef3024825df5e7e0b84ffde51
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169692"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="51abf-103">vppTokenActionFailureReason-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="51abf-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="51abf-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51abf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51abf-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="51abf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51abf-106">Mögliche Ursachen für ein Apple Volume Purchase Program Token Action-Fehlers.</span><span class="sxs-lookup"><span data-stu-id="51abf-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="51abf-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="51abf-107">Members</span></span>
|<span data-ttu-id="51abf-108">Element</span><span class="sxs-lookup"><span data-stu-id="51abf-108">Member</span></span>|<span data-ttu-id="51abf-109">Wert</span><span class="sxs-lookup"><span data-stu-id="51abf-109">Value</span></span>|<span data-ttu-id="51abf-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51abf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51abf-111">Keine</span><span class="sxs-lookup"><span data-stu-id="51abf-111">none</span></span>|<span data-ttu-id="51abf-112">0</span><span class="sxs-lookup"><span data-stu-id="51abf-112">0</span></span>|<span data-ttu-id="51abf-113">Keine.</span><span class="sxs-lookup"><span data-stu-id="51abf-113">None.</span></span>|
|<span data-ttu-id="51abf-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="51abf-114">appleFailure</span></span>|<span data-ttu-id="51abf-115">1</span><span class="sxs-lookup"><span data-stu-id="51abf-115">1</span></span>|<span data-ttu-id="51abf-116">Beim Apple-Dienst ist ein Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="51abf-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="51abf-117">internalError</span><span class="sxs-lookup"><span data-stu-id="51abf-117">internalError</span></span>|<span data-ttu-id="51abf-118">2</span><span class="sxs-lookup"><span data-stu-id="51abf-118">2</span></span>|<span data-ttu-id="51abf-119">Interner Fehler.</span><span class="sxs-lookup"><span data-stu-id="51abf-119">There was an internal error.</span></span>|
|<span data-ttu-id="51abf-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="51abf-120">expiredVppToken</span></span>|<span data-ttu-id="51abf-121">3</span><span class="sxs-lookup"><span data-stu-id="51abf-121">3</span></span>|<span data-ttu-id="51abf-122">Es ist ein Fehler aufgetreten, da das Apple Volume Purchase Program-Token abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="51abf-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="51abf-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="51abf-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="51abf-124">4</span><span class="sxs-lookup"><span data-stu-id="51abf-124">4</span></span>|<span data-ttu-id="51abf-125">Es ist ein Fehler aufgetreten, da das Apple Volume Purchase Program Push Notification Certificate abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="51abf-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|




