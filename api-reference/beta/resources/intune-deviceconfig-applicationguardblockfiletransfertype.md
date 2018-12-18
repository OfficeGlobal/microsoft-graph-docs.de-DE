---
title: ApplicationGuardBlockFileTransferType Enum-Typ
description: Mögliche Werte für applicationGuardBlockFileTransfer
author: tfitzmac
ms.openlocfilehash: fe1be9b0ceaee5651302b041b6612515557d899e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347390"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="c0421-103">ApplicationGuardBlockFileTransferType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c0421-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="c0421-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0421-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0421-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0421-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0421-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c0421-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0421-107">Mögliche Werte für applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="c0421-107">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="c0421-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="c0421-108">Members</span></span>
|<span data-ttu-id="c0421-109">Member</span><span class="sxs-lookup"><span data-stu-id="c0421-109">Member</span></span>|<span data-ttu-id="c0421-110">Wert</span><span class="sxs-lookup"><span data-stu-id="c0421-110">Value</span></span>|<span data-ttu-id="c0421-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c0421-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0421-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="c0421-112">notConfigured</span></span>|<span data-ttu-id="c0421-113">0</span><span class="sxs-lookup"><span data-stu-id="c0421-113">0</span></span>|<span data-ttu-id="c0421-114">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="c0421-114">Not Configured</span></span>|
|<span data-ttu-id="c0421-115">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="c0421-115">blockImageAndTextFile</span></span>|<span data-ttu-id="c0421-116">1</span><span class="sxs-lookup"><span data-stu-id="c0421-116">1</span></span>|<span data-ttu-id="c0421-117">Blockieren der Zwischenablage zum Übertragen von Text und Bild-Datei</span><span class="sxs-lookup"><span data-stu-id="c0421-117">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="c0421-118">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="c0421-118">blockImageFile</span></span>|<span data-ttu-id="c0421-119">2</span><span class="sxs-lookup"><span data-stu-id="c0421-119">2</span></span>|<span data-ttu-id="c0421-120">Blockieren der Zwischenablage zum Übertragen Bilddatei</span><span class="sxs-lookup"><span data-stu-id="c0421-120">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="c0421-121">blockNone</span><span class="sxs-lookup"><span data-stu-id="c0421-121">blockNone</span></span>|<span data-ttu-id="c0421-122">3</span><span class="sxs-lookup"><span data-stu-id="c0421-122">3</span></span>|<span data-ttu-id="c0421-123">Keines der Textdatei oder Bilddatei wird übertragen blockiert</span><span class="sxs-lookup"><span data-stu-id="c0421-123">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="c0421-124">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="c0421-124">blockTextFile</span></span>|<span data-ttu-id="c0421-125">4</span><span class="sxs-lookup"><span data-stu-id="c0421-125">4</span></span>|<span data-ttu-id="c0421-126">Blockieren der Zwischenablage zum Übertragen von Textdatei</span><span class="sxs-lookup"><span data-stu-id="c0421-126">Block clipboard to transfer Text file</span></span>|





