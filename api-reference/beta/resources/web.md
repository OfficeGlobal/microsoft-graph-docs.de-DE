---
title: Web-Ressourcentyp
description: Gibt die Einstellungen für eine Webanwendung.
localization_priority: Normal
ms.openlocfilehash: 281a3f23dd0e22cae6b3ca2b67e2e9cd8b400740
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572717"
---
# <a name="web-resource-type"></a><span data-ttu-id="36053-103">Web-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="36053-103">web resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36053-104">Gibt die Einstellungen für eine Webanwendung.</span><span class="sxs-lookup"><span data-stu-id="36053-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="36053-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="36053-105">Properties</span></span>

| <span data-ttu-id="36053-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="36053-106">Property</span></span> | <span data-ttu-id="36053-107">Typ</span><span class="sxs-lookup"><span data-stu-id="36053-107">Type</span></span> | <span data-ttu-id="36053-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="36053-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="36053-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="36053-109">implicitGrantSettings</span></span>|[<span data-ttu-id="36053-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="36053-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="36053-111">Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann.</span><span class="sxs-lookup"><span data-stu-id="36053-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="36053-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="36053-112">logoutUrl</span></span>|<span data-ttu-id="36053-113">String</span><span class="sxs-lookup"><span data-stu-id="36053-113">String</span></span>| <span data-ttu-id="36053-114">Gibt die URL, die von Microsoft Autorisierungsdienst Abmelden ein Benutzer mit der [Vorderseite-Kanal](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [Back-Kanal](https://openid.net/specs/openid-connect-backchannel-1_0.html) oder SAML Abmeldung Protokolle verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="36053-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="36053-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="36053-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="36053-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="36053-116">Boolean</span></span>| <span data-ttu-id="36053-117">Veraltet.</span><span class="sxs-lookup"><span data-stu-id="36053-117">Deprecated.</span></span> <span data-ttu-id="36053-118">Nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="36053-118">Do not use.</span></span> | 
|<span data-ttu-id="36053-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="36053-119">redirectUris</span></span>|<span data-ttu-id="36053-120">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="36053-120">String collection</span></span>| <span data-ttu-id="36053-121">Gibt die URLs der Benutzertoken für die Anmeldung an gesendet werden, oder die Umleitung, URIs, dass OAuth 2.0 Autorisierungscodes und Zugriffstoken gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="36053-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="36053-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="36053-122">JSON representation</span></span>
<span data-ttu-id="36053-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="36053-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
}-->

```json
{
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "oauth2AllowImplicitFlow": false,
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/web.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
