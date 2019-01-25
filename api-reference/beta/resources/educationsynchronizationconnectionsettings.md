---
title: Ressourcentyp educationSynchronizationConnectionSettings
description: 'Stellt die Einstellungen für die Anbieter-Verbindung dar. Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f6af6851e1e9d327b05c9ca1c7ed5929335a6e17
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526865"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="28550-104">Ressourcentyp educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="28550-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28550-105">Stellt die Einstellungen für die Anbieter-Verbindung dar.</span><span class="sxs-lookup"><span data-stu-id="28550-105">Represents the provider connection settings.</span></span> <span data-ttu-id="28550-106">Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden.</span><span class="sxs-lookup"><span data-stu-id="28550-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="28550-107">**Hinweis:** Dieser komplexe Typ ist abstrakt.</span><span class="sxs-lookup"><span data-stu-id="28550-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="28550-108">Verweisen Sie auf die bestimmten Arten von Verbindungseinstellungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="28550-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="28550-109">Abgeleitete Typen</span><span class="sxs-lookup"><span data-stu-id="28550-109">Derived types</span></span>
| <span data-ttu-id="28550-110">Typ</span><span class="sxs-lookup"><span data-stu-id="28550-110">Type</span></span> | <span data-ttu-id="28550-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28550-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="28550-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="28550-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="28550-113">Verwenden Sie diesen Typ OAuth1 Verbindungseinstellungen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="28550-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="28550-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="28550-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="28550-115">Verwenden Sie diesen Typ OAuth2 Client Anmeldeinformationen Grant-Verbindungseinstellungen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="28550-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="28550-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="28550-116">Properties</span></span>

| <span data-ttu-id="28550-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28550-117">Property</span></span> | <span data-ttu-id="28550-118">Typ</span><span class="sxs-lookup"><span data-stu-id="28550-118">Type</span></span> | <span data-ttu-id="28550-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28550-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="28550-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="28550-120">**clientId**</span></span> | <span data-ttu-id="28550-121">String</span><span class="sxs-lookup"><span data-stu-id="28550-121">String</span></span> |  <span data-ttu-id="28550-122">Client-ID für die Verbindung an den Anbieter verwendet.</span><span class="sxs-lookup"><span data-stu-id="28550-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="28550-123">client_secret</span><span class="sxs-lookup"><span data-stu-id="28550-123">**clientSecret**</span></span> | <span data-ttu-id="28550-124">String</span><span class="sxs-lookup"><span data-stu-id="28550-124">String</span></span> |  <span data-ttu-id="28550-125">Geheimer Clientschlüssel zum Authentifizieren der Verbindungs an den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="28550-125">Client secret to authenticate the connection to the provider.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
