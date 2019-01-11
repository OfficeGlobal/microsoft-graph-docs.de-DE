---
title: Abrufen von SynchronisationVorlage
description: Rufen Sie eine Synchronisierung Vorlage anhand des Bezeichners ab.
localization_priority: Normal
ms.openlocfilehash: 9754b1fbc8c86f05d22f0ada57b8b97e0b1efbed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863812"
---
# <a name="get-synchronizationtemplate"></a><span data-ttu-id="32c16-103">Abrufen von SynchronisationVorlage</span><span class="sxs-lookup"><span data-stu-id="32c16-103">Get synchronizationTemplate</span></span>

> <span data-ttu-id="32c16-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="32c16-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32c16-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="32c16-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32c16-106">Rufen Sie eine Synchronisierung Vorlage anhand des Bezeichners ab.</span><span class="sxs-lookup"><span data-stu-id="32c16-106">Retrieve a synchronization template by its identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="32c16-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="32c16-107">Permissions</span></span>
<span data-ttu-id="32c16-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32c16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32c16-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="32c16-110">Permission type</span></span>                        | <span data-ttu-id="32c16-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="32c16-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="32c16-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="32c16-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="32c16-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32c16-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="32c16-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="32c16-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="32c16-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32c16-115">Not supported.</span></span>|
|<span data-ttu-id="32c16-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="32c16-116">Application</span></span>                            |<span data-ttu-id="32c16-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="32c16-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="32c16-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="32c16-118">HTTP Request</span></span>

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="32c16-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="32c16-119">Request headers</span></span>

| <span data-ttu-id="32c16-120">Name</span><span class="sxs-lookup"><span data-stu-id="32c16-120">Name</span></span>           | <span data-ttu-id="32c16-121">Typ</span><span class="sxs-lookup"><span data-stu-id="32c16-121">Type</span></span>    | <span data-ttu-id="32c16-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32c16-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="32c16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32c16-123">Authorization</span></span>  | <span data-ttu-id="32c16-124">string</span><span class="sxs-lookup"><span data-stu-id="32c16-124">string</span></span>  | <span data-ttu-id="32c16-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="32c16-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32c16-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="32c16-127">Request body</span></span>

<span data-ttu-id="32c16-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="32c16-128">Do not supply a request body for this method.</span></span>

### <a name="response"></a><span data-ttu-id="32c16-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="32c16-129">Response</span></span>

<span data-ttu-id="32c16-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="32c16-130">If successful, this method returns a `200 OK` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="32c16-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="32c16-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="32c16-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="32c16-132">Request</span></span>
<span data-ttu-id="32c16-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="32c16-133">The following is an example of a request.</span></span>

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a><span data-ttu-id="32c16-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="32c16-134">Response</span></span>
<span data-ttu-id="32c16-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="32c16-135">The following is an example of a response.</span></span>
><span data-ttu-id="32c16-136">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="32c16-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="32c16-137">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="32c16-137">All the properties will be returned in an actual call.</span></span>

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
