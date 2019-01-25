---
title: Ressourcentyp educationIdentityCreationConfiguration
description: Definiert die Einstellungen, die bei der Erstellung der Schule Daten Profil Identitäten. Diese Identitäten enthalten Schüler und Lehrer. Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis erstellt werden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 92ad3c36a9379bb570f2a635038903e64a0309e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511401"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="7cef0-105">Ressourcentyp educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7cef0-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cef0-106">Definiert die Einstellungen, die bei der Erstellung der Schule Daten Profil Identitäten.</span><span class="sxs-lookup"><span data-stu-id="7cef0-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="7cef0-107">Diese Identitäten enthalten Schüler und Lehrer.</span><span class="sxs-lookup"><span data-stu-id="7cef0-107">These identities include students and teachers.</span></span> <span data-ttu-id="7cef0-108">Basierend auf diese Einstellungen, werden die Benutzer im Verzeichnis erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="7cef0-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="7cef0-109">**Hinweis:** Wenn Sie die verzeichnissynchronisierung aktiviert die Synchronisierung zwischen der lokalen Active Directory und Azure Active Directory (AD Azure) haben, verwenden Sie stattdessen die [EducationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="7cef0-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="7cef0-110">[EducationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="7cef0-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7cef0-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7cef0-111">Properties</span></span>

| <span data-ttu-id="7cef0-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7cef0-112">Property</span></span> | <span data-ttu-id="7cef0-113">Typ</span><span class="sxs-lookup"><span data-stu-id="7cef0-113">Type</span></span> | <span data-ttu-id="7cef0-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7cef0-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7cef0-115">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="7cef0-115">**userDomains**</span></span> | <span data-ttu-id="7cef0-116">[EducationIdentityDomain](educationidentitydomain.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7cef0-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="7cef0-117">Stellt die Liste der Domänen pro Benutzertyp verwenden.</span><span class="sxs-lookup"><span data-stu-id="7cef0-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="7cef0-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7cef0-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitycreationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
