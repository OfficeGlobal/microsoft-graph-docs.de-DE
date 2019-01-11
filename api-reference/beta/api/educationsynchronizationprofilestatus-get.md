---
title: Abrufen des Status eines educationSynchronizationProfile
description: Rufen Sie den Status eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten. Die Antwort wird den Status der auszuführenden Synchronisierung hingewiesen.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: f371d86d188068a90b3a9503adea12fd38ba8e8d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869953"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="83b35-104">Abrufen des Status eines educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="83b35-104">Get the status of an educationSynchronizationProfile</span></span>

> <span data-ttu-id="83b35-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="83b35-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83b35-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83b35-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="83b35-107">Rufen Sie den Status eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="83b35-107">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="83b35-108">Die Antwort wird den Status der auszuführenden Synchronisierung hingewiesen.</span><span class="sxs-lookup"><span data-stu-id="83b35-108">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="83b35-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="83b35-109">Permissions</span></span>
<span data-ttu-id="83b35-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83b35-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83b35-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="83b35-112">Permission type</span></span> | <span data-ttu-id="83b35-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="83b35-113">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="83b35-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="83b35-114">Delegated (work or school account)</span></span> | <span data-ttu-id="83b35-115">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83b35-115">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="83b35-116">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="83b35-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="83b35-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="83b35-117">Not supported.</span></span>|
|<span data-ttu-id="83b35-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="83b35-118">Application</span></span>| <span data-ttu-id="83b35-119">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b35-119">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83b35-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="83b35-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="83b35-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="83b35-121">Request headers</span></span>
| <span data-ttu-id="83b35-122">Name</span><span class="sxs-lookup"><span data-stu-id="83b35-122">Name</span></span>       | <span data-ttu-id="83b35-123">Typ</span><span class="sxs-lookup"><span data-stu-id="83b35-123">Type</span></span> | <span data-ttu-id="83b35-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83b35-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="83b35-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="83b35-125">Authorization</span></span>  | <span data-ttu-id="83b35-126">string</span><span class="sxs-lookup"><span data-stu-id="83b35-126">string</span></span>  | <span data-ttu-id="83b35-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="83b35-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83b35-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="83b35-129">Request body</span></span>
<span data-ttu-id="83b35-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="83b35-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="83b35-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="83b35-131">Response</span></span>
<span data-ttu-id="83b35-132">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines [Educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="83b35-132">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83b35-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="83b35-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83b35-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="83b35-134">Request</span></span>
<span data-ttu-id="83b35-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="83b35-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="83b35-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="83b35-136">Response</span></span>
<span data-ttu-id="83b35-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="83b35-137">The following is an example of the response.</span></span> 

><span data-ttu-id="83b35-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="83b35-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
```
