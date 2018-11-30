---
title: Löschrichtlinie
description: Löschen einer Richtlinie.
ms.openlocfilehash: 37ed08e7f53db726a46821c08d68c955afdacc5a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065442"
---
# <a name="delete-policy"></a><span data-ttu-id="7e73f-103">Löschrichtlinie</span><span class="sxs-lookup"><span data-stu-id="7e73f-103">Delete Policy</span></span>

> <span data-ttu-id="7e73f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7e73f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e73f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7e73f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e73f-106">Löschen einer [Richtlinie](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="7e73f-106">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e73f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7e73f-107">Permissions</span></span>
<span data-ttu-id="7e73f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e73f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e73f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7e73f-110">Permission type</span></span>      | <span data-ttu-id="7e73f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7e73f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e73f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7e73f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7e73f-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e73f-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e73f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7e73f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e73f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e73f-115">Not supported.</span></span>    |
|<span data-ttu-id="7e73f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7e73f-116">Application</span></span> | <span data-ttu-id="7e73f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7e73f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e73f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e73f-118">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7e73f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7e73f-119">Request headers</span></span>
| <span data-ttu-id="7e73f-120">Name</span><span class="sxs-lookup"><span data-stu-id="7e73f-120">Name</span></span>       | <span data-ttu-id="7e73f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="7e73f-121">Type</span></span> | <span data-ttu-id="7e73f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e73f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7e73f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e73f-123">Authorization</span></span>  | <span data-ttu-id="7e73f-124">string</span><span class="sxs-lookup"><span data-stu-id="7e73f-124">string</span></span>  | <span data-ttu-id="7e73f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7e73f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e73f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7e73f-127">Request body</span></span>
<span data-ttu-id="7e73f-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7e73f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e73f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e73f-129">Response</span></span>

<span data-ttu-id="7e73f-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e73f-130">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="7e73f-131">Wenn Sie nicht erfolgreich...</span><span class="sxs-lookup"><span data-stu-id="7e73f-131">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="7e73f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7e73f-132">Example</span></span>
<span data-ttu-id="7e73f-133">Im folgende Beispiel wird eine Richtlinie gelöscht.</span><span class="sxs-lookup"><span data-stu-id="7e73f-133">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="7e73f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7e73f-134">Request</span></span>
<span data-ttu-id="7e73f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7e73f-135">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="7e73f-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7e73f-136">Response</span></span>
<span data-ttu-id="7e73f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7e73f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
