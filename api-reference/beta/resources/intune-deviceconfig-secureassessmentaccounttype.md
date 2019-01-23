---
title: SecureAssessmentAccountType Enum-Typ
description: Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f9e620f87173708b852bd7eac79bee5a45e432c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409881"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="b6da5-103">SecureAssessmentAccountType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b6da5-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="b6da5-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b6da5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6da5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6da5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6da5-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b6da5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6da5-107">Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="b6da5-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="b6da5-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b6da5-108">Members</span></span>
|<span data-ttu-id="b6da5-109">Member</span><span class="sxs-lookup"><span data-stu-id="b6da5-109">Member</span></span>|<span data-ttu-id="b6da5-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b6da5-110">Value</span></span>|<span data-ttu-id="b6da5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6da5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6da5-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="b6da5-112">azureADAccount</span></span>|<span data-ttu-id="b6da5-113">0</span><span class="sxs-lookup"><span data-stu-id="b6da5-113">0</span></span>|<span data-ttu-id="b6da5-114">Gibt ein Azure AD-Konto im Format von AzureAD\ username@tenant.com an.</span><span class="sxs-lookup"><span data-stu-id="b6da5-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="b6da5-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="b6da5-115">domainAccount</span></span>|<span data-ttu-id="b6da5-116">1</span><span class="sxs-lookup"><span data-stu-id="b6da5-116">1</span></span>|<span data-ttu-id="b6da5-117">Gibt ein Domänenkonto, das im Format Domäne\Benutzer oder user@domain.com an.</span><span class="sxs-lookup"><span data-stu-id="b6da5-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="b6da5-118">localAccount</span><span class="sxs-lookup"><span data-stu-id="b6da5-118">localAccount</span></span>|<span data-ttu-id="b6da5-119">2</span><span class="sxs-lookup"><span data-stu-id="b6da5-119">2</span></span>|<span data-ttu-id="b6da5-120">Gibt ein lokales Konto im Username-Format an.</span><span class="sxs-lookup"><span data-stu-id="b6da5-120">Indicates a local account in format of username.</span></span>|




