---
title: Abrufen von Einstellungen
description: Lesen Sie Benutzer- und Settings-Objekts.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 59685923c939dae2ae066a2e146398ea8f87a05c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943648"
---
# <a name="get-settings"></a><span data-ttu-id="501da-103">Abrufen von Einstellungen</span><span class="sxs-lookup"><span data-stu-id="501da-103">Get settings</span></span>

<span data-ttu-id="501da-104">Lesen Sie Benutzer- und [Settings](../resources/user-settings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="501da-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="501da-105">Weitere Informationen zum Aktualisieren der Eigenschaften des [Settings](../resources/user-settings.md) -Objekts finden Sie unter [Aktualisieren von benutzereinstellungen](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="501da-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="501da-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="501da-106">Permissions</span></span>

<span data-ttu-id="501da-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="501da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="501da-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="501da-109">Permission type</span></span>      | <span data-ttu-id="501da-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="501da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="501da-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="501da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="501da-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="501da-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="501da-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="501da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="501da-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="501da-114">Not supported.</span></span>    |
|<span data-ttu-id="501da-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="501da-115">Application</span></span> | <span data-ttu-id="501da-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="501da-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="501da-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="501da-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="501da-118">Fordern Sie mit einer 'Benutzer-Id"oder"UserPrincipalName"ist nur verfügbar, durch den Benutzer oder von einem Benutzer mit den Berechtigungen User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="501da-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="501da-119">Weitere Informationen finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="501da-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="501da-120">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="501da-120">Request body</span></span>

<span data-ttu-id="501da-121">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="501da-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="501da-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="501da-122">Response</span></span>

<span data-ttu-id="501da-123">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [Einstellungen](../resources/user-settings.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="501da-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="501da-124">Beispiel</span><span class="sxs-lookup"><span data-stu-id="501da-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="501da-125">Anforderung</span><span class="sxs-lookup"><span data-stu-id="501da-125">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="501da-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="501da-126">Response</span></span>

<span data-ttu-id="501da-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="501da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

