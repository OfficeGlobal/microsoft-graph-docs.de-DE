---
title: Ressourcentyp implicitGrantSettings
description: Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann. Separate Eigenschaften sind verfügbar als Teil der implizite Ablauf Token-ID und Zugriff anfordern. Um implizite Ablauf aktivieren, mindestens eine der folgenden Eigenschaften festgelegt werden muss auf "true".
ms.openlocfilehash: 018cd422b56724811e1913ff0e94aea16d7c68f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060472"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="6ee20-105">Ressourcentyp implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="6ee20-105">implicitGrantSettings resource type</span></span>

> <span data-ttu-id="6ee20-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6ee20-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ee20-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ee20-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ee20-108">Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann.</span><span class="sxs-lookup"><span data-stu-id="6ee20-108">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="6ee20-109">Separate Eigenschaften sind verfügbar als Teil der implizite Ablauf Token-ID und Zugriff anfordern.</span><span class="sxs-lookup"><span data-stu-id="6ee20-109">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="6ee20-110">Um implizite Ablauf aktivieren, mindestens eine der folgenden Eigenschaften festgelegt werden muss auf "true".</span><span class="sxs-lookup"><span data-stu-id="6ee20-110">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="6ee20-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ee20-111">Properties</span></span>

| <span data-ttu-id="6ee20-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ee20-112">Property</span></span> | <span data-ttu-id="6ee20-113">Typ</span><span class="sxs-lookup"><span data-stu-id="6ee20-113">Type</span></span> | <span data-ttu-id="6ee20-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ee20-114">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="6ee20-115">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="6ee20-115">enableIdTokenIssuance</span></span>| <span data-ttu-id="6ee20-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="6ee20-116">Boolean</span></span> | <span data-ttu-id="6ee20-117">Gibt an, ob diese Web Application ein Token-ID mithilfe des impliziten OAuth 2.0-Fluss anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="6ee20-117">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="6ee20-118">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="6ee20-118">enableAccessTokenIssuance</span></span>| <span data-ttu-id="6ee20-119">Boolesch</span><span class="sxs-lookup"><span data-stu-id="6ee20-119">Boolean</span></span> | <span data-ttu-id="6ee20-120">Gibt an, ob diese Web Application ein Zugriffstoken mit den impliziten OAuth 2.0-Fluss anfordern kann.</span><span class="sxs-lookup"><span data-stu-id="6ee20-120">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ee20-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ee20-121">JSON representation</span></span>
<span data-ttu-id="6ee20-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ee20-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
