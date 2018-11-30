---
title: KeyStorageProviderOption Enum-Typ
description: Importoptionen für wichtige Speicher-Anbieter (KSP).
ms.openlocfilehash: 236489d288ec0be70a818e1c51b8c634ad3933a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059042"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="1615c-103">KeyStorageProviderOption Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="1615c-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="1615c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1615c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1615c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1615c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1615c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1615c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1615c-107">Importoptionen für wichtige Speicher-Anbieter (KSP).</span><span class="sxs-lookup"><span data-stu-id="1615c-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="1615c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="1615c-108">Members</span></span>
|<span data-ttu-id="1615c-109">Element</span><span class="sxs-lookup"><span data-stu-id="1615c-109">Member</span></span>|<span data-ttu-id="1615c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="1615c-110">Value</span></span>|<span data-ttu-id="1615c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1615c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1615c-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="1615c-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="1615c-113">0</span><span class="sxs-lookup"><span data-stu-id="1615c-113">0</span></span>|<span data-ttu-id="1615c-114">Importieren Sie um Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls in Software KSP importieren.</span><span class="sxs-lookup"><span data-stu-id="1615c-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="1615c-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="1615c-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="1615c-116">1</span><span class="sxs-lookup"><span data-stu-id="1615c-116">1</span></span>|<span data-ttu-id="1615c-117">Import auf Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="1615c-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="1615c-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="1615c-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="1615c-119">2</span><span class="sxs-lookup"><span data-stu-id="1615c-119">2</span></span>|<span data-ttu-id="1615c-120">Importieren von Passport für Arbeit KSP falls verfügbar, andernfalls ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="1615c-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="1615c-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="1615c-121">useSoftwareKsp</span></span>|<span data-ttu-id="1615c-122">3</span><span class="sxs-lookup"><span data-stu-id="1615c-122">3</span></span>|<span data-ttu-id="1615c-123">In Software KSP importieren.</span><span class="sxs-lookup"><span data-stu-id="1615c-123">Import to Software KSP.</span></span>|





