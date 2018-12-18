---
title: EducationOneRosterApiDataProvider-Ressource
description: Verwendet die Synchronisierung Schule Datenprofil einrichten, wenn die OneRoster-API als Eingabe Quelle verwendet wird.
author: mmast-msft
ms.openlocfilehash: 66c79c5e5d5ced4efcd635d2976e83887e545a9f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309569"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="7ad0f-103">EducationOneRosterApiDataProvider-Ressource</span><span class="sxs-lookup"><span data-stu-id="7ad0f-103">educationOneRosterApiDataProvider resource</span></span>

> <span data-ttu-id="7ad0f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7ad0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ad0f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ad0f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ad0f-106">Verwendet die Synchronisierung Schule Datenprofil einrichten, wenn die [OneRoster-API](https://www.imsglobal.org/activity/onerosterlis) als Eingabe Quelle verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="7ad0f-106">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="7ad0f-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="7ad0f-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7ad0f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7ad0f-108">Properties</span></span>

| <span data-ttu-id="7ad0f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7ad0f-109">Property</span></span> | <span data-ttu-id="7ad0f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="7ad0f-110">Type</span></span> | <span data-ttu-id="7ad0f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7ad0f-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7ad0f-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="7ad0f-112">**connectionUrl**</span></span> | <span data-ttu-id="7ad0f-113">String</span><span class="sxs-lookup"><span data-stu-id="7ad0f-113">String</span></span> | <span data-ttu-id="7ad0f-114">Die Verbindungs-URL für die OneRoster-Instanz.</span><span class="sxs-lookup"><span data-stu-id="7ad0f-114">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="7ad0f-115">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="7ad0f-115">**schoolsIds**</span></span> | <span data-ttu-id="7ad0f-116">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="7ad0f-116">String collection</span></span> |  <span data-ttu-id="7ad0f-117">Die Liste der Schule SourcedIds synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="7ad0f-117">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="7ad0f-118">**providerName**</span><span class="sxs-lookup"><span data-stu-id="7ad0f-118">**providerName**</span></span> | <span data-ttu-id="7ad0f-119">String</span><span class="sxs-lookup"><span data-stu-id="7ad0f-119">String</span></span> | <span data-ttu-id="7ad0f-120">Der Dienstanbieter OneRoster Name gemäß der [Spezifikation OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="7ad0f-120">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="7ad0f-121">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="7ad0f-121">**connectionSettings**</span></span> | [<span data-ttu-id="7ad0f-122">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="7ad0f-122">educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="7ad0f-123">Verbindungseinstellungen für die OneRoster-Instanz.</span><span class="sxs-lookup"><span data-stu-id="7ad0f-123">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="7ad0f-124">Muss vom Typ [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) oder [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)sein.</span><span class="sxs-lookup"><span data-stu-id="7ad0f-124">Should be of type [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="7ad0f-125">**Anpassungen**</span><span class="sxs-lookup"><span data-stu-id="7ad0f-125">**customizations**</span></span> | [<span data-ttu-id="7ad0f-126">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="7ad0f-126">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="7ad0f-127">Optional Anpassung der Synchronisierung Profil angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="7ad0f-127">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ad0f-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7ad0f-128">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
