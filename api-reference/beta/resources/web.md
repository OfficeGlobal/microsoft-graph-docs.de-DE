---
title: Web-Ressourcentyp
description: Gibt die Einstellungen für eine Webanwendung.
localization_priority: Normal
ms.openlocfilehash: 26efe59eda739597e7193fa1ff79443f3d64b5a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890202"
---
# <a name="web-resource-type"></a><span data-ttu-id="d71d0-103">Web-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d71d0-103">web resource type</span></span>

> <span data-ttu-id="d71d0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d71d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d71d0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d71d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d71d0-106">Gibt die Einstellungen für eine Webanwendung.</span><span class="sxs-lookup"><span data-stu-id="d71d0-106">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="d71d0-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d71d0-107">Properties</span></span>

| <span data-ttu-id="d71d0-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d71d0-108">Property</span></span> | <span data-ttu-id="d71d0-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d71d0-109">Type</span></span> | <span data-ttu-id="d71d0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d71d0-110">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="d71d0-111">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="d71d0-111">implicitGrantSettings</span></span>|[<span data-ttu-id="d71d0-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="d71d0-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="d71d0-113">Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann.</span><span class="sxs-lookup"><span data-stu-id="d71d0-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="d71d0-114">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="d71d0-114">logoutUrl</span></span>|<span data-ttu-id="d71d0-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d71d0-115">String</span></span>| <span data-ttu-id="d71d0-116">Gibt die URL, die von Microsoft Autorisierungsdienst Abmelden ein Benutzer mit der [Vorderseite-Kanal](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [Back-Kanal](https://openid.net/specs/openid-connect-backchannel-1_0.html) oder SAML Abmeldung Protokolle verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d71d0-116">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="d71d0-117">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="d71d0-117">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="d71d0-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d71d0-118">Boolean</span></span>| <span data-ttu-id="d71d0-119">Veraltet.</span><span class="sxs-lookup"><span data-stu-id="d71d0-119">Deprecated.</span></span> <span data-ttu-id="d71d0-120">Nicht verwenden.</span><span class="sxs-lookup"><span data-stu-id="d71d0-120">Do not use.</span></span> | 
|<span data-ttu-id="d71d0-121">redirectUris</span><span class="sxs-lookup"><span data-stu-id="d71d0-121">redirectUris</span></span>|<span data-ttu-id="d71d0-122">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="d71d0-122">String collection</span></span>| <span data-ttu-id="d71d0-123">Gibt die URLs der Benutzertoken für die Anmeldung an gesendet werden, oder die Umleitung, URIs, dass OAuth 2.0 Autorisierungscodes und Zugriffstoken gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="d71d0-123">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d71d0-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d71d0-124">JSON representation</span></span>
<span data-ttu-id="d71d0-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d71d0-125">Here is a JSON representation of the resource.</span></span>

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
