---
title: VppTokenActionFailureReason Enum-Typ
description: Möglichen Typen der Gründe für ein Apple Volume Purchase Program token Aktion Fehler aufgetreten.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba4c339b774fd32a852925729e2e158dc13e52d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393144"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="a68dc-103">VppTokenActionFailureReason Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a68dc-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="a68dc-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a68dc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a68dc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a68dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a68dc-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a68dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a68dc-107">Möglichen Typen der Gründe für ein Apple Volume Purchase Program token Aktion Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="a68dc-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="a68dc-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="a68dc-108">Members</span></span>
|<span data-ttu-id="a68dc-109">Member</span><span class="sxs-lookup"><span data-stu-id="a68dc-109">Member</span></span>|<span data-ttu-id="a68dc-110">Wert</span><span class="sxs-lookup"><span data-stu-id="a68dc-110">Value</span></span>|<span data-ttu-id="a68dc-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a68dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a68dc-112">Keine</span><span class="sxs-lookup"><span data-stu-id="a68dc-112">none</span></span>|<span data-ttu-id="a68dc-113">0</span><span class="sxs-lookup"><span data-stu-id="a68dc-113">0</span></span>|<span data-ttu-id="a68dc-114">Keine.</span><span class="sxs-lookup"><span data-stu-id="a68dc-114">None.</span></span>|
|<span data-ttu-id="a68dc-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="a68dc-115">appleFailure</span></span>|<span data-ttu-id="a68dc-116">1</span><span class="sxs-lookup"><span data-stu-id="a68dc-116">1</span></span>|<span data-ttu-id="a68dc-117">Apple Dienst ist ein Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="a68dc-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="a68dc-118">internalError</span><span class="sxs-lookup"><span data-stu-id="a68dc-118">internalError</span></span>|<span data-ttu-id="a68dc-119">2</span><span class="sxs-lookup"><span data-stu-id="a68dc-119">2</span></span>|<span data-ttu-id="a68dc-120">Ein interner Fehler ist aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="a68dc-120">There was an internal error.</span></span>|
|<span data-ttu-id="a68dc-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="a68dc-121">expiredVppToken</span></span>|<span data-ttu-id="a68dc-122">3</span><span class="sxs-lookup"><span data-stu-id="a68dc-122">3</span></span>|<span data-ttu-id="a68dc-123">Ein Fehler aufgetreten, da das Token Apple Volume Purchase Program abgelaufen wurde.</span><span class="sxs-lookup"><span data-stu-id="a68dc-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="a68dc-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="a68dc-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="a68dc-125">4</span><span class="sxs-lookup"><span data-stu-id="a68dc-125">4</span></span>|<span data-ttu-id="a68dc-126">Ein Fehler aufgetreten, da das Apple Volume Purchase Programm Pushbenachrichtigung Zertifikat ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="a68dc-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|




