---
title: Ressourcentyp educationIdentityCreationConfiguration
description: Definiert die Einstellungen, die bei der Erstellung der Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis erstellt werden.
ms.openlocfilehash: edbfa03bb574a1d8d9d4faaa2032ec82f6d20f66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065161"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="a6975-105">Ressourcentyp educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6975-105">educationIdentityCreationConfiguration resource type</span></span>

> <span data-ttu-id="a6975-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a6975-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6975-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6975-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6975-108">Definiert die Einstellungen, die bei der Erstellung der Schule Daten Profil Identitäten.</span><span class="sxs-lookup"><span data-stu-id="a6975-108">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="a6975-109">Diese Identitäten enthalten Schüler und Lehrer.</span><span class="sxs-lookup"><span data-stu-id="a6975-109">These identities include students and teachers.</span></span> <span data-ttu-id="a6975-110">Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="a6975-110">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="a6975-111">**Hinweis:** Wenn Sie die verzeichnissynchronisierung aktiviert die Synchronisierung zwischen der lokalen Active Directory und Azure Active Directory (AD Azure) haben, verwenden Sie stattdessen die [EducationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="a6975-111">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="a6975-112">[EducationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="a6975-112">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a6975-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a6975-113">Properties</span></span>

| <span data-ttu-id="a6975-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6975-114">Property</span></span> | <span data-ttu-id="a6975-115">Typ</span><span class="sxs-lookup"><span data-stu-id="a6975-115">Type</span></span> | <span data-ttu-id="a6975-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6975-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a6975-117">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="a6975-117">**userDomains**</span></span> | <span data-ttu-id="a6975-118">[EducationIdentityDomain](educationidentitydomain.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a6975-118">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="a6975-119">Stellt die Liste der Domänen pro Benutzertyp verwenden.</span><span class="sxs-lookup"><span data-stu-id="a6975-119">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="a6975-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a6975-120">JSON representation</span></span>
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