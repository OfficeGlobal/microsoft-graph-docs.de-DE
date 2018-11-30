---
title: Benutzer abrufen
description: Abrufen des einfachen Verzeichnis-**Benutzers**, der diesem **educationUser** entspricht.
ms.openlocfilehash: e026fbb1b9294d99e124b16209465c530e229b86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063655"
---
# <a name="get-user"></a><span data-ttu-id="d5353-103">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="d5353-103">Get user</span></span>

> <span data-ttu-id="d5353-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d5353-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5353-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5353-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5353-106">Abrufen des einfachen Verzeichnis-**Benutzers**, der diesem **educationUser** entspricht.</span><span class="sxs-lookup"><span data-stu-id="d5353-106">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="d5353-107">**Hinweis:** Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Schulen.</span><span class="sxs-lookup"><span data-stu-id="d5353-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="d5353-108">Verwenden Sie in diesem Fall die Ressource `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="d5353-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5353-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d5353-109">Permissions</span></span>
<span data-ttu-id="d5353-110">Zum Aufrufen dieser API ist eine Kombination von Berechtigungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d5353-110">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="d5353-111">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5353-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5353-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d5353-112">Permission type</span></span>      | <span data-ttu-id="d5353-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d5353-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5353-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d5353-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="d5353-115">Eine aus EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write sowie entweder Directory.Read.All oder User.Read</span><span class="sxs-lookup"><span data-stu-id="d5353-115">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="d5353-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d5353-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d5353-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5353-117">Not supported.</span></span>  |
|<span data-ttu-id="d5353-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d5353-118">Application</span></span> | <span data-ttu-id="d5353-119">EduRoster.Read.All, EduRoster.ReadWrite.All und Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5353-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="d5353-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5353-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="d5353-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d5353-121">Request headers</span></span>
| <span data-ttu-id="d5353-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d5353-122">Header</span></span>       | <span data-ttu-id="d5353-123">Wert</span><span class="sxs-lookup"><span data-stu-id="d5353-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d5353-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5353-124">Authorization</span></span>  | <span data-ttu-id="d5353-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d5353-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d5353-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d5353-127">Request body</span></span>
<span data-ttu-id="d5353-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d5353-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d5353-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5353-129">Response</span></span>
<span data-ttu-id="d5353-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5353-130">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d5353-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d5353-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5353-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5353-132">Request</span></span>
<span data-ttu-id="d5353-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d5353-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/user
```
##### <a name="response"></a><span data-ttu-id="d5353-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5353-134">Response</span></span>
<span data-ttu-id="d5353-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d5353-135">The following is an example of the response.</span></span> 

><span data-ttu-id="d5353-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d5353-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

<!-- uuid: FC4AAF57-A0ED-4899-B104-A8B89B72AD5A
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->