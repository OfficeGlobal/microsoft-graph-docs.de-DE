---
title: Löschrichtlinie
description: Löschen einer Richtlinie.
localization_priority: Normal
ms.openlocfilehash: e4e5f5372e2904e1f74bc25224e3d2b1ce7ba154
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520438"
---
# <a name="delete-policy"></a><span data-ttu-id="45e9c-103">Löschrichtlinie</span><span class="sxs-lookup"><span data-stu-id="45e9c-103">Delete Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45e9c-104">Löschen einer [Richtlinie](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="45e9c-104">Delete a [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="45e9c-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="45e9c-105">Permissions</span></span>
<span data-ttu-id="45e9c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45e9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45e9c-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45e9c-108">Permission type</span></span>      | <span data-ttu-id="45e9c-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45e9c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45e9c-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45e9c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="45e9c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="45e9c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="45e9c-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45e9c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45e9c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45e9c-113">Not supported.</span></span>    |
|<span data-ttu-id="45e9c-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45e9c-114">Application</span></span> | <span data-ttu-id="45e9c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45e9c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45e9c-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45e9c-116">HTTP request</span></span>

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="45e9c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45e9c-117">Request headers</span></span>
| <span data-ttu-id="45e9c-118">Name</span><span class="sxs-lookup"><span data-stu-id="45e9c-118">Name</span></span>       | <span data-ttu-id="45e9c-119">Typ</span><span class="sxs-lookup"><span data-stu-id="45e9c-119">Type</span></span> | <span data-ttu-id="45e9c-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45e9c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="45e9c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45e9c-121">Authorization</span></span>  | <span data-ttu-id="45e9c-122">string</span><span class="sxs-lookup"><span data-stu-id="45e9c-122">string</span></span>  | <span data-ttu-id="45e9c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="45e9c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45e9c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45e9c-125">Request body</span></span>
<span data-ttu-id="45e9c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="45e9c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45e9c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="45e9c-127">Response</span></span>

<span data-ttu-id="45e9c-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45e9c-128">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="45e9c-129">Wenn Sie nicht erfolgreich...</span><span class="sxs-lookup"><span data-stu-id="45e9c-129">If unsuccessful...</span></span>

## <a name="example"></a><span data-ttu-id="45e9c-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45e9c-130">Example</span></span>
<span data-ttu-id="45e9c-131">Im folgende Beispiel wird eine Richtlinie gelöscht.</span><span class="sxs-lookup"><span data-stu-id="45e9c-131">The following example deletes a policy.</span></span>

##### <a name="request"></a><span data-ttu-id="45e9c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="45e9c-132">Request</span></span>
<span data-ttu-id="45e9c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="45e9c-133">Here is an example of the request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a><span data-ttu-id="45e9c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="45e9c-134">Response</span></span>
<span data-ttu-id="45e9c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45e9c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
