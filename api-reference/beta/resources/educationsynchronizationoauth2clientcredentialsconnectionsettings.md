---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings-Ressource
description: Wenn OAuth2 Client Anmeldeinformationen Grant in Verbindung mit den Datenanbieter bestimmt ist, sollte dieser Einstellungen Verbindungstyp So richten Sie das Profil ein verwendet werden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 8976c3a3a6088abd88cf70182040d4b3a6cc3f7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912890"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="17fba-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings-Ressource</span><span class="sxs-lookup"><span data-stu-id="17fba-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="17fba-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="17fba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17fba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="17fba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17fba-106">Wenn [OAuth2 Client Anmeldeinformationen Grant](https://tools.ietf.org/html/rfc6749#section-4.4) in Verbindung mit den Datenanbieter bestimmt ist, sollte dieser Einstellungen Verbindungstyp So richten Sie das Profil ein verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="17fba-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="17fba-107">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="17fba-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="17fba-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="17fba-108">Properties</span></span>

| <span data-ttu-id="17fba-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17fba-109">Property</span></span> | <span data-ttu-id="17fba-110">Typ</span><span class="sxs-lookup"><span data-stu-id="17fba-110">Type</span></span> | <span data-ttu-id="17fba-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17fba-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="17fba-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="17fba-112">**tokenUrl**</span></span> | <span data-ttu-id="17fba-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17fba-113">String</span></span> | <span data-ttu-id="17fba-114">Die URL für den Datenanbieter Zugriffstoken abgerufen.</span><span class="sxs-lookup"><span data-stu-id="17fba-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="17fba-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="17fba-115">**scope**</span></span> | <span data-ttu-id="17fba-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17fba-116">String</span></span> | <span data-ttu-id="17fba-117">[Der Bereich der Access-Anforderung](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="17fba-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="17fba-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="17fba-118">JSON representation</span></span>
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
