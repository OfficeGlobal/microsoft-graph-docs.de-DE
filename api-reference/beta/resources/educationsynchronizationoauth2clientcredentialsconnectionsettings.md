---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings-Ressource
description: Wenn OAuth2 Client Anmeldeinformationen Grant in Verbindung mit den Datenanbieter bestimmt ist, sollte dieser Einstellungen Verbindungstyp So richten Sie das Profil ein verwendet werden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 8cf7ee292b819a05a735ce6bed2a2c4fc4275907
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425456"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="ea902-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings-Ressource</span><span class="sxs-lookup"><span data-stu-id="ea902-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="ea902-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="ea902-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea902-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea902-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ea902-106">Wenn [OAuth2 Client Anmeldeinformationen Grant](https://tools.ietf.org/html/rfc6749#section-4.4) in Verbindung mit den Datenanbieter bestimmt ist, sollte dieser Einstellungen Verbindungstyp So richten Sie das Profil ein verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="ea902-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="ea902-107">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="ea902-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ea902-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ea902-108">Properties</span></span>

| <span data-ttu-id="ea902-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea902-109">Property</span></span> | <span data-ttu-id="ea902-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ea902-110">Type</span></span> | <span data-ttu-id="ea902-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea902-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ea902-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="ea902-112">**tokenUrl**</span></span> | <span data-ttu-id="ea902-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea902-113">String</span></span> | <span data-ttu-id="ea902-114">Die URL für den Datenanbieter Zugriffstoken abgerufen.</span><span class="sxs-lookup"><span data-stu-id="ea902-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="ea902-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="ea902-115">**scope**</span></span> | <span data-ttu-id="ea902-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea902-116">String</span></span> | <span data-ttu-id="ea902-117">[Der Bereich der Access-Anforderung](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="ea902-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ea902-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ea902-118">JSON representation</span></span>
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
