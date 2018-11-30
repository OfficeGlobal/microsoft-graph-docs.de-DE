---
title: mobileAppContentFile aktualisieren
description: Aktualisieren der Eigenschaften eines MobileAppContentFile-Objekts.
ms.openlocfilehash: 224ebd8ad72dfd1b7e205354df17e87ed50eea62
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059071"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="d8e76-103">mobileAppContentFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d8e76-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="d8e76-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d8e76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8e76-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8e76-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8e76-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d8e76-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8e76-107">Aktualisieren der Eigenschaften eines [MobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d8e76-107">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8e76-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d8e76-108">Prerequisites</span></span>
<span data-ttu-id="d8e76-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8e76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8e76-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d8e76-111">Permission type</span></span>|<span data-ttu-id="d8e76-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d8e76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8e76-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d8e76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8e76-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e76-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8e76-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d8e76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8e76-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8e76-116">Not supported.</span></span>|
|<span data-ttu-id="d8e76-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d8e76-117">Application</span></span>|<span data-ttu-id="d8e76-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8e76-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8e76-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8e76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="d8e76-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d8e76-120">Request headers</span></span>
|<span data-ttu-id="d8e76-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d8e76-121">Header</span></span>|<span data-ttu-id="d8e76-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d8e76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8e76-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8e76-123">Authorization</span></span>|<span data-ttu-id="d8e76-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d8e76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8e76-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8e76-125">Accept</span></span>|<span data-ttu-id="d8e76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8e76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8e76-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d8e76-127">Request body</span></span>
<span data-ttu-id="d8e76-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) an.</span><span class="sxs-lookup"><span data-stu-id="d8e76-128">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="d8e76-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="d8e76-129">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="d8e76-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d8e76-130">Property</span></span>|<span data-ttu-id="d8e76-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d8e76-131">Type</span></span>|<span data-ttu-id="d8e76-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8e76-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e76-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="d8e76-133">azureStorageUri</span></span>|<span data-ttu-id="d8e76-134">String</span><span class="sxs-lookup"><span data-stu-id="d8e76-134">String</span></span>|<span data-ttu-id="d8e76-135">Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="d8e76-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="d8e76-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="d8e76-136">isCommitted</span></span>|<span data-ttu-id="d8e76-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8e76-137">Boolean</span></span>|<span data-ttu-id="d8e76-138">Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde</span><span class="sxs-lookup"><span data-stu-id="d8e76-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="d8e76-139">id</span><span class="sxs-lookup"><span data-stu-id="d8e76-139">id</span></span>|<span data-ttu-id="d8e76-140">String</span><span class="sxs-lookup"><span data-stu-id="d8e76-140">String</span></span>|<span data-ttu-id="d8e76-141">ID der Datei</span><span class="sxs-lookup"><span data-stu-id="d8e76-141">The File Id.</span></span>|
|<span data-ttu-id="d8e76-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e76-142">createdDateTime</span></span>|<span data-ttu-id="d8e76-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e76-143">DateTimeOffset</span></span>|<span data-ttu-id="d8e76-144">Datum und Uhrzeit der Erstellung der Datei</span><span class="sxs-lookup"><span data-stu-id="d8e76-144">The time the file was created.</span></span>|
|<span data-ttu-id="d8e76-145">name</span><span class="sxs-lookup"><span data-stu-id="d8e76-145">name</span></span>|<span data-ttu-id="d8e76-146">String</span><span class="sxs-lookup"><span data-stu-id="d8e76-146">String</span></span>|<span data-ttu-id="d8e76-147">Name der Datei</span><span class="sxs-lookup"><span data-stu-id="d8e76-147">the file name.</span></span>|
|<span data-ttu-id="d8e76-148">size</span><span class="sxs-lookup"><span data-stu-id="d8e76-148">size</span></span>|<span data-ttu-id="d8e76-149">Int64</span><span class="sxs-lookup"><span data-stu-id="d8e76-149">Int64</span></span>|<span data-ttu-id="d8e76-150">Größe der Datei vor der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="d8e76-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="d8e76-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="d8e76-151">sizeEncrypted</span></span>|<span data-ttu-id="d8e76-152">Int64</span><span class="sxs-lookup"><span data-stu-id="d8e76-152">Int64</span></span>|<span data-ttu-id="d8e76-153">Größe der Datei nach der Verschlüsselung</span><span class="sxs-lookup"><span data-stu-id="d8e76-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="d8e76-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e76-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="d8e76-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e76-155">DateTimeOffset</span></span>|<span data-ttu-id="d8e76-156">Datum und Uhrzeit des Ablaufs des Azure Storage-URI</span><span class="sxs-lookup"><span data-stu-id="d8e76-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="d8e76-157">manifest</span><span class="sxs-lookup"><span data-stu-id="d8e76-157">manifest</span></span>|<span data-ttu-id="d8e76-158">Binär</span><span class="sxs-lookup"><span data-stu-id="d8e76-158">Binary</span></span>|<span data-ttu-id="d8e76-159">Manifestinformationen</span><span class="sxs-lookup"><span data-stu-id="d8e76-159">The manifest information.</span></span>|
|<span data-ttu-id="d8e76-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="d8e76-160">uploadState</span></span>|[<span data-ttu-id="d8e76-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="d8e76-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="d8e76-162">Status der aktuellen Uploadanforderung.</span><span class="sxs-lookup"><span data-stu-id="d8e76-162">The state of the current upload request.</span></span> <span data-ttu-id="d8e76-163">Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed` und `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="d8e76-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="d8e76-164">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="d8e76-164">isFrameworkFile</span></span>|<span data-ttu-id="d8e76-165">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d8e76-165">Boolean</span></span>|<span data-ttu-id="d8e76-166">Ein Wert, der angibt, ob die Datei Framework handelt.</span><span class="sxs-lookup"><span data-stu-id="d8e76-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="d8e76-167">isDependency</span><span class="sxs-lookup"><span data-stu-id="d8e76-167">isDependency</span></span>|<span data-ttu-id="d8e76-168">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d8e76-168">Boolean</span></span>|<span data-ttu-id="d8e76-169">Gibt an, ob die Datei eine Abhängigkeit für die wichtigsten Inhaltsdatei ist.</span><span class="sxs-lookup"><span data-stu-id="d8e76-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="d8e76-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8e76-170">Response</span></span>
<span data-ttu-id="d8e76-171">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8e76-171">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8e76-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d8e76-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8e76-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8e76-173">Request</span></span>
<span data-ttu-id="d8e76-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d8e76-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 336

{
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```

### <a name="response"></a><span data-ttu-id="d8e76-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8e76-175">Response</span></span>
<span data-ttu-id="d8e76-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d8e76-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 503

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
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```





