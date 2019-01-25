---
title: EducationOneRosterApiDataProvider-Ressource
description: Verwendet die Synchronisierung Schule Datenprofil einrichten, wenn die OneRoster-API als Eingabe Quelle verwendet wird.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 55a3cd0e20f15c4b7d44bc7aebdc19f202e044f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527983"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="5f375-103">EducationOneRosterApiDataProvider-Ressource</span><span class="sxs-lookup"><span data-stu-id="5f375-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f375-104">Verwendet die Synchronisierung Schule Datenprofil einrichten, wenn die [OneRoster-API](https://www.imsglobal.org/activity/onerosterlis) als Eingabe Quelle verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="5f375-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="5f375-105">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="5f375-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5f375-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5f375-106">Properties</span></span>

| <span data-ttu-id="5f375-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f375-107">Property</span></span> | <span data-ttu-id="5f375-108">Typ</span><span class="sxs-lookup"><span data-stu-id="5f375-108">Type</span></span> | <span data-ttu-id="5f375-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f375-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5f375-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="5f375-110">**connectionUrl**</span></span> | <span data-ttu-id="5f375-111">String</span><span class="sxs-lookup"><span data-stu-id="5f375-111">String</span></span> | <span data-ttu-id="5f375-112">Die Verbindungs-URL für die OneRoster-Instanz.</span><span class="sxs-lookup"><span data-stu-id="5f375-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="5f375-113">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="5f375-113">**schoolsIds**</span></span> | <span data-ttu-id="5f375-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="5f375-114">String collection</span></span> |  <span data-ttu-id="5f375-115">Die Liste der Schule SourcedIds synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="5f375-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="5f375-116">ProviderName</span><span class="sxs-lookup"><span data-stu-id="5f375-116">**providerName**</span></span> | <span data-ttu-id="5f375-117">String</span><span class="sxs-lookup"><span data-stu-id="5f375-117">String</span></span> | <span data-ttu-id="5f375-118">Der Dienstanbieter OneRoster Name gemäß der [Spezifikation OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="5f375-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="5f375-119">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="5f375-119">**connectionSettings**</span></span> | [<span data-ttu-id="5f375-120">microsoft.graph.educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="5f375-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="5f375-121">Verbindungseinstellungen für die OneRoster-Instanz.</span><span class="sxs-lookup"><span data-stu-id="5f375-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="5f375-122">Muss vom Typ [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) oder [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)sein.</span><span class="sxs-lookup"><span data-stu-id="5f375-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="5f375-123">**Anpassungen**</span><span class="sxs-lookup"><span data-stu-id="5f375-123">**customizations**</span></span> | [<span data-ttu-id="5f375-124">microsoft.graph.educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="5f375-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="5f375-125">Optional Anpassung der Synchronisierung Profil angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5f375-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f375-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5f375-126">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonerosterapidataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
