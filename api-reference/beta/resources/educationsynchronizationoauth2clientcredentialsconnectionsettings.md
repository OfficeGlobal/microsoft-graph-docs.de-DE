---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings-Ressource
description: Wenn OAuth2 Client Anmeldeinformationen Grant in Verbindung mit den Datenanbieter bestimmt ist, sollte dieser Einstellungen Verbindungstyp So richten Sie das Profil ein verwendet werden.
ms.openlocfilehash: 901fabb802d4ed5fa0c99538e52b9a07199eb298
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063873"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="e8492-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings-Ressource</span><span class="sxs-lookup"><span data-stu-id="e8492-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="e8492-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e8492-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8492-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e8492-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8492-106">Wenn [OAuth2 Client Anmeldeinformationen Grant](https://tools.ietf.org/html/rfc6749#section-4.4) in Verbindung mit den Datenanbieter bestimmt ist, sollte dieser Einstellungen Verbindungstyp So richten Sie das Profil ein verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e8492-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="e8492-107">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="e8492-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e8492-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e8492-108">Properties</span></span>

| <span data-ttu-id="e8492-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e8492-109">Property</span></span> | <span data-ttu-id="e8492-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e8492-110">Type</span></span> | <span data-ttu-id="e8492-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e8492-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="e8492-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="e8492-112">**tokenUrl**</span></span> | <span data-ttu-id="e8492-113">String</span><span class="sxs-lookup"><span data-stu-id="e8492-113">String</span></span> | <span data-ttu-id="e8492-114">Die URL für den Datenanbieter Zugriffstoken abgerufen.</span><span class="sxs-lookup"><span data-stu-id="e8492-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="e8492-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="e8492-115">**scope**</span></span> | <span data-ttu-id="e8492-116">String</span><span class="sxs-lookup"><span data-stu-id="e8492-116">String</span></span> | <span data-ttu-id="e8492-117">[Der Bereich der Access-Anforderung](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="e8492-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e8492-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e8492-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
