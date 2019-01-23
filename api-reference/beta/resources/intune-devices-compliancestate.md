---
title: ComplianceState Enum-Typ
description: Compliance-Zustand.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 04f77da451970a302dbf249e8820aa5a2a8f0ebc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392738"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="72e0d-103">ComplianceState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="72e0d-103">complianceState enum type</span></span>

> <span data-ttu-id="72e0d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="72e0d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="72e0d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="72e0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72e0d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="72e0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72e0d-107">Compliance-Zustand.</span><span class="sxs-lookup"><span data-stu-id="72e0d-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="72e0d-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="72e0d-108">Members</span></span>
|<span data-ttu-id="72e0d-109">Member</span><span class="sxs-lookup"><span data-stu-id="72e0d-109">Member</span></span>|<span data-ttu-id="72e0d-110">Wert</span><span class="sxs-lookup"><span data-stu-id="72e0d-110">Value</span></span>|<span data-ttu-id="72e0d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72e0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72e0d-112">unknown</span><span class="sxs-lookup"><span data-stu-id="72e0d-112">unknown</span></span>|<span data-ttu-id="72e0d-113">0</span><span class="sxs-lookup"><span data-stu-id="72e0d-113">0</span></span>|<span data-ttu-id="72e0d-114">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="72e0d-114">Unknown.</span></span>|
|<span data-ttu-id="72e0d-115">kompatible</span><span class="sxs-lookup"><span data-stu-id="72e0d-115">compliant</span></span>|<span data-ttu-id="72e0d-116">1</span><span class="sxs-lookup"><span data-stu-id="72e0d-116">1</span></span>|<span data-ttu-id="72e0d-117">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="72e0d-117">Compliant.</span></span>|
|<span data-ttu-id="72e0d-118">nicht konformer</span><span class="sxs-lookup"><span data-stu-id="72e0d-118">noncompliant</span></span>|<span data-ttu-id="72e0d-119">2</span><span class="sxs-lookup"><span data-stu-id="72e0d-119">2</span></span>|<span data-ttu-id="72e0d-120">Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="72e0d-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="72e0d-121">Konflikt</span><span class="sxs-lookup"><span data-stu-id="72e0d-121">conflict</span></span>|<span data-ttu-id="72e0d-122">3</span><span class="sxs-lookup"><span data-stu-id="72e0d-122">3</span></span>|<span data-ttu-id="72e0d-123">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="72e0d-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="72e0d-124">error</span><span class="sxs-lookup"><span data-stu-id="72e0d-124">error</span></span>|<span data-ttu-id="72e0d-125">4</span><span class="sxs-lookup"><span data-stu-id="72e0d-125">4</span></span>|<span data-ttu-id="72e0d-126">Fehler</span><span class="sxs-lookup"><span data-stu-id="72e0d-126">Error.</span></span>|
|<span data-ttu-id="72e0d-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="72e0d-127">inGracePeriod</span></span>|<span data-ttu-id="72e0d-128">254</span><span class="sxs-lookup"><span data-stu-id="72e0d-128">254</span></span>|<span data-ttu-id="72e0d-129">Gerät nicht kompatibel ist, aber dennoch hat Zugriff auf Unternehmensressourcen</span><span class="sxs-lookup"><span data-stu-id="72e0d-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="72e0d-130">configManager</span><span class="sxs-lookup"><span data-stu-id="72e0d-130">configManager</span></span>|<span data-ttu-id="72e0d-131">255</span><span class="sxs-lookup"><span data-stu-id="72e0d-131">255</span></span>|<span data-ttu-id="72e0d-132">Vom Konfigurations-Manager verwaltet</span><span class="sxs-lookup"><span data-stu-id="72e0d-132">Managed by Config Manager</span></span>|




