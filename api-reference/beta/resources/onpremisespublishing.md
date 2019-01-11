---
title: Ressourcentyp onPremisesPublishing
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 30ff6908a42a690e07d71b5d0c62fcb22dea3c34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842539"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="263eb-103">Ressourcentyp onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="263eb-103">onPremisesPublishing resource type</span></span>

> <span data-ttu-id="263eb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="263eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="263eb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="263eb-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="263eb-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="263eb-106">Properties</span></span>
| <span data-ttu-id="263eb-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="263eb-107">Property</span></span>     | <span data-ttu-id="263eb-108">Typ</span><span class="sxs-lookup"><span data-stu-id="263eb-108">Type</span></span>   |<span data-ttu-id="263eb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="263eb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="263eb-110">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="263eb-110">customDomainCertificate</span></span>|<span data-ttu-id="263eb-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263eb-111">String</span></span>|<span data-ttu-id="263eb-112">Details des Zertifikats mit der Anwendung verbunden sind, wenn eine benutzerdefinierte Domäne verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="263eb-112">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="263eb-113">NULL, wenn die Standarddomäne zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="263eb-113">Null when using the default domain.</span></span>|
|<span data-ttu-id="263eb-114">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="263eb-114">externalAuthenticationType</span></span>|<span data-ttu-id="263eb-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263eb-115">String</span></span>|<span data-ttu-id="263eb-116">Details der Vorauthentifizierung-Einstellung für die Anwendung möglichen Werte sind: `passthru`, `aadPreAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="263eb-116">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="263eb-117">externalUrl</span><span class="sxs-lookup"><span data-stu-id="263eb-117">externalUrl</span></span>|<span data-ttu-id="263eb-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263eb-118">String</span></span>|<span data-ttu-id="263eb-119">Die veröffentlichte externe Url für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="263eb-119">The published external url for the application.</span></span> <span data-ttu-id="263eb-120">Zum Beispielhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="263eb-120">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="263eb-121">internalUrl</span><span class="sxs-lookup"><span data-stu-id="263eb-121">internalUrl</span></span>|<span data-ttu-id="263eb-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263eb-122">String</span></span>|<span data-ttu-id="263eb-123">Die interne Url der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="263eb-123">The internal url of the application.</span></span> <span data-ttu-id="263eb-124">Zum Beispielhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="263eb-124">For example https://intranet/</span></span> |
|<span data-ttu-id="263eb-125">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="263eb-125">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="263eb-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="263eb-126">Boolean</span></span>|<span data-ttu-id="263eb-127">Gibt an, ob die Anwendung derzeit oder nicht veröffentlicht wird.</span><span class="sxs-lookup"><span data-stu-id="263eb-127">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="263eb-128">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="263eb-128">applicationServerTimeout</span></span>|<span data-ttu-id="263eb-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="263eb-129">String</span></span>|<span data-ttu-id="263eb-130">Die Dauer der Verbindung eine Antwort aus der Back-End-Anwendung vor dem Schließen der Verbindungs wartet.</span><span class="sxs-lookup"><span data-stu-id="263eb-130">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="263eb-131">Mögliche Werte sind `default`, `long`.</span><span class="sxs-lookup"><span data-stu-id="263eb-131">Possible values are `default`, `long`.</span></span> <span data-ttu-id="263eb-132">Verwendung `long` Wenn Ihr Server mehr als 60 75 Sekunden reagiert auf Anforderungen dauert.</span><span class="sxs-lookup"><span data-stu-id="263eb-132">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="263eb-133">Versuchen Sie außerdem `long` Wenn Sie nicht sind auf die Anwendung zugreifen und der Fehlerstatus "Backend Timeout" ist.</span><span class="sxs-lookup"><span data-stu-id="263eb-133">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="263eb-134">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="263eb-134">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="263eb-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="263eb-135">Boolean</span></span>|<span data-ttu-id="263eb-136">Gibt an, ob die Anwendung Urls in der Antwort-Headern übersetzen sollten.</span><span class="sxs-lookup"><span data-stu-id="263eb-136">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="263eb-137">Dies beinhaltet das Festlegen der richtigen Website für Cookies.</span><span class="sxs-lookup"><span data-stu-id="263eb-137">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="263eb-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="263eb-138">JSON representation</span></span>

<span data-ttu-id="263eb-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="263eb-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
