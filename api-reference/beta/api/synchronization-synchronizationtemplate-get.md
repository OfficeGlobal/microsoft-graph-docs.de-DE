---
title: Abrufen von SynchronisationVorlage
description: Rufen Sie eine Synchronisierung Vorlage anhand des Bezeichners ab.
ms.openlocfilehash: 1ff3f11cf42f5a861e379c8fba2b491fbee2225e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060064"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="a642a-103">Abrufen von SynchronisationVorlage</span><span class="sxs-lookup"><span data-stu-id="a642a-103">Get synchronizationTemplate</span></span>

> <span data-ttu-id="a642a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a642a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a642a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a642a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a642a-106">Rufen Sie eine Synchronisierung Vorlage anhand des Bezeichners ab.</span><span class="sxs-lookup"><span data-stu-id="a642a-106">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="a642a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a642a-107">Permissions</span></span>
<span data-ttu-id="a642a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a642a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a642a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a642a-110">Permission type</span></span>                        | <span data-ttu-id="a642a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a642a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a642a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a642a-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="a642a-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a642a-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a642a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a642a-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a642a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a642a-115">Not supported.</span></span>|
|<span data-ttu-id="a642a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a642a-116">Application</span></span>                            |<span data-ttu-id="a642a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a642a-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="a642a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a642a-118">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="a642a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a642a-119">Request headers</span></span>

| <span data-ttu-id="a642a-120">Name</span><span class="sxs-lookup"><span data-stu-id="a642a-120">Name</span></span>           | <span data-ttu-id="a642a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a642a-121">Type</span></span>    | <span data-ttu-id="a642a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a642a-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a642a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a642a-123">Authorization</span></span>  | <span data-ttu-id="a642a-124">string</span><span class="sxs-lookup"><span data-stu-id="a642a-124">string</span></span>  | <span data-ttu-id="a642a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a642a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a642a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a642a-127">Request body</span></span>

<span data-ttu-id="a642a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a642a-128">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="a642a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a642a-129">Response</span></span>

<span data-ttu-id="a642a-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a642a-130">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="a642a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a642a-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a642a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a642a-132">Request</span></span>
<span data-ttu-id="a642a-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a642a-133">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="a642a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a642a-134">Response</span></span>
<span data-ttu-id="a642a-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="a642a-135">The following is an example of a response.</span></span>
><span data-ttu-id="a642a-136">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="a642a-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a642a-137">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a642a-137">All the properties will be returned in an actual call.</span></span>

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