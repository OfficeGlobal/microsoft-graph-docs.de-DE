---
title: Ressourcentyp implicitGrantSettings
description: Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann. Separate Eigenschaften sind verfügbar als Teil der implizite Ablauf Token-ID und Zugriff anfordern. Um implizite Ablauf aktivieren, mindestens eine der folgenden Eigenschaften festgelegt werden muss auf "true".
localization_priority: Normal
ms.openlocfilehash: 93a54ac0c0e4c6c32ebb99c9747d44d75f98af07
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834265"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="87c76-105">Ressourcentyp implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="87c76-105">implicitGrantSettings resource type</span></span>

> <span data-ttu-id="87c76-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87c76-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87c76-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87c76-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87c76-108">Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann.</span><span class="sxs-lookup"><span data-stu-id="87c76-108">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="87c76-109">Separate Eigenschaften sind verfügbar als Teil der implizite Ablauf Token-ID und Zugriff anfordern.</span><span class="sxs-lookup"><span data-stu-id="87c76-109">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="87c76-110">Um implizite Ablauf aktivieren, mindestens eine der folgenden Eigenschaften festgelegt werden muss auf "true".</span><span class="sxs-lookup"><span data-stu-id="87c76-110">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="87c76-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="87c76-111">Properties</span></span>

| <span data-ttu-id="87c76-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87c76-112">Property</span></span> | <span data-ttu-id="87c76-113">Typ</span><span class="sxs-lookup"><span data-stu-id="87c76-113">Type</span></span> | <span data-ttu-id="87c76-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87c76-114">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="87c76-115">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="87c76-115">enableIdTokenIssuance</span></span>| <span data-ttu-id="87c76-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="87c76-116">Boolean</span></span> | <span data-ttu-id="87c76-117">Gibt an, ob diese Web Application ein Token-ID mithilfe des impliziten OAuth 2.0-Fluss anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="87c76-117">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="87c76-118">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="87c76-118">enableAccessTokenIssuance</span></span>| <span data-ttu-id="87c76-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="87c76-119">Boolean</span></span> | <span data-ttu-id="87c76-120">Gibt an, ob diese Web Application ein Zugriffstoken mit den impliziten OAuth 2.0-Fluss anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="87c76-120">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87c76-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="87c76-121">JSON representation</span></span>
<span data-ttu-id="87c76-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="87c76-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
