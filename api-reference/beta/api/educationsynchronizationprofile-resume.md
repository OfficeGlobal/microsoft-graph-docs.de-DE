---
title: Sync auf ein EducationSynchronizationProfile fortsetzen
description: Setzen Sie die Synchronisierung eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten fort.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 50ffcb4ceab401a3041ecb69baa1de0409be94a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513256"
---
# <a name="resume-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="0f45b-103">Sync auf ein EducationSynchronizationProfile fortsetzen</span><span class="sxs-lookup"><span data-stu-id="0f45b-103">Resume sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f45b-104">Setzen Sie die Synchronisierung eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten fort.</span><span class="sxs-lookup"><span data-stu-id="0f45b-104">Resume the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f45b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0f45b-105">Permissions</span></span>
<span data-ttu-id="0f45b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f45b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f45b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f45b-108">Permission type</span></span> | <span data-ttu-id="0f45b-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0f45b-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="0f45b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f45b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f45b-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f45b-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="0f45b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f45b-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0f45b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f45b-113">Not supported.</span></span>|
|<span data-ttu-id="0f45b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f45b-114">Application</span></span>|<span data-ttu-id="0f45b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f45b-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f45b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f45b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/resume
```

## <a name="request-headers"></a><span data-ttu-id="0f45b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f45b-117">Request headers</span></span>
| <span data-ttu-id="0f45b-118">Name</span><span class="sxs-lookup"><span data-stu-id="0f45b-118">Name</span></span>       | <span data-ttu-id="0f45b-119">Typ</span><span class="sxs-lookup"><span data-stu-id="0f45b-119">Type</span></span> | <span data-ttu-id="0f45b-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f45b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0f45b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f45b-121">Authorization</span></span>  | <span data-ttu-id="0f45b-122">string</span><span class="sxs-lookup"><span data-stu-id="0f45b-122">string</span></span>  | <span data-ttu-id="0f45b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f45b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f45b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f45b-125">Request body</span></span>
<span data-ttu-id="0f45b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0f45b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0f45b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f45b-127">Response</span></span>
<span data-ttu-id="0f45b-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f45b-128">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0f45b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f45b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f45b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f45b-130">Request</span></span>
<span data-ttu-id="0f45b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f45b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/resume
```

##### <a name="response"></a><span data-ttu-id="0f45b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f45b-132">Response</span></span>

<span data-ttu-id="0f45b-133">Es ist keine Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0f45b-133">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_resume"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-resume.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
