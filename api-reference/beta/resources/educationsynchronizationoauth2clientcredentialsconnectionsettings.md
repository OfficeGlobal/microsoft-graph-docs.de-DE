---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings-Ressource
description: Wenn OAuth2 Client Anmeldeinformationen Grant in Verbindung mit den Datenanbieter bestimmt ist, sollte dieser Einstellungen Verbindungstyp So richten Sie das Profil ein verwendet werden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 37121868793dd76aec2c3b48182e114348d21014
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523554"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="8aacb-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings-Ressource</span><span class="sxs-lookup"><span data-stu-id="8aacb-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aacb-104">Wenn [OAuth2 Client Anmeldeinformationen Grant](https://tools.ietf.org/html/rfc6749#section-4.4) in Verbindung mit den Datenanbieter bestimmt ist, sollte dieser Einstellungen Verbindungstyp So richten Sie das Profil ein verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="8aacb-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="8aacb-105">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="8aacb-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8aacb-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8aacb-106">Properties</span></span>

| <span data-ttu-id="8aacb-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8aacb-107">Property</span></span> | <span data-ttu-id="8aacb-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8aacb-108">Type</span></span> | <span data-ttu-id="8aacb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8aacb-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8aacb-110">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="8aacb-110">**tokenUrl**</span></span> | <span data-ttu-id="8aacb-111">String</span><span class="sxs-lookup"><span data-stu-id="8aacb-111">String</span></span> | <span data-ttu-id="8aacb-112">Die URL für den Datenanbieter Zugriffstoken abgerufen.</span><span class="sxs-lookup"><span data-stu-id="8aacb-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="8aacb-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="8aacb-113">**scope**</span></span> | <span data-ttu-id="8aacb-114">String</span><span class="sxs-lookup"><span data-stu-id="8aacb-114">String</span></span> | <span data-ttu-id="8aacb-115">[Der Bereich der Access-Anforderung](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="8aacb-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8aacb-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8aacb-116">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationoauth2clientcredentialsconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
