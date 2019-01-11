---
title: Ressourcentyp educationIdentitySynchronizationConfiguration
description: Abstrakte Basisklasse für alle Schule Daten Profil Identität Synchronisierung Konfigurationen. Abgeleiteten Klassen definieren Sie das Verhalten für das Synchronisieren von Identitäten. Im folgenden werden die abgeleiteten Typen.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: c04233dd7f0383d238f0a7e7245e9451fb764be6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869062"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="8acd9-105">Ressourcentyp educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8acd9-105">educationIdentitySynchronizationConfiguration resource type</span></span>

> <span data-ttu-id="8acd9-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8acd9-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8acd9-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8acd9-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8acd9-108">Abstrakte Basisklasse für alle Schule Daten Profil Identität Synchronisierung Konfigurationen.</span><span class="sxs-lookup"><span data-stu-id="8acd9-108">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="8acd9-109">Abgeleiteten Klassen definieren Sie das Verhalten für das Synchronisieren von Identitäten.</span><span class="sxs-lookup"><span data-stu-id="8acd9-109">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="8acd9-110">Im folgenden werden die abgeleiteten Typen.</span><span class="sxs-lookup"><span data-stu-id="8acd9-110">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="8acd9-111">Abgeleitete Typen</span><span class="sxs-lookup"><span data-stu-id="8acd9-111">Derived types</span></span>
| <span data-ttu-id="8acd9-112">Typ</span><span class="sxs-lookup"><span data-stu-id="8acd9-112">Type</span></span> | <span data-ttu-id="8acd9-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8acd9-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="8acd9-114">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="8acd9-114">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="8acd9-115">Verwenden Sie diesen Typ zu vorhandenen Benutzerkonten in Azure Active Directory (AD Azure) übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="8acd9-115">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="8acd9-116">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="8acd9-116">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="8acd9-117">Verwenden Sie diesen Typ in Azure Active Directory neue Benutzerkonten erstellen.</span><span class="sxs-lookup"><span data-stu-id="8acd9-117">Use this type to create new user accounts in Azure AD.</span></span> |
