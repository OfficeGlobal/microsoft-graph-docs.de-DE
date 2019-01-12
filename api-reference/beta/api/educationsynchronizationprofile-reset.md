---
title: Zurücksetzen Sie auf eine EducationSynchronizationProfile sync
description: Setzen Sie die Synchronisierung eines bestimmten Schule Daten Synchronisierungsprofils im Mandanten zurück.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e397a5d3a1a49cc827ed6ad72d1fc9fbeca01299
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984577"
---
# <a name="reset-sync-on-an-educationsynchronizationprofile"></a><span data-ttu-id="75d9c-103">Zurücksetzen Sie auf eine EducationSynchronizationProfile sync</span><span class="sxs-lookup"><span data-stu-id="75d9c-103">Reset sync on an educationSynchronizationProfile</span></span>

> <span data-ttu-id="75d9c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="75d9c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75d9c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="75d9c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75d9c-106">Setzen Sie die Synchronisierung eines bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten zurück.</span><span class="sxs-lookup"><span data-stu-id="75d9c-106">Reset the sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

> <span data-ttu-id="75d9c-107">**Hinweis:** Dieser Vorgang wird durch die Synchronisierung neu starten.</span><span class="sxs-lookup"><span data-stu-id="75d9c-107">**Note:** This operation will cause synchronization to restart.</span></span> <span data-ttu-id="75d9c-108">Aufgetretenen werden gelöscht.</span><span class="sxs-lookup"><span data-stu-id="75d9c-108">Any errors encountered will be deleted.</span></span> <span data-ttu-id="75d9c-109">Keine Daten werden von Azure Active Directory (AD Azure) gelöscht.</span><span class="sxs-lookup"><span data-stu-id="75d9c-109">No data will be deleted from Azure Active Directory (Azure AD).</span></span> 

## <a name="permissions"></a><span data-ttu-id="75d9c-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="75d9c-110">Permissions</span></span>
<span data-ttu-id="75d9c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75d9c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75d9c-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="75d9c-113">Permission type</span></span> | <span data-ttu-id="75d9c-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="75d9c-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="75d9c-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="75d9c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="75d9c-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75d9c-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="75d9c-117">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="75d9c-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="75d9c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75d9c-118">Not supported.</span></span>|
|<span data-ttu-id="75d9c-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="75d9c-119">Application</span></span>|<span data-ttu-id="75d9c-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="75d9c-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75d9c-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="75d9c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/reset
```

## <a name="request-headers"></a><span data-ttu-id="75d9c-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="75d9c-122">Request headers</span></span>
| <span data-ttu-id="75d9c-123">Name</span><span class="sxs-lookup"><span data-stu-id="75d9c-123">Name</span></span>       | <span data-ttu-id="75d9c-124">Typ</span><span class="sxs-lookup"><span data-stu-id="75d9c-124">Type</span></span> | <span data-ttu-id="75d9c-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="75d9c-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="75d9c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="75d9c-126">Authorization</span></span>  | <span data-ttu-id="75d9c-127">string</span><span class="sxs-lookup"><span data-stu-id="75d9c-127">string</span></span>  | <span data-ttu-id="75d9c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="75d9c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75d9c-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="75d9c-130">Request body</span></span>
<span data-ttu-id="75d9c-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="75d9c-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="75d9c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="75d9c-132">Response</span></span>
<span data-ttu-id="75d9c-133">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75d9c-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="75d9c-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="75d9c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75d9c-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="75d9c-135">Request</span></span>
<span data-ttu-id="75d9c-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="75d9c-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/reset
```

##### <a name="response"></a><span data-ttu-id="75d9c-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="75d9c-137">Response</span></span>

<span data-ttu-id="75d9c-138">Es ist keine Antworttext.</span><span class="sxs-lookup"><span data-stu-id="75d9c-138">There is no response body.</span></span>

<!-- {
  "blockType": "response",
  "name": "post_educationSynchronizationProfile_reset"
}-->
```
HTTP/1.1 200 OK
```
