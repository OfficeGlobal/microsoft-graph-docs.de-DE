---
title: Ressourcentyp implicitGrantSettings
description: Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann. Separate Eigenschaften sind verfügbar als Teil der implizite Ablauf Token-ID und Zugriff anfordern. Um implizite Ablauf aktivieren, mindestens eine der folgenden Eigenschaften festgelegt werden muss auf "true".
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642765"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="321bd-105">Ressourcentyp implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="321bd-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="321bd-106">Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann.</span><span class="sxs-lookup"><span data-stu-id="321bd-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="321bd-107">Separate Eigenschaften sind verfügbar als Teil der implizite Ablauf Token-ID und Zugriff anfordern.</span><span class="sxs-lookup"><span data-stu-id="321bd-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="321bd-108">Um implizite Ablauf aktivieren, mindestens eine der folgenden Eigenschaften festgelegt werden muss auf "true".</span><span class="sxs-lookup"><span data-stu-id="321bd-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="321bd-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="321bd-109">Properties</span></span>

| <span data-ttu-id="321bd-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="321bd-110">Property</span></span> | <span data-ttu-id="321bd-111">Typ</span><span class="sxs-lookup"><span data-stu-id="321bd-111">Type</span></span> | <span data-ttu-id="321bd-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="321bd-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="321bd-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="321bd-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="321bd-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="321bd-114">Boolean</span></span> | <span data-ttu-id="321bd-115">Gibt an, ob diese Web Application ein Token-ID mithilfe des impliziten OAuth 2.0-Fluss anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="321bd-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="321bd-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="321bd-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="321bd-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="321bd-117">Boolean</span></span> | <span data-ttu-id="321bd-118">Gibt an, ob diese Web Application ein Zugriffstoken mit den impliziten OAuth 2.0-Fluss anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="321bd-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="321bd-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="321bd-119">JSON representation</span></span>
<span data-ttu-id="321bd-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="321bd-120">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
