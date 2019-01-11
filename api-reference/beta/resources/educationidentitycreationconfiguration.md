---
title: Ressourcentyp educationIdentityCreationConfiguration
description: Definiert die Einstellungen, die bei der Erstellung der Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis erstellt werden.
localization_priority: Normal
ms.openlocfilehash: 86624c7203dc6425372556572c40efda2bc1a53f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858863"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="0ccc7-105">Ressourcentyp educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ccc7-105">educationIdentityCreationConfiguration resource type</span></span>

> <span data-ttu-id="0ccc7-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0ccc7-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ccc7-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ccc7-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ccc7-108">Definiert die Einstellungen, die bei der Erstellung der Schule Daten Profil Identitäten.</span><span class="sxs-lookup"><span data-stu-id="0ccc7-108">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="0ccc7-109">Diese Identitäten enthalten Schüler und Lehrer.</span><span class="sxs-lookup"><span data-stu-id="0ccc7-109">These identities include students and teachers.</span></span> <span data-ttu-id="0ccc7-110">Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="0ccc7-110">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="0ccc7-111">**Hinweis:** Wenn Sie die verzeichnissynchronisierung aktiviert die Synchronisierung zwischen der lokalen Active Directory und Azure Active Directory (AD Azure) haben, verwenden Sie stattdessen die [EducationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="0ccc7-111">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="0ccc7-112">[EducationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="0ccc7-112">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0ccc7-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0ccc7-113">Properties</span></span>

| <span data-ttu-id="0ccc7-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0ccc7-114">Property</span></span> | <span data-ttu-id="0ccc7-115">Typ</span><span class="sxs-lookup"><span data-stu-id="0ccc7-115">Type</span></span> | <span data-ttu-id="0ccc7-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ccc7-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0ccc7-117">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="0ccc7-117">**userDomains**</span></span> | <span data-ttu-id="0ccc7-118">[EducationIdentityDomain](educationidentitydomain.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="0ccc7-118">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="0ccc7-119">Stellt die Liste der Domänen pro Benutzertyp verwenden.</span><span class="sxs-lookup"><span data-stu-id="0ccc7-119">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="0ccc7-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0ccc7-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
