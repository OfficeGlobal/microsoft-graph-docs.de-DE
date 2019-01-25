---
title: 'EducationSynchronizationProfile: UploadUrl'
description: Abrufen einer gemeinsamen Zugriff Signatur (SAS) für das Hochladen von Quelldateien in Azure Blob-Speicher für ein bestimmtes Schule Synchronisierung Datenprofil im Mandanten. Das Token SAS hat eine Gültigkeit von einer Stunde.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 74f37f5653147691c408cf83e3039920957352c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511597"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="9460c-104">EducationSynchronizationProfile: UploadUrl</span><span class="sxs-lookup"><span data-stu-id="9460c-104">educationSynchronizationProfile: uploadUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9460c-105">Abrufen einer gemeinsamen Zugriff Signatur (SAS) für das Hochladen von Quelldateien in Azure Blob-Speicher für eine bestimmte Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9460c-105">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="9460c-106">Das Token SAS hat eine Gültigkeit von einer Stunde.</span><span class="sxs-lookup"><span data-stu-id="9460c-106">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="9460c-107">Der Upload wird nur für die [CSV-Datenanbieter](../resources/educationcsvdataprovider.md)URL bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="9460c-107">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="9460c-108">**Hinweis:** Verwenden Sie den Zugriff auf die Blob-Speicherung mit dem SAS-Token der [Azure-Speicher SDKs](https://github.com/search?q=org%3AAzure+azure-storage) oder [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span><span class="sxs-lookup"><span data-stu-id="9460c-108">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="9460c-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9460c-109">Permissions</span></span>
<span data-ttu-id="9460c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9460c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9460c-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9460c-112">Permission type</span></span> | <span data-ttu-id="9460c-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9460c-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9460c-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9460c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9460c-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9460c-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="9460c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9460c-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9460c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9460c-117">Not supported.</span></span>|
|<span data-ttu-id="9460c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9460c-118">Application</span></span>|<span data-ttu-id="9460c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9460c-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9460c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9460c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="9460c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9460c-121">Request headers</span></span>
| <span data-ttu-id="9460c-122">Name</span><span class="sxs-lookup"><span data-stu-id="9460c-122">Name</span></span>       | <span data-ttu-id="9460c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="9460c-123">Type</span></span> | <span data-ttu-id="9460c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9460c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9460c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9460c-125">Authorization</span></span>  | <span data-ttu-id="9460c-126">string</span><span class="sxs-lookup"><span data-stu-id="9460c-126">string</span></span>  | <span data-ttu-id="9460c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9460c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9460c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9460c-129">Request body</span></span>
<span data-ttu-id="9460c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9460c-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9460c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9460c-131">Response</span></span>
<span data-ttu-id="9460c-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine SAS-URL für die [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9460c-132">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="9460c-133">Wenn weiterhin eine vorherige Anforderung verarbeitet wird, gibt diese Methode einen `409 Conflict` zurück, der angibt, dass der Upload gegenwärtig für die [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md)ausgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="9460c-133">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="9460c-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9460c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9460c-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9460c-135">Request</span></span>
<span data-ttu-id="9460c-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9460c-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="9460c-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="9460c-137">Response</span></span>
<span data-ttu-id="9460c-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9460c-138">The following is an example of the response.</span></span> 

><span data-ttu-id="9460c-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9460c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
