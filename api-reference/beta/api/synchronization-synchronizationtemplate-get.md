---
title: Abrufen von SynchronisationVorlage
description: Rufen Sie eine Synchronisierung Vorlage anhand des Bezeichners ab.
localization_priority: Normal
ms.openlocfilehash: 4fc13ee5d83d6501f75bb45ce69f189b8809270c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524373"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="6d28a-103">Abrufen von SynchronisationVorlage</span><span class="sxs-lookup"><span data-stu-id="6d28a-103">Get synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d28a-104">Rufen Sie eine Synchronisierung Vorlage anhand des Bezeichners ab.</span><span class="sxs-lookup"><span data-stu-id="6d28a-104">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d28a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6d28a-105">Permissions</span></span>
<span data-ttu-id="6d28a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d28a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d28a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d28a-108">Permission type</span></span>                        | <span data-ttu-id="6d28a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d28a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d28a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d28a-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="6d28a-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d28a-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="6d28a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d28a-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="6d28a-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d28a-113">Not supported.</span></span>|
|<span data-ttu-id="6d28a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d28a-114">Application</span></span>                            |<span data-ttu-id="6d28a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d28a-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="6d28a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d28a-116">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="6d28a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d28a-117">Request headers</span></span>

| <span data-ttu-id="6d28a-118">Name</span><span class="sxs-lookup"><span data-stu-id="6d28a-118">Name</span></span>           | <span data-ttu-id="6d28a-119">Typ</span><span class="sxs-lookup"><span data-stu-id="6d28a-119">Type</span></span>    | <span data-ttu-id="6d28a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d28a-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="6d28a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d28a-121">Authorization</span></span>  | <span data-ttu-id="6d28a-122">string</span><span class="sxs-lookup"><span data-stu-id="6d28a-122">string</span></span>  | <span data-ttu-id="6d28a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6d28a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d28a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d28a-125">Request body</span></span>

<span data-ttu-id="6d28a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6d28a-126">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="6d28a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d28a-127">Response</span></span>

<span data-ttu-id="6d28a-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6d28a-128">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="6d28a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d28a-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6d28a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d28a-130">Request</span></span>
<span data-ttu-id="6d28a-131">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d28a-131">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="6d28a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d28a-132">Response</span></span>
<span data-ttu-id="6d28a-133">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="6d28a-133">The following is an example of a response.</span></span>
><span data-ttu-id="6d28a-134">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="6d28a-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6d28a-135">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d28a-135">All the properties will be returned in an actual call.</span></span>

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
