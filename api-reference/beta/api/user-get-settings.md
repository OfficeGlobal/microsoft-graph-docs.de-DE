---
title: Abrufen von Einstellungen
description: Lesen Sie Benutzer- und Settings-Objekts.
author: dkershaw10
ms.openlocfilehash: 1cf2d621c6f9b8d483b017325ea87628ba388466
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351275"
---
# <a name="get-settings"></a><span data-ttu-id="33ef1-103">Abrufen von Einstellungen</span><span class="sxs-lookup"><span data-stu-id="33ef1-103">Get settings</span></span>

> <span data-ttu-id="33ef1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="33ef1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33ef1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33ef1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33ef1-106">Lesen Sie Benutzer- und [Settings](../resources/user-settings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="33ef1-106">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="33ef1-107">Weitere Informationen zum Aktualisieren der Eigenschaften des [Settings](../resources/user-settings.md) -Objekts finden Sie unter [Aktualisieren von benutzereinstellungen](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="33ef1-107">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="33ef1-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="33ef1-108">Permissions</span></span>

<span data-ttu-id="33ef1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33ef1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33ef1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33ef1-111">Permission type</span></span>      | <span data-ttu-id="33ef1-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33ef1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33ef1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33ef1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="33ef1-114">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33ef1-114">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="33ef1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33ef1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33ef1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33ef1-116">Not supported.</span></span>    |
|<span data-ttu-id="33ef1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33ef1-117">Application</span></span> | <span data-ttu-id="33ef1-118">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33ef1-118">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33ef1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33ef1-119">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="33ef1-120">Fordern Sie mit einer 'Benutzer-Id"oder"UserPrincipalName"ist nur verfügbar, durch den Benutzer oder von einem Benutzer mit den Berechtigungen User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="33ef1-120">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="33ef1-121">Weitere Informationen finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33ef1-121">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="33ef1-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33ef1-122">Request body</span></span>

<span data-ttu-id="33ef1-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="33ef1-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33ef1-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="33ef1-124">Response</span></span>

<span data-ttu-id="33ef1-125">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [Einstellungen](../resources/user-settings.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="33ef1-125">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33ef1-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33ef1-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="33ef1-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33ef1-127">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="33ef1-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="33ef1-128">Response</span></span>

<span data-ttu-id="33ef1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33ef1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
