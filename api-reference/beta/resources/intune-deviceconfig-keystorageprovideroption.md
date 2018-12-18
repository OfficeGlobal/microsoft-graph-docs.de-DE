---
title: KeyStorageProviderOption Enum-Typ
description: Importoptionen für wichtige Speicher-Anbieter (KSP).
author: tfitzmac
ms.openlocfilehash: 7923dd5c4b8a09d834d29b65928430828f3dafac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342217"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="f6d43-103">KeyStorageProviderOption Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="f6d43-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="f6d43-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f6d43-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6d43-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6d43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6d43-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f6d43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6d43-107">Importoptionen für wichtige Speicher-Anbieter (KSP).</span><span class="sxs-lookup"><span data-stu-id="f6d43-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="f6d43-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="f6d43-108">Members</span></span>
|<span data-ttu-id="f6d43-109">Member</span><span class="sxs-lookup"><span data-stu-id="f6d43-109">Member</span></span>|<span data-ttu-id="f6d43-110">Wert</span><span class="sxs-lookup"><span data-stu-id="f6d43-110">Value</span></span>|<span data-ttu-id="f6d43-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6d43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d43-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="f6d43-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="f6d43-113">0</span><span class="sxs-lookup"><span data-stu-id="f6d43-113">0</span></span>|<span data-ttu-id="f6d43-114">Importieren Sie um Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls in Software KSP importieren.</span><span class="sxs-lookup"><span data-stu-id="f6d43-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="f6d43-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="f6d43-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="f6d43-116">1</span><span class="sxs-lookup"><span data-stu-id="f6d43-116">1</span></span>|<span data-ttu-id="f6d43-117">Import auf Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="f6d43-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="f6d43-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="f6d43-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="f6d43-119">2</span><span class="sxs-lookup"><span data-stu-id="f6d43-119">2</span></span>|<span data-ttu-id="f6d43-120">Importieren von Passport für Arbeit KSP falls verfügbar, andernfalls ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="f6d43-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="f6d43-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="f6d43-121">useSoftwareKsp</span></span>|<span data-ttu-id="f6d43-122">3</span><span class="sxs-lookup"><span data-stu-id="f6d43-122">3</span></span>|<span data-ttu-id="f6d43-123">In Software KSP importieren.</span><span class="sxs-lookup"><span data-stu-id="f6d43-123">Import to Software KSP.</span></span>|





