---
title: KeyStorageProviderOption Enum-Typ
description: Importoptionen für wichtige Speicher-Anbieter (KSP).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6993d7e241ef94c572975c709c286a14f6eabf5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424224"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="315c2-103">KeyStorageProviderOption Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="315c2-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="315c2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="315c2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="315c2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="315c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="315c2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="315c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="315c2-107">Importoptionen für wichtige Speicher-Anbieter (KSP).</span><span class="sxs-lookup"><span data-stu-id="315c2-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="315c2-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="315c2-108">Members</span></span>
|<span data-ttu-id="315c2-109">Member</span><span class="sxs-lookup"><span data-stu-id="315c2-109">Member</span></span>|<span data-ttu-id="315c2-110">Wert</span><span class="sxs-lookup"><span data-stu-id="315c2-110">Value</span></span>|<span data-ttu-id="315c2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="315c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="315c2-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="315c2-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="315c2-113">0</span><span class="sxs-lookup"><span data-stu-id="315c2-113">0</span></span>|<span data-ttu-id="315c2-114">Importieren Sie um Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls in Software KSP importieren.</span><span class="sxs-lookup"><span data-stu-id="315c2-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="315c2-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="315c2-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="315c2-116">1</span><span class="sxs-lookup"><span data-stu-id="315c2-116">1</span></span>|<span data-ttu-id="315c2-117">Import auf Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="315c2-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="315c2-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="315c2-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="315c2-119">2</span><span class="sxs-lookup"><span data-stu-id="315c2-119">2</span></span>|<span data-ttu-id="315c2-120">Importieren von Passport für Arbeit KSP falls verfügbar, andernfalls ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="315c2-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="315c2-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="315c2-121">useSoftwareKsp</span></span>|<span data-ttu-id="315c2-122">3</span><span class="sxs-lookup"><span data-stu-id="315c2-122">3</span></span>|<span data-ttu-id="315c2-123">In Software KSP importieren.</span><span class="sxs-lookup"><span data-stu-id="315c2-123">Import to Software KSP.</span></span>|




