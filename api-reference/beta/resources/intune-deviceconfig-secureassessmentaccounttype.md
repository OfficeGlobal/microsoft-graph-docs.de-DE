---
title: SecureAssessmentAccountType Enum-Typ
description: Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.
ms.openlocfilehash: 97dc60d8d15e90c43923d939cf957e1092b2cc45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064215"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="0f4ac-103">SecureAssessmentAccountType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="0f4ac-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="0f4ac-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f4ac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f4ac-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f4ac-107">Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>
## <a name="members"></a><span data-ttu-id="0f4ac-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="0f4ac-108">Members</span></span>
|<span data-ttu-id="0f4ac-109">Element</span><span class="sxs-lookup"><span data-stu-id="0f4ac-109">Member</span></span>|<span data-ttu-id="0f4ac-110">Wert</span><span class="sxs-lookup"><span data-stu-id="0f4ac-110">Value</span></span>|<span data-ttu-id="0f4ac-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f4ac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f4ac-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="0f4ac-112">azureADAccount</span></span>|<span data-ttu-id="0f4ac-113">0</span><span class="sxs-lookup"><span data-stu-id="0f4ac-113">0</span></span>|<span data-ttu-id="0f4ac-114">Gibt ein Azure AD-Konto im Format von AzureAD\ username@tenant.com an.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="0f4ac-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="0f4ac-115">domainAccount</span></span>|<span data-ttu-id="0f4ac-116">1</span><span class="sxs-lookup"><span data-stu-id="0f4ac-116">1</span></span>|<span data-ttu-id="0f4ac-117">Gibt ein Domänenkonto, das im Format Domäne\Benutzer oder user@domain.com an.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="0f4ac-118">localAccount</span><span class="sxs-lookup"><span data-stu-id="0f4ac-118">localAccount</span></span>|<span data-ttu-id="0f4ac-119">2</span><span class="sxs-lookup"><span data-stu-id="0f4ac-119">2</span></span>|<span data-ttu-id="0f4ac-120">Gibt ein lokales Konto im Username-Format an.</span><span class="sxs-lookup"><span data-stu-id="0f4ac-120">Indicates a local account in format of username.</span></span>|





