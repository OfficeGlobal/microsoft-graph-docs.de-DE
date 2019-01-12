---
title: KeyStorageProviderOption Enum-Typ
description: Importoptionen für wichtige Speicher-Anbieter (KSP).
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f3a8169b4bb6cd2357f02aa7fec89ba640780f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946553"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="e4e6f-103">KeyStorageProviderOption Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e4e6f-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="e4e6f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4e6f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4e6f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4e6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4e6f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e4e6f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4e6f-107">Importoptionen für wichtige Speicher-Anbieter (KSP).</span><span class="sxs-lookup"><span data-stu-id="e4e6f-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="e4e6f-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="e4e6f-108">Members</span></span>
|<span data-ttu-id="e4e6f-109">Element</span><span class="sxs-lookup"><span data-stu-id="e4e6f-109">Member</span></span>|<span data-ttu-id="e4e6f-110">Wert</span><span class="sxs-lookup"><span data-stu-id="e4e6f-110">Value</span></span>|<span data-ttu-id="e4e6f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4e6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4e6f-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="e4e6f-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="e4e6f-113">0</span><span class="sxs-lookup"><span data-stu-id="e4e6f-113">0</span></span>|<span data-ttu-id="e4e6f-114">Importieren Sie um Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls in Software KSP importieren.</span><span class="sxs-lookup"><span data-stu-id="e4e6f-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="e4e6f-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="e4e6f-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="e4e6f-116">1</span><span class="sxs-lookup"><span data-stu-id="e4e6f-116">1</span></span>|<span data-ttu-id="e4e6f-117">Import auf Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="e4e6f-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="e4e6f-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="e4e6f-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="e4e6f-119">2</span><span class="sxs-lookup"><span data-stu-id="e4e6f-119">2</span></span>|<span data-ttu-id="e4e6f-120">Importieren von Passport für Arbeit KSP falls verfügbar, andernfalls ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="e4e6f-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="e4e6f-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="e4e6f-121">useSoftwareKsp</span></span>|<span data-ttu-id="e4e6f-122">3</span><span class="sxs-lookup"><span data-stu-id="e4e6f-122">3</span></span>|<span data-ttu-id="e4e6f-123">In Software KSP importieren.</span><span class="sxs-lookup"><span data-stu-id="e4e6f-123">Import to Software KSP.</span></span>|





