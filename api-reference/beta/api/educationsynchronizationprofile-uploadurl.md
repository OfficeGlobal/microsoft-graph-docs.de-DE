---
title: 'EducationSynchronizationProfile: UploadUrl'
description: Abrufen einer gemeinsamen Zugriff Signatur (SAS) für das Hochladen von Quelldateien in Azure Blob-Speicher für ein bestimmtes Schule Synchronisierung Datenprofil im Mandanten. Das Token SAS hat eine Gültigkeit von einer Stunde.
author: mmast-msft
ms.openlocfilehash: 15a4536e21307067ac55783edd9eac675ae4144b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341062"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="97b5b-104">EducationSynchronizationProfile: UploadUrl</span><span class="sxs-lookup"><span data-stu-id="97b5b-104">educationSynchronizationProfile: uploadUrl</span></span>

> <span data-ttu-id="97b5b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="97b5b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97b5b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97b5b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97b5b-107">Abrufen einer gemeinsamen Zugriff Signatur (SAS) für das Hochladen von Quelldateien in Azure Blob-Speicher für eine bestimmte Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="97b5b-107">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="97b5b-108">Das Token SAS hat eine Gültigkeit von einer Stunde.</span><span class="sxs-lookup"><span data-stu-id="97b5b-108">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="97b5b-109">Der Upload wird nur für die [CSV-Datenanbieter](../resources/educationcsvdataprovider.md)URL bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="97b5b-109">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="97b5b-110">**Hinweis:** Verwenden Sie den Zugriff auf die Blob-Speicherung mit dem SAS-Token der [Azure-Speicher SDKs](https://github.com/search?q=org%3AAzure+azure-storage) oder [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span><span class="sxs-lookup"><span data-stu-id="97b5b-110">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="97b5b-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97b5b-111">Permissions</span></span>
<span data-ttu-id="97b5b-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97b5b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97b5b-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97b5b-114">Permission type</span></span> | <span data-ttu-id="97b5b-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97b5b-115">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="97b5b-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97b5b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="97b5b-117">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97b5b-117">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="97b5b-118">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="97b5b-118">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="97b5b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97b5b-119">Not supported.</span></span>|
|<span data-ttu-id="97b5b-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97b5b-120">Application</span></span>|<span data-ttu-id="97b5b-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97b5b-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97b5b-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97b5b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="97b5b-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97b5b-123">Request headers</span></span>
| <span data-ttu-id="97b5b-124">Name</span><span class="sxs-lookup"><span data-stu-id="97b5b-124">Name</span></span>       | <span data-ttu-id="97b5b-125">Typ</span><span class="sxs-lookup"><span data-stu-id="97b5b-125">Type</span></span> | <span data-ttu-id="97b5b-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97b5b-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97b5b-127">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="97b5b-127">Authorization</span></span>  | <span data-ttu-id="97b5b-128">string</span><span class="sxs-lookup"><span data-stu-id="97b5b-128">string</span></span>  | <span data-ttu-id="97b5b-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97b5b-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97b5b-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97b5b-131">Request body</span></span>
<span data-ttu-id="97b5b-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="97b5b-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="97b5b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="97b5b-133">Response</span></span>
<span data-ttu-id="97b5b-134">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine SAS-URL für die [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="97b5b-134">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="97b5b-135">Wenn weiterhin eine vorherige Anforderung verarbeitet wird, gibt diese Methode einen `409 Conflict` zurück, der angibt, dass der Upload gegenwärtig für die [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md)ausgeschlossen wird.</span><span class="sxs-lookup"><span data-stu-id="97b5b-135">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="97b5b-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97b5b-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97b5b-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97b5b-137">Request</span></span>
<span data-ttu-id="97b5b-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97b5b-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="97b5b-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="97b5b-139">Response</span></span>
<span data-ttu-id="97b5b-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="97b5b-140">The following is an example of the response.</span></span> 

><span data-ttu-id="97b5b-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="97b5b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
