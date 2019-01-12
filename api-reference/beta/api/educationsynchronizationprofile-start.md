---
title: Nach dem Hochladen von Dateien in einer EducationSynchronizationProfile starten Sie Synchronisierung
description: Überprüfen Sie die Dateien auf einem bestimmten Schule Daten Synchronisierung Profil in den Mandanten hochgeladen. Wenn die Überprüfung erfolgreich ist, wird auf das Profil Synchronisierung starten. Andernfalls enthält die Antwort Fehler und Warnungen. Wenn die Antwort Fehler enthält, wird die Synchronisierung nicht gestartet. Wenn die Antwort nur Warnungen enthält, wird Synchronisierung starten.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: efdc0863a1de58f7ebf46492b662e632972275c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915249"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="c97cd-107">Nach dem Hochladen von Dateien in einer EducationSynchronizationProfile starten Sie Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="c97cd-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

> <span data-ttu-id="c97cd-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c97cd-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c97cd-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c97cd-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c97cd-110">Überprüfen Sie die Dateien auf einem bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten hochgeladen.</span><span class="sxs-lookup"><span data-stu-id="c97cd-110">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="c97cd-111">Wenn die Überprüfung erfolgreich ist, wird auf das Profil Synchronisierung starten.</span><span class="sxs-lookup"><span data-stu-id="c97cd-111">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="c97cd-112">Andernfalls enthält die Antwort Fehler und Warnungen.</span><span class="sxs-lookup"><span data-stu-id="c97cd-112">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="c97cd-113">Wenn die Antwort Fehler enthält, wird die Synchronisierung nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="c97cd-113">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="c97cd-114">Wenn die Antwort nur Warnungen enthält, wird Synchronisierung starten.</span><span class="sxs-lookup"><span data-stu-id="c97cd-114">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="c97cd-115">**Hinweis:** Verwenden Sie diese Methode nur, wenn Sie der Datenanbieter vom Typ [Educationcsvdataprovider](../resources/educationcsvdataprovider.md)ist.</span><span class="sxs-lookup"><span data-stu-id="c97cd-115">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="c97cd-116">Darüber hinaus muss das Profil State-Eigenschaft bereitgestellt werden, bevor er gestartet werden kann.</span><span class="sxs-lookup"><span data-stu-id="c97cd-116">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="c97cd-117">Umfrage Profile-Objekts, um die State-Eigenschaft zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="c97cd-117">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="c97cd-118">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c97cd-118">Permissions</span></span>
<span data-ttu-id="c97cd-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c97cd-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c97cd-121">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c97cd-121">Permission type</span></span> | <span data-ttu-id="c97cd-122">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c97cd-122">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c97cd-123">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c97cd-123">Delegated (work or school account)</span></span> | <span data-ttu-id="c97cd-124">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c97cd-124">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c97cd-125">Delegierte (Persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="c97cd-125">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c97cd-126">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c97cd-126">Not supported.</span></span>|
|<span data-ttu-id="c97cd-127">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c97cd-127">Application</span></span>|<span data-ttu-id="c97cd-128">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c97cd-128">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c97cd-129">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c97cd-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="c97cd-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c97cd-130">Request headers</span></span>
| <span data-ttu-id="c97cd-131">Name</span><span class="sxs-lookup"><span data-stu-id="c97cd-131">Name</span></span>       | <span data-ttu-id="c97cd-132">Typ</span><span class="sxs-lookup"><span data-stu-id="c97cd-132">Type</span></span> | <span data-ttu-id="c97cd-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c97cd-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c97cd-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="c97cd-134">Authorization</span></span>  | <span data-ttu-id="c97cd-135">string</span><span class="sxs-lookup"><span data-stu-id="c97cd-135">string</span></span>  | <span data-ttu-id="c97cd-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c97cd-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c97cd-138">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c97cd-138">Request body</span></span>
<span data-ttu-id="c97cd-139">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c97cd-139">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c97cd-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="c97cd-140">Response</span></span>
<span data-ttu-id="c97cd-141">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c97cd-141">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="c97cd-142">Wenn nicht erfolgreich ist, es gibt eine `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="c97cd-142">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="c97cd-143">Die Antwort enthält eine Auflistung von [EducationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) -Objekten im Rahmen des Antworttexts, wenn Fehler oder Warnungen gefunden wurden.</span><span class="sxs-lookup"><span data-stu-id="c97cd-143">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="c97cd-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c97cd-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c97cd-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c97cd-145">Request</span></span>
<span data-ttu-id="c97cd-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c97cd-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a><span data-ttu-id="c97cd-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="c97cd-147">Response</span></span>
<span data-ttu-id="c97cd-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c97cd-148">Here is an example of the response.</span></span> 

><span data-ttu-id="c97cd-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="c97cd-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
