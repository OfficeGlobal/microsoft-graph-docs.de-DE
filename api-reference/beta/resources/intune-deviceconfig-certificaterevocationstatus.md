---
title: CertificateRevocationStatus Enum-Typ
description: Status der Zertifikatsperre.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 373cb6247a695a5912d02d4fb1a353c40aeac581
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421970"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="c41fe-103">CertificateRevocationStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c41fe-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="c41fe-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c41fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c41fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c41fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c41fe-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c41fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c41fe-107">Status der Zertifikatsperre.</span><span class="sxs-lookup"><span data-stu-id="c41fe-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="c41fe-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="c41fe-108">Members</span></span>
|<span data-ttu-id="c41fe-109">Member</span><span class="sxs-lookup"><span data-stu-id="c41fe-109">Member</span></span>|<span data-ttu-id="c41fe-110">Wert</span><span class="sxs-lookup"><span data-stu-id="c41fe-110">Value</span></span>|<span data-ttu-id="c41fe-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c41fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c41fe-112">Keine</span><span class="sxs-lookup"><span data-stu-id="c41fe-112">none</span></span>|<span data-ttu-id="c41fe-113">0</span><span class="sxs-lookup"><span data-stu-id="c41fe-113">0</span></span>|<span data-ttu-id="c41fe-114">Nicht gesperrt.</span><span class="sxs-lookup"><span data-stu-id="c41fe-114">Not revoked.</span></span>|
|<span data-ttu-id="c41fe-115">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="c41fe-115">pending</span></span>|<span data-ttu-id="c41fe-116">1</span><span class="sxs-lookup"><span data-stu-id="c41fe-116">1</span></span>|<span data-ttu-id="c41fe-117">OCSP ausstehende.</span><span class="sxs-lookup"><span data-stu-id="c41fe-117">Revocation pending.</span></span>|
|<span data-ttu-id="c41fe-118">ausgestellt</span><span class="sxs-lookup"><span data-stu-id="c41fe-118">issued</span></span>|<span data-ttu-id="c41fe-119">2</span><span class="sxs-lookup"><span data-stu-id="c41fe-119">2</span></span>|<span data-ttu-id="c41fe-120">OCSP-Befehl ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="c41fe-120">Revocation command issued.</span></span>|
|<span data-ttu-id="c41fe-121">failed</span><span class="sxs-lookup"><span data-stu-id="c41fe-121">failed</span></span>|<span data-ttu-id="c41fe-122">3</span><span class="sxs-lookup"><span data-stu-id="c41fe-122">3</span></span>|<span data-ttu-id="c41fe-123">OCSP ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="c41fe-123">Revocation failed.</span></span>|
|<span data-ttu-id="c41fe-124">widerrufen</span><span class="sxs-lookup"><span data-stu-id="c41fe-124">revoked</span></span>|<span data-ttu-id="c41fe-125">4</span><span class="sxs-lookup"><span data-stu-id="c41fe-125">4</span></span>|<span data-ttu-id="c41fe-126">Widerrufen.</span><span class="sxs-lookup"><span data-stu-id="c41fe-126">Revoked.</span></span>|




