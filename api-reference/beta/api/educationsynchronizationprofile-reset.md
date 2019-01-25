---
title: Zurücksetzen Sie auf eine EducationSynchronizationProfile sync
description: Setzen Sie die Synchronisierung eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten zurück.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 502eb8d7afdc61926a024b7ddfbac5383a146622
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520410"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="2449a-103">Zurücksetzen Sie auf eine EducationSynchronizationProfile sync</span><span class="sxs-lookup"><span data-stu-id="2449a-103">Reset sync on an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2449a-104">Setzen Sie die Synchronisierung eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten zurück.</span><span class="sxs-lookup"><span data-stu-id="2449a-104">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="2449a-105">**Hinweis:** Dieser Vorgang wird durch die Synchronisierung neu starten.</span><span class="sxs-lookup"><span data-stu-id="2449a-105">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="2449a-106">Aufgetretenen werden gelöscht.</span><span class="sxs-lookup"><span data-stu-id="2449a-106">Any errors encountered will be deleted.</span></span> <span data-ttu-id="2449a-107">Keine Daten werden von Azure Active Directory (AD Azure) gelöscht.</span><span class="sxs-lookup"><span data-stu-id="2449a-107">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2449a-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2449a-108">Permissions</span></span>
<span data-ttu-id="2449a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2449a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2449a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2449a-111">Permission type</span></span> | <span data-ttu-id="2449a-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2449a-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="2449a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2449a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2449a-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2449a-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="2449a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2449a-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2449a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2449a-116">Not supported.</span></span>|
|<span data-ttu-id="2449a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2449a-117">Application</span></span>|<span data-ttu-id="2449a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2449a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2449a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2449a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="2449a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2449a-120">Request headers</span></span>
| <span data-ttu-id="2449a-121">Name</span><span class="sxs-lookup"><span data-stu-id="2449a-121">Name</span></span>       | <span data-ttu-id="2449a-122">Typ</span><span class="sxs-lookup"><span data-stu-id="2449a-122">Type</span></span> | <span data-ttu-id="2449a-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2449a-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2449a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2449a-124">Authorization</span></span>  | <span data-ttu-id="2449a-125">string</span><span class="sxs-lookup"><span data-stu-id="2449a-125">string</span></span>  | <span data-ttu-id="2449a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2449a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2449a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2449a-128">Request body</span></span>
<span data-ttu-id="2449a-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2449a-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2449a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2449a-130">Response</span></span>
<span data-ttu-id="2449a-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2449a-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2449a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2449a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2449a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2449a-133">Request</span></span>
<span data-ttu-id="2449a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2449a-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="2449a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2449a-135">Response</span></span>

<span data-ttu-id="2449a-136">Es ist keine Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2449a-136">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-reset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
