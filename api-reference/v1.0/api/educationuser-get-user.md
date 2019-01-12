---
title: Benutzer abrufen
description: Abrufen des einfachen Verzeichnis-**Benutzers**, der diesem **educationUser** entspricht.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 063b1297c2243f11b6eb1020703b7332390a4aa2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991923"
---
# <a name="get-user"></a><span data-ttu-id="fbff5-103">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="fbff5-103">Get user</span></span>

<span data-ttu-id="fbff5-104">Abrufen des einfachen Verzeichnis-**Benutzers**, der diesem **educationUser** entspricht.</span><span class="sxs-lookup"><span data-stu-id="fbff5-104">Retrieve the simple directory **user** that corresponds to this **educationUser**.</span></span>

><span data-ttu-id="fbff5-105">**Hinweis:** Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Schulen.</span><span class="sxs-lookup"><span data-stu-id="fbff5-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="fbff5-106">Verwenden Sie in diesem Fall die Ressource `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="fbff5-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbff5-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fbff5-107">Permissions</span></span>
<span data-ttu-id="fbff5-108">Zum Aufrufen dieser API ist eine Kombination von Berechtigungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fbff5-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="fbff5-109">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbff5-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbff5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fbff5-110">Permission type</span></span>      | <span data-ttu-id="fbff5-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fbff5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbff5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fbff5-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="fbff5-113">Eine aus EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write sowie entweder Directory.Read.All oder User.Read</span><span class="sxs-lookup"><span data-stu-id="fbff5-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus either Directory.Read.All or User.Read</span></span>|
|<span data-ttu-id="fbff5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fbff5-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fbff5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fbff5-115">Not supported.</span></span>  |
|<span data-ttu-id="fbff5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fbff5-116">Application</span></span> | <span data-ttu-id="fbff5-117">EduRoster.Read.All, EduRoster.ReadWrite.All und Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbff5-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="fbff5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbff5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/user
GET /education/users/{id}/user
```
## <a name="request-headers"></a><span data-ttu-id="fbff5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fbff5-119">Request headers</span></span>
| <span data-ttu-id="fbff5-120">Header</span><span class="sxs-lookup"><span data-stu-id="fbff5-120">Header</span></span>       | <span data-ttu-id="fbff5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fbff5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fbff5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbff5-122">Authorization</span></span>  | <span data-ttu-id="fbff5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fbff5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbff5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fbff5-125">Request body</span></span>
<span data-ttu-id="fbff5-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fbff5-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fbff5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbff5-127">Response</span></span>
<span data-ttu-id="fbff5-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fbff5-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fbff5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fbff5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbff5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fbff5-130">Request</span></span>
<span data-ttu-id="fbff5-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fbff5-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/user
```
##### <a name="response"></a><span data-ttu-id="fbff5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fbff5-132">Response</span></span>
<span data-ttu-id="fbff5-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fbff5-133">The following is an example of the response.</span></span> 

><span data-ttu-id="fbff5-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="fbff5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
