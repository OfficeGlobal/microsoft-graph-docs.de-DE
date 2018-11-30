---
title: mobileAppContentFile aktualisieren
description: Aktualisieren der Eigenschaften eines MobileAppContentFile-Objekts.
ms.openlocfilehash: b3a25c3ccce6598f12d6742546cca0f61679a138
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016695"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="4cdeb-103">mobileAppContentFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4cdeb-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="4cdeb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4cdeb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cdeb-105">Aktualisieren der Eigenschaften eines [MobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4cdeb-105">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4cdeb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4cdeb-106">Prerequisites</span></span>
<span data-ttu-id="4cdeb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cdeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cdeb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4cdeb-109">Permission type</span></span>|<span data-ttu-id="4cdeb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4cdeb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cdeb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4cdeb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4cdeb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cdeb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4cdeb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4cdeb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cdeb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4cdeb-114">Not supported.</span></span>|
|<span data-ttu-id="4cdeb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4cdeb-115">Application</span></span>|<span data-ttu-id="4cdeb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4cdeb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cdeb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cdeb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="4cdeb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4cdeb-118">Request headers</span></span>
|<span data-ttu-id="4cdeb-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4cdeb-119">Header</span></span>|<span data-ttu-id="4cdeb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4cdeb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cdeb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cdeb-121">Authorization</span></span>|<span data-ttu-id="4cdeb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4cdeb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cdeb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4cdeb-123">Accept</span></span>|<span data-ttu-id="4cdeb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4cdeb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cdeb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4cdeb-125">Request body</span></span>
<span data-ttu-id="4cdeb-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) an.</span><span class="sxs-lookup"><span data-stu-id="4cdeb-126">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="4cdeb-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="4cdeb-127">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="4cdeb-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4cdeb-128">Property</span></span>|<span data-ttu-id="4cdeb-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4cdeb-129">Type</span></span>|<span data-ttu-id="4cdeb-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cdeb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cdeb-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="4cdeb-131">azureStorageUri</span></span>|<span data-ttu-id="4cdeb-132">String</span><span class="sxs-lookup"><span data-stu-id="4cdeb-132">String</span></span>|<span data-ttu-id="4cdeb-133">Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="4cdeb-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="4cdeb-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="4cdeb-134">isCommitted</span></span>|<span data-ttu-id="4cdeb-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cdeb-135">Boolean</span></span>|<span data-ttu-id="4cdeb-136">Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde</span><span class="sxs-lookup"><span data-stu-id="4cdeb-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="4cdeb-137">id</span><span class="sxs-lookup"><span data-stu-id="4cdeb-137">id</span></span>|<span data-ttu-id="4cdeb-138">String</span><span class="sxs-lookup"><span data-stu-id="4cdeb-138">String</span></span>|<span data-ttu-id="4cdeb-139">ID der Datei</span><span class="sxs-lookup"><span data-stu-id="4cdeb-139">The File Id.</span></span>|
|<span data-ttu-id="4cdeb-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cdeb-140">createdDateTime</span></span>|<span data-ttu-id="4cdeb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cdeb-141">DateTimeOffset</span></span>|<span data-ttu-id="4cdeb-142">Datum und Uhrzeit der Erstellung der Datei</span><span class="sxs-lookup"><span data-stu-id="4cdeb-142">The time the file was created.</span></span>|
|<span data-ttu-id="4cdeb-143">name</span><span class="sxs-lookup"><span data-stu-id="4cdeb-143">name</span></span>|<span data-ttu-id="4cdeb-144">String</span><span class="sxs-lookup"><span data-stu-id="4cdeb-144">String</span></span>|<span data-ttu-id="4cdeb-145">Name der Datei</span><span class="sxs-lookup"><span data-stu-id="4cdeb-145">the file name.</span></span>|
|<span data-ttu-id="4cdeb-146">size</span><span class="sxs-lookup"><span data-stu-id="4cdeb-146">size</span></span>|<span data-ttu-id="4cdeb-147">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdeb-147">Int64</span></span>|<span data-ttu-id="4cdeb-148">Größe der Datei vor der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="4cdeb-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="4cdeb-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="4cdeb-149">sizeEncrypted</span></span>|<span data-ttu-id="4cdeb-150">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdeb-150">Int64</span></span>|<span data-ttu-id="4cdeb-151">Größe der Datei nach der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="4cdeb-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="4cdeb-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4cdeb-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="4cdeb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cdeb-153">DateTimeOffset</span></span>|<span data-ttu-id="4cdeb-154">Datum und Uhrzeit des Ablaufs des Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="4cdeb-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="4cdeb-155">manifest</span><span class="sxs-lookup"><span data-stu-id="4cdeb-155">manifest</span></span>|<span data-ttu-id="4cdeb-156">Binär</span><span class="sxs-lookup"><span data-stu-id="4cdeb-156">Binary</span></span>|<span data-ttu-id="4cdeb-157">Manifestinformationen</span><span class="sxs-lookup"><span data-stu-id="4cdeb-157">The manifest information.</span></span>|
|<span data-ttu-id="4cdeb-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="4cdeb-158">uploadState</span></span>|[<span data-ttu-id="4cdeb-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="4cdeb-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="4cdeb-160">Status der aktuellen Uploadanforderung.</span><span class="sxs-lookup"><span data-stu-id="4cdeb-160">The state of the current upload request.</span></span> <span data-ttu-id="4cdeb-161">Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed` und `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="4cdeb-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="4cdeb-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cdeb-162">Response</span></span>
<span data-ttu-id="4cdeb-163">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cdeb-163">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cdeb-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4cdeb-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="4cdeb-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cdeb-165">Request</span></span>
<span data-ttu-id="4cdeb-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4cdeb-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```

### <a name="response"></a><span data-ttu-id="4cdeb-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cdeb-167">Response</span></span>
<span data-ttu-id="4cdeb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cdeb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```



