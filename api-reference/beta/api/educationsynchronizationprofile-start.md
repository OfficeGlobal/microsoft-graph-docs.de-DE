---
title: Nach dem Hochladen von Dateien in einer EducationSynchronizationProfile starten Sie Synchronisierung
description: Überprüfen Sie die Dateien auf einem bestimmten Schule Daten Synchronisierung Profil in den Mandanten hochgeladen. Wenn die Überprüfung erfolgreich ist, wird auf das Profil Synchronisierung starten. Andernfalls enthält die Antwort Fehler und Warnungen. Wenn die Antwort Fehler enthält, wird die Synchronisierung nicht gestartet. Wenn die Antwort nur Warnungen enthält, wird Synchronisierung starten.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 1447178e80d30058b415345aea83dce4390e6bcf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512353"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="7101a-107">Nach dem Hochladen von Dateien in einer EducationSynchronizationProfile starten Sie Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="7101a-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7101a-108">Überprüfen Sie die Dateien auf einem bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten hochgeladen.</span><span class="sxs-lookup"><span data-stu-id="7101a-108">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="7101a-109">Wenn die Überprüfung erfolgreich ist, wird auf das Profil Synchronisierung starten.</span><span class="sxs-lookup"><span data-stu-id="7101a-109">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="7101a-110">Andernfalls enthält die Antwort Fehler und Warnungen.</span><span class="sxs-lookup"><span data-stu-id="7101a-110">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="7101a-111">Wenn die Antwort Fehler enthält, wird die Synchronisierung nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="7101a-111">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="7101a-112">Wenn die Antwort nur Warnungen enthält, wird Synchronisierung starten.</span><span class="sxs-lookup"><span data-stu-id="7101a-112">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="7101a-113">**Hinweis:** Verwenden Sie diese Methode nur, wenn Sie der Datenanbieter vom Typ [Educationcsvdataprovider](../resources/educationcsvdataprovider.md)ist.</span><span class="sxs-lookup"><span data-stu-id="7101a-113">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="7101a-114">Darüber hinaus muss das Profil State-Eigenschaft bereitgestellt werden, bevor er gestartet werden kann.</span><span class="sxs-lookup"><span data-stu-id="7101a-114">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="7101a-115">Umfrage Profile-Objekts, um die State-Eigenschaft zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="7101a-115">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="7101a-116">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7101a-116">Permissions</span></span>
<span data-ttu-id="7101a-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7101a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7101a-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7101a-119">Permission type</span></span> | <span data-ttu-id="7101a-120">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7101a-120">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="7101a-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7101a-121">Delegated (work or school account)</span></span> | <span data-ttu-id="7101a-122">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7101a-122">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="7101a-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7101a-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7101a-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7101a-124">Not supported.</span></span>|
|<span data-ttu-id="7101a-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7101a-125">Application</span></span>|<span data-ttu-id="7101a-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7101a-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7101a-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7101a-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="7101a-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7101a-128">Request headers</span></span>
| <span data-ttu-id="7101a-129">Name</span><span class="sxs-lookup"><span data-stu-id="7101a-129">Name</span></span>       | <span data-ttu-id="7101a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="7101a-130">Type</span></span> | <span data-ttu-id="7101a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7101a-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7101a-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="7101a-132">Authorization</span></span>  | <span data-ttu-id="7101a-133">string</span><span class="sxs-lookup"><span data-stu-id="7101a-133">string</span></span>  | <span data-ttu-id="7101a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7101a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7101a-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7101a-136">Request body</span></span>
<span data-ttu-id="7101a-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7101a-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7101a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="7101a-138">Response</span></span>
<span data-ttu-id="7101a-139">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7101a-139">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="7101a-140">Wenn nicht erfolgreich ist, es gibt eine `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="7101a-140">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="7101a-141">Die Antwort enthält eine Auflistung von [EducationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) -Objekten im Rahmen des Antworttexts, wenn Fehler oder Warnungen gefunden wurden.</span><span class="sxs-lookup"><span data-stu-id="7101a-141">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="7101a-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7101a-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7101a-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7101a-143">Request</span></span>
<span data-ttu-id="7101a-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7101a-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a><span data-ttu-id="7101a-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="7101a-145">Response</span></span>
<span data-ttu-id="7101a-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7101a-146">Here is an example of the response.</span></span> 

><span data-ttu-id="7101a-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="7101a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2105

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/Collection(microsoft.graph.verificationMessage)",
    "value": [
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have missing data for the field - SIS ID"
        },
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have an invalid format for the field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "125 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "35 row(s) have referenced data not found in source. Field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "10 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "91 row(s) have referenced data not found in source. Field - SIS ID"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-start.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
