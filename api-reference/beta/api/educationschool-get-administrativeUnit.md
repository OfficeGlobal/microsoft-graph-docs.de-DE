---
title: AdministrativeUnit abrufen
description: Abrufen der einfachen **AdministrativeUnit** , die diese **EducationSchool**entspricht.
ms.openlocfilehash: 49ac05b44bc89f827091c3b846885a58cb7b8956
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062332"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="c19c0-103">AdministrativeUnit abrufen</span><span class="sxs-lookup"><span data-stu-id="c19c0-103">Get administrativeUnit</span></span>

> <span data-ttu-id="c19c0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c19c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c19c0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c19c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c19c0-106">Abrufen der einfachen **AdministrativeUnit** , die diese **EducationSchool**entspricht.</span><span class="sxs-lookup"><span data-stu-id="c19c0-106">Retrieve the simple directory **administrativeUnit** that corresponds to this **educationSchool**.</span></span>

><span data-ttu-id="c19c0-107">**Hinweis:** Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Schulen.</span><span class="sxs-lookup"><span data-stu-id="c19c0-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="c19c0-108">Verwenden Sie in diesem Fall die Ressource `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="c19c0-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="c19c0-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c19c0-109">Permissions</span></span>
<span data-ttu-id="c19c0-110">Zum Aufrufen dieser API ist eine Kombination von Berechtigungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c19c0-110">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="c19c0-111">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c19c0-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c19c0-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c19c0-112">Permission type</span></span>      | <span data-ttu-id="c19c0-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c19c0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c19c0-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c19c0-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="c19c0-115">Eine von EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write sowie Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c19c0-115">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="c19c0-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c19c0-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c19c0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c19c0-117">Not supported.</span></span>  |
|<span data-ttu-id="c19c0-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c19c0-118">Application</span></span> | <span data-ttu-id="c19c0-119">EduRoster.Read.All, EduRoster.ReadWrite.All und Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c19c0-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="c19c0-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c19c0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a><span data-ttu-id="c19c0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c19c0-121">Request headers</span></span>
| <span data-ttu-id="c19c0-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c19c0-122">Header</span></span>       | <span data-ttu-id="c19c0-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c19c0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c19c0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c19c0-124">Authorization</span></span>  | <span data-ttu-id="c19c0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c19c0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c19c0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c19c0-127">Request body</span></span>
<span data-ttu-id="c19c0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c19c0-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c19c0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c19c0-129">Response</span></span>
<span data-ttu-id="c19c0-130">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [AdministrativeUnit](../resources/administrativeunit.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c19c0-130">If successful, this method returns a `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c19c0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c19c0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c19c0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c19c0-132">Request</span></span>
<span data-ttu-id="c19c0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c19c0-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeUnit"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
##### <a name="response"></a><span data-ttu-id="c19c0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c19c0-134">Response</span></span>
<span data-ttu-id="c19c0-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c19c0-135">The following is an example of the response.</span></span> 

><span data-ttu-id="c19c0-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c19c0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

<!-- uuid: A681726F-B4A7-4BCF-9407-F87CB9A4771D
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->