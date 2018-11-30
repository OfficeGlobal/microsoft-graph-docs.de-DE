---
title: Web-Ressourcentyp
description: Gibt die Einstellungen für eine Webanwendung.
ms.openlocfilehash: c040de0c323e57f20e04dcf662ea088b1018c144
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064069"
---
# <a name="web-resource-type"></a><span data-ttu-id="1bfa6-103">Web-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1bfa6-103">web resource type</span></span>

> <span data-ttu-id="1bfa6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1bfa6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bfa6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1bfa6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1bfa6-106">Gibt die Einstellungen für eine Webanwendung.</span><span class="sxs-lookup"><span data-stu-id="1bfa6-106">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="1bfa6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1bfa6-107">Properties</span></span>

| <span data-ttu-id="1bfa6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1bfa6-108">Property</span></span> | <span data-ttu-id="1bfa6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1bfa6-109">Type</span></span> | <span data-ttu-id="1bfa6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1bfa6-110">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="1bfa6-111">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="1bfa6-111">implicitGrantSettings</span></span>|[<span data-ttu-id="1bfa6-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="1bfa6-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="1bfa6-113">Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann.</span><span class="sxs-lookup"><span data-stu-id="1bfa6-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="1bfa6-114">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="1bfa6-114">logoutUrl</span></span>|<span data-ttu-id="1bfa6-115">String</span><span class="sxs-lookup"><span data-stu-id="1bfa6-115">String</span></span>| <span data-ttu-id="1bfa6-116">Gibt die URL, die von Microsoft Autorisierungsdienst Abmelden ein Benutzer mit der [Vorderseite-Kanal](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [Back-Kanal](https://openid.net/specs/openid-connect-backchannel-1_0.html) oder SAML Abmeldung Protokolle verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1bfa6-116">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="1bfa6-117">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="1bfa6-117">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="1bfa6-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="1bfa6-118">Boolean</span></span>| <span data-ttu-id="1bfa6-119">Veraltet.</span><span class="sxs-lookup"><span data-stu-id="1bfa6-119">Deprecated.</span></span> <span data-ttu-id="1bfa6-120">Nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="1bfa6-120">Do not use.</span></span> | 
|<span data-ttu-id="1bfa6-121">redirectUris</span><span class="sxs-lookup"><span data-stu-id="1bfa6-121">redirectUris</span></span>|<span data-ttu-id="1bfa6-122">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="1bfa6-122">String collection</span></span>| <span data-ttu-id="1bfa6-123">Gibt die URLs der Benutzertoken für die Anmeldung an gesendet werden, oder die Umleitung, URIs, dass OAuth 2.0 Autorisierungscodes und Zugriffstoken gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="1bfa6-123">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1bfa6-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1bfa6-124">JSON representation</span></span>
<span data-ttu-id="1bfa6-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1bfa6-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.web"
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
<!-- {
  "type": "#page.annotation",
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
