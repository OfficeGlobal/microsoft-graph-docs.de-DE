---
title: FileHashType-Enumeration
description: Enum für Hash Dateitypen.
localization_priority: Normal
ms.openlocfilehash: e1c31aaea6c8cea40817efea61dc8654d3d17fae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816331"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="87307-103">FileHashType-Enumeration</span><span class="sxs-lookup"><span data-stu-id="87307-103">fileHashType enum</span></span>

> <span data-ttu-id="87307-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87307-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87307-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87307-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87307-106">Enum für Hash Dateitypen.</span><span class="sxs-lookup"><span data-stu-id="87307-106">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="87307-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="87307-107">Members</span></span>

|<span data-ttu-id="87307-108">Element</span><span class="sxs-lookup"><span data-stu-id="87307-108">Member</span></span>|<span data-ttu-id="87307-109">Wert</span><span class="sxs-lookup"><span data-stu-id="87307-109">Value</span></span>|<span data-ttu-id="87307-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87307-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87307-111">unknown</span><span class="sxs-lookup"><span data-stu-id="87307-111">unknown</span></span>|<span data-ttu-id="87307-112">0</span><span class="sxs-lookup"><span data-stu-id="87307-112">0</span></span>|<span data-ttu-id="87307-113">Unbekannten Typs.</span><span class="sxs-lookup"><span data-stu-id="87307-113">Unknown type.</span></span>|
|<span data-ttu-id="87307-114">SHA1</span><span class="sxs-lookup"><span data-stu-id="87307-114">sha1</span></span>|<span data-ttu-id="87307-115">1</span><span class="sxs-lookup"><span data-stu-id="87307-115">1</span></span>|<span data-ttu-id="87307-116">SHA1 Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="87307-116">SHA1 hash type.</span></span>|
|<span data-ttu-id="87307-117">SHA256</span><span class="sxs-lookup"><span data-stu-id="87307-117">sha256</span></span>|<span data-ttu-id="87307-118">2</span><span class="sxs-lookup"><span data-stu-id="87307-118">2</span></span>| <span data-ttu-id="87307-119">SHA256-Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="87307-119">SHA256 hash type.</span></span>|
|<span data-ttu-id="87307-120">MD5</span><span class="sxs-lookup"><span data-stu-id="87307-120">md5</span></span>|<span data-ttu-id="87307-121">3</span><span class="sxs-lookup"><span data-stu-id="87307-121">3</span></span>| <span data-ttu-id="87307-122">MD5 Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="87307-122">MD5 hash type.</span></span>|
|<span data-ttu-id="87307-123">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="87307-123">authenticodeHash256</span></span>|<span data-ttu-id="87307-124">4</span><span class="sxs-lookup"><span data-stu-id="87307-124">4</span></span>| <span data-ttu-id="87307-125">AuthenticodeHash256 Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="87307-125">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="87307-126">lsHash</span><span class="sxs-lookup"><span data-stu-id="87307-126">lsHash</span></span>|<span data-ttu-id="87307-127">5</span><span class="sxs-lookup"><span data-stu-id="87307-127">5</span></span>| <span data-ttu-id="87307-128">LsHash Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="87307-128">LsHash hash type.</span></span>|
|<span data-ttu-id="87307-129">ctph</span><span class="sxs-lookup"><span data-stu-id="87307-129">ctph</span></span>|<span data-ttu-id="87307-130">6</span><span class="sxs-lookup"><span data-stu-id="87307-130">6</span></span>| <span data-ttu-id="87307-131">CTPH Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="87307-131">CTPH hash type.</span></span>|
|<span data-ttu-id="87307-132">peSha1</span><span class="sxs-lookup"><span data-stu-id="87307-132">peSha1</span></span>|<span data-ttu-id="87307-133">7</span><span class="sxs-lookup"><span data-stu-id="87307-133">7</span></span>| <span data-ttu-id="87307-134">PESHA1 Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="87307-134">PESHA1 hash type.</span></span>|
|<span data-ttu-id="87307-135">peSha256</span><span class="sxs-lookup"><span data-stu-id="87307-135">peSha256</span></span>|<span data-ttu-id="87307-136">8</span><span class="sxs-lookup"><span data-stu-id="87307-136">8</span></span>| <span data-ttu-id="87307-137">PESHA256 Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="87307-137">PESHA256 hash type.</span></span>|
