---
title: SecureAssessmentAccountType Enum-Typ
description: Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b1f8a3d03c0e7b9e91c68ff5a87611fcaa6f31e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826054"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="61b97-103">SecureAssessmentAccountType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="61b97-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="61b97-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="61b97-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61b97-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61b97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61b97-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="61b97-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61b97-107">Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="61b97-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>
## <a name="members"></a><span data-ttu-id="61b97-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="61b97-108">Members</span></span>
|<span data-ttu-id="61b97-109">Element</span><span class="sxs-lookup"><span data-stu-id="61b97-109">Member</span></span>|<span data-ttu-id="61b97-110">Wert</span><span class="sxs-lookup"><span data-stu-id="61b97-110">Value</span></span>|<span data-ttu-id="61b97-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61b97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61b97-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="61b97-112">azureADAccount</span></span>|<span data-ttu-id="61b97-113">0</span><span class="sxs-lookup"><span data-stu-id="61b97-113">0</span></span>|<span data-ttu-id="61b97-114">Gibt ein Azure AD-Konto im Format von AzureAD\ username@tenant.com an.</span><span class="sxs-lookup"><span data-stu-id="61b97-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="61b97-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="61b97-115">domainAccount</span></span>|<span data-ttu-id="61b97-116">1</span><span class="sxs-lookup"><span data-stu-id="61b97-116">1</span></span>|<span data-ttu-id="61b97-117">Gibt ein Domänenkonto, das im Format Domäne\Benutzer oder user@domain.com an.</span><span class="sxs-lookup"><span data-stu-id="61b97-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="61b97-118">localAccount</span><span class="sxs-lookup"><span data-stu-id="61b97-118">localAccount</span></span>|<span data-ttu-id="61b97-119">2</span><span class="sxs-lookup"><span data-stu-id="61b97-119">2</span></span>|<span data-ttu-id="61b97-120">Gibt ein lokales Konto im Username-Format an.</span><span class="sxs-lookup"><span data-stu-id="61b97-120">Indicates a local account in format of username.</span></span>|





