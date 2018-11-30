---
title: ImportDeviceIdentityList Aktion
description: Noch nicht dokumentiert
ms.openlocfilehash: a99b610e4a781aa6f11aec3517f06646f3b436ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058850"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="129a5-103">ImportDeviceIdentityList Aktion</span><span class="sxs-lookup"><span data-stu-id="129a5-103">importDeviceIdentityList action</span></span>

> <span data-ttu-id="129a5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="129a5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="129a5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="129a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="129a5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="129a5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="129a5-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="129a5-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="129a5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="129a5-108">Prerequisites</span></span>
<span data-ttu-id="129a5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="129a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="129a5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="129a5-111">Permission type</span></span>|<span data-ttu-id="129a5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="129a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="129a5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="129a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="129a5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="129a5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="129a5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="129a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="129a5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="129a5-116">Not supported.</span></span>|
|<span data-ttu-id="129a5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="129a5-117">Application</span></span>|<span data-ttu-id="129a5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="129a5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="129a5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="129a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="129a5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="129a5-120">Request headers</span></span>
|<span data-ttu-id="129a5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="129a5-121">Header</span></span>|<span data-ttu-id="129a5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="129a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="129a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="129a5-123">Authorization</span></span>|<span data-ttu-id="129a5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="129a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="129a5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="129a5-125">Accept</span></span>|<span data-ttu-id="129a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="129a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="129a5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="129a5-127">Request body</span></span>
<span data-ttu-id="129a5-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="129a5-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="129a5-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="129a5-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="129a5-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="129a5-130">Property</span></span>|<span data-ttu-id="129a5-131">Typ</span><span class="sxs-lookup"><span data-stu-id="129a5-131">Type</span></span>|<span data-ttu-id="129a5-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="129a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="129a5-133">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="129a5-133">importedDeviceIdentities</span></span>|<span data-ttu-id="129a5-134">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="129a5-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="129a5-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="129a5-135">Not yet documented</span></span>|
|<span data-ttu-id="129a5-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="129a5-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="129a5-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="129a5-137">Boolean</span></span>|<span data-ttu-id="129a5-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="129a5-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="129a5-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="129a5-139">Response</span></span>
<span data-ttu-id="129a5-140">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="129a5-140">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="129a5-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="129a5-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="129a5-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="129a5-142">Request</span></span>
<span data-ttu-id="129a5-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="129a5-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList

Content-type: application/json
Content-length: 642

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="129a5-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="129a5-144">Response</span></span>
<span data-ttu-id="129a5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="129a5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```





