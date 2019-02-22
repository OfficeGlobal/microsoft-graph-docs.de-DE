---
title: keyStorageProviderOption-Enumerationstyp
description: Import Optionen des Schlüsselspeicheranbieters (KSP).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ddc1cffe1f4e6056d53a151a3b36b2622c9bf4b5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153018"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="ff307-103">keyStorageProviderOption-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="ff307-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="ff307-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff307-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff307-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ff307-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff307-106">Import Optionen des Schlüsselspeicheranbieters (KSP).</span><span class="sxs-lookup"><span data-stu-id="ff307-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="ff307-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="ff307-107">Members</span></span>
|<span data-ttu-id="ff307-108">Element</span><span class="sxs-lookup"><span data-stu-id="ff307-108">Member</span></span>|<span data-ttu-id="ff307-109">Wert</span><span class="sxs-lookup"><span data-stu-id="ff307-109">Value</span></span>|<span data-ttu-id="ff307-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff307-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff307-111">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="ff307-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="ff307-112">0</span><span class="sxs-lookup"><span data-stu-id="ff307-112">0</span></span>|<span data-ttu-id="ff307-113">Import in Trusted Platform Module (TPM) KSP, falls vorhanden, andernfalls in Software KSP importieren.</span><span class="sxs-lookup"><span data-stu-id="ff307-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="ff307-114">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="ff307-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="ff307-115">1</span><span class="sxs-lookup"><span data-stu-id="ff307-115">1</span></span>|<span data-ttu-id="ff307-116">Importieren Sie in Trusted Platform Module (TPM) KSP, falls vorhanden, andernfalls fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="ff307-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="ff307-117">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="ff307-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="ff307-118">2</span><span class="sxs-lookup"><span data-stu-id="ff307-118">2</span></span>|<span data-ttu-id="ff307-119">Import in Passport für Arbeit KSP, falls verfügbar, andernfalls fehlschlagen.</span><span class="sxs-lookup"><span data-stu-id="ff307-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="ff307-120">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="ff307-120">useSoftwareKsp</span></span>|<span data-ttu-id="ff307-121">3</span><span class="sxs-lookup"><span data-stu-id="ff307-121">3</span></span>|<span data-ttu-id="ff307-122">Importieren in Software KSP.</span><span class="sxs-lookup"><span data-stu-id="ff307-122">Import to Software KSP.</span></span>|




