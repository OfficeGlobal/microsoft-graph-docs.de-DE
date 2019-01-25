---
title: Ressourcentyp implicitGrantSettings
description: Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann. Separate Eigenschaften sind verfügbar als Teil der implizite Ablauf Token-ID und Zugriff anfordern. Um implizite Ablauf aktivieren, mindestens eine der folgenden Eigenschaften festgelegt werden muss auf "true".
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520564"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="fae0a-105">Ressourcentyp implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="fae0a-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fae0a-106">Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann.</span><span class="sxs-lookup"><span data-stu-id="fae0a-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="fae0a-107">Separate Eigenschaften sind verfügbar als Teil der implizite Ablauf Token-ID und Zugriff anfordern.</span><span class="sxs-lookup"><span data-stu-id="fae0a-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="fae0a-108">Um implizite Ablauf aktivieren, mindestens eine der folgenden Eigenschaften festgelegt werden muss auf "true".</span><span class="sxs-lookup"><span data-stu-id="fae0a-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="fae0a-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fae0a-109">Properties</span></span>

| <span data-ttu-id="fae0a-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fae0a-110">Property</span></span> | <span data-ttu-id="fae0a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="fae0a-111">Type</span></span> | <span data-ttu-id="fae0a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fae0a-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="fae0a-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="fae0a-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="fae0a-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fae0a-114">Boolean</span></span> | <span data-ttu-id="fae0a-115">Gibt an, ob diese Web Application ein Token-ID mithilfe des impliziten OAuth 2.0-Fluss anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="fae0a-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="fae0a-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="fae0a-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="fae0a-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fae0a-117">Boolean</span></span> | <span data-ttu-id="fae0a-118">Gibt an, ob diese Web Application ein Zugriffstoken mit den impliziten OAuth 2.0-Fluss anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="fae0a-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fae0a-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fae0a-119">JSON representation</span></span>
<span data-ttu-id="fae0a-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fae0a-120">Here is a JSON representation of the resource.</span></span>

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
