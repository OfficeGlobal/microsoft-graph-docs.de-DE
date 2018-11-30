---
title: FileHashType-Enumeration
description: Enum für Hash Dateitypen.
ms.openlocfilehash: fbaa390ee8c543d2ed7c77cc05a11b519df0da9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058839"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="1a982-103">FileHashType-Enumeration</span><span class="sxs-lookup"><span data-stu-id="1a982-103">fileHashType enum</span></span>

> <span data-ttu-id="1a982-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1a982-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a982-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a982-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a982-106">Enum für Hash Dateitypen.</span><span class="sxs-lookup"><span data-stu-id="1a982-106">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="1a982-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="1a982-107">Members</span></span>

|<span data-ttu-id="1a982-108">Element</span><span class="sxs-lookup"><span data-stu-id="1a982-108">Member</span></span>|<span data-ttu-id="1a982-109">Wert</span><span class="sxs-lookup"><span data-stu-id="1a982-109">Value</span></span>|<span data-ttu-id="1a982-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a982-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a982-111">unknown</span><span class="sxs-lookup"><span data-stu-id="1a982-111">unknown</span></span>|<span data-ttu-id="1a982-112">0</span><span class="sxs-lookup"><span data-stu-id="1a982-112">0</span></span>|<span data-ttu-id="1a982-113">Unbekannten Typs.</span><span class="sxs-lookup"><span data-stu-id="1a982-113">Unknown type.</span></span>|
|<span data-ttu-id="1a982-114">SHA1</span><span class="sxs-lookup"><span data-stu-id="1a982-114">sha1</span></span>|<span data-ttu-id="1a982-115">1</span><span class="sxs-lookup"><span data-stu-id="1a982-115">1</span></span>|<span data-ttu-id="1a982-116">SHA1 Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="1a982-116">SHA1 hash type.</span></span>|
|<span data-ttu-id="1a982-117">SHA256</span><span class="sxs-lookup"><span data-stu-id="1a982-117">sha256</span></span>|<span data-ttu-id="1a982-118">2</span><span class="sxs-lookup"><span data-stu-id="1a982-118">2</span></span>| <span data-ttu-id="1a982-119">SHA256-Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="1a982-119">SHA256 hash type.</span></span>|
|<span data-ttu-id="1a982-120">MD5</span><span class="sxs-lookup"><span data-stu-id="1a982-120">md5</span></span>|<span data-ttu-id="1a982-121">3</span><span class="sxs-lookup"><span data-stu-id="1a982-121">3</span></span>| <span data-ttu-id="1a982-122">MD5 Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="1a982-122">MD5 hash type.</span></span>|
|<span data-ttu-id="1a982-123">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="1a982-123">authenticodeHash256</span></span>|<span data-ttu-id="1a982-124">4</span><span class="sxs-lookup"><span data-stu-id="1a982-124">4</span></span>| <span data-ttu-id="1a982-125">AuthenticodeHash256 Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="1a982-125">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="1a982-126">lsHash</span><span class="sxs-lookup"><span data-stu-id="1a982-126">lsHash</span></span>|<span data-ttu-id="1a982-127">5</span><span class="sxs-lookup"><span data-stu-id="1a982-127">5</span></span>| <span data-ttu-id="1a982-128">LsHash Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="1a982-128">LsHash hash type.</span></span>|
|<span data-ttu-id="1a982-129">ctph</span><span class="sxs-lookup"><span data-stu-id="1a982-129">ctph</span></span>|<span data-ttu-id="1a982-130">6</span><span class="sxs-lookup"><span data-stu-id="1a982-130">6</span></span>| <span data-ttu-id="1a982-131">CTPH Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="1a982-131">CTPH hash type.</span></span>|
|<span data-ttu-id="1a982-132">peSha1</span><span class="sxs-lookup"><span data-stu-id="1a982-132">peSha1</span></span>|<span data-ttu-id="1a982-133">7</span><span class="sxs-lookup"><span data-stu-id="1a982-133">7</span></span>| <span data-ttu-id="1a982-134">PESHA1 Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="1a982-134">PESHA1 hash type.</span></span>|
|<span data-ttu-id="1a982-135">peSha256</span><span class="sxs-lookup"><span data-stu-id="1a982-135">peSha256</span></span>|<span data-ttu-id="1a982-136">8</span><span class="sxs-lookup"><span data-stu-id="1a982-136">8</span></span>| <span data-ttu-id="1a982-137">PESHA256 Hash-Typ.</span><span class="sxs-lookup"><span data-stu-id="1a982-137">PESHA256 hash type.</span></span>|
