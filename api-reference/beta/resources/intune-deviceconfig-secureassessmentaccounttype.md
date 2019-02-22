---
title: secureAssessmentAccountType-Enumerationstyp
description: Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6698086b3da16466e9069781312e15ccd7c80c3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169377"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="8074b-103">secureAssessmentAccountType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="8074b-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="8074b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8074b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8074b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8074b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8074b-106">Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="8074b-106">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="8074b-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="8074b-107">Members</span></span>
|<span data-ttu-id="8074b-108">Element</span><span class="sxs-lookup"><span data-stu-id="8074b-108">Member</span></span>|<span data-ttu-id="8074b-109">Wert</span><span class="sxs-lookup"><span data-stu-id="8074b-109">Value</span></span>|<span data-ttu-id="8074b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8074b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8074b-111">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="8074b-111">azureADAccount</span></span>|<span data-ttu-id="8074b-112">0</span><span class="sxs-lookup"><span data-stu-id="8074b-112">0</span></span>|<span data-ttu-id="8074b-113">Gibt ein Azure AD-Konto im Format AzureAD\username@tenant.com an.</span><span class="sxs-lookup"><span data-stu-id="8074b-113">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="8074b-114">domainAccount</span><span class="sxs-lookup"><span data-stu-id="8074b-114">domainAccount</span></span>|<span data-ttu-id="8074b-115">1</span><span class="sxs-lookup"><span data-stu-id="8074b-115">1</span></span>|<span data-ttu-id="8074b-116">Gibt ein Domänenkonto im Format Domäne \ Benutzer oder user@domain.com an.</span><span class="sxs-lookup"><span data-stu-id="8074b-116">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="8074b-117">localAccount</span><span class="sxs-lookup"><span data-stu-id="8074b-117">localAccount</span></span>|<span data-ttu-id="8074b-118">2</span><span class="sxs-lookup"><span data-stu-id="8074b-118">2</span></span>|<span data-ttu-id="8074b-119">Gibt ein lokales Konto im Format des Benutzernamens an.</span><span class="sxs-lookup"><span data-stu-id="8074b-119">Indicates a local account in format of username.</span></span>|




