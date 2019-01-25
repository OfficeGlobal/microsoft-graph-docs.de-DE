---
title: Ressourcentyp onPremisesPublishing
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508181"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="f0b82-103">Ressourcentyp onPremisesPublishing</span><span class="sxs-lookup"><span data-stu-id="f0b82-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="f0b82-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f0b82-104">Properties</span></span>
| <span data-ttu-id="f0b82-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0b82-105">Property</span></span>     | <span data-ttu-id="f0b82-106">Typ</span><span class="sxs-lookup"><span data-stu-id="f0b82-106">Type</span></span>   |<span data-ttu-id="f0b82-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0b82-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0b82-108">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="f0b82-108">customDomainCertificate</span></span>|<span data-ttu-id="f0b82-109">String</span><span class="sxs-lookup"><span data-stu-id="f0b82-109">String</span></span>|<span data-ttu-id="f0b82-110">Details des Zertifikats mit der Anwendung verbunden sind, wenn eine benutzerdefinierte Domäne verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f0b82-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="f0b82-111">NULL, wenn die Standarddomäne zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f0b82-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="f0b82-112">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="f0b82-112">externalAuthenticationType</span></span>|<span data-ttu-id="f0b82-113">String</span><span class="sxs-lookup"><span data-stu-id="f0b82-113">String</span></span>|<span data-ttu-id="f0b82-114">Details der Vorauthentifizierung-Einstellung für die Anwendung möglichen Werte sind: `passthru`, `aadPreAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="f0b82-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="f0b82-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="f0b82-115">externalUrl</span></span>|<span data-ttu-id="f0b82-116">String</span><span class="sxs-lookup"><span data-stu-id="f0b82-116">String</span></span>|<span data-ttu-id="f0b82-117">Die veröffentlichte externe Url für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="f0b82-117">The published external url for the application.</span></span> <span data-ttu-id="f0b82-118">Beispiel: https://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="f0b82-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="f0b82-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="f0b82-119">internalUrl</span></span>|<span data-ttu-id="f0b82-120">String</span><span class="sxs-lookup"><span data-stu-id="f0b82-120">String</span></span>|<span data-ttu-id="f0b82-121">Die interne Url der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="f0b82-121">The internal url of the application.</span></span> <span data-ttu-id="f0b82-122">Beispiel: https://intranet/</span><span class="sxs-lookup"><span data-stu-id="f0b82-122">For example https://intranet/</span></span> |
|<span data-ttu-id="f0b82-123">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="f0b82-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="f0b82-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f0b82-124">Boolean</span></span>|<span data-ttu-id="f0b82-125">Gibt an, ob die Anwendung derzeit oder nicht veröffentlicht wird.</span><span class="sxs-lookup"><span data-stu-id="f0b82-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="f0b82-126">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="f0b82-126">applicationServerTimeout</span></span>|<span data-ttu-id="f0b82-127">String</span><span class="sxs-lookup"><span data-stu-id="f0b82-127">String</span></span>|<span data-ttu-id="f0b82-128">Die Dauer der Verbindung eine Antwort aus der Back-End-Anwendung vor dem Schließen der Verbindungs wartet.</span><span class="sxs-lookup"><span data-stu-id="f0b82-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="f0b82-129">Mögliche Werte sind: `default` und `long`.</span><span class="sxs-lookup"><span data-stu-id="f0b82-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="f0b82-130">Verwendung `long` Wenn Ihr Server mehr als 60 75 Sekunden reagiert auf Anforderungen dauert.</span><span class="sxs-lookup"><span data-stu-id="f0b82-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="f0b82-131">Versuchen Sie außerdem `long` Wenn Sie nicht sind auf die Anwendung zugreifen und der Fehlerstatus "Backend Timeout" ist.</span><span class="sxs-lookup"><span data-stu-id="f0b82-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="f0b82-132">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="f0b82-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="f0b82-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f0b82-133">Boolean</span></span>|<span data-ttu-id="f0b82-134">Gibt an, ob die Anwendung Urls in der Antwort-Headern übersetzen sollten.</span><span class="sxs-lookup"><span data-stu-id="f0b82-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="f0b82-135">Dies beinhaltet das Festlegen der richtigen Website für Cookies.</span><span class="sxs-lookup"><span data-stu-id="f0b82-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0b82-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f0b82-136">JSON representation</span></span>

<span data-ttu-id="f0b82-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0b82-137">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
