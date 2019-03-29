---
title: Gettopmobileappcount-Funktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68646ead33d9505522381ace92e5eeaa3e7b48ce
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974237"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="09191-103">Gettopmobileappcount-Funktion</span><span class="sxs-lookup"><span data-stu-id="09191-103">getTopMobileApps function</span></span>

> <span data-ttu-id="09191-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="09191-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09191-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="09191-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09191-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="09191-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09191-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="09191-107">Prerequisites</span></span>
<span data-ttu-id="09191-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09191-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09191-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09191-110">Permission type</span></span>|<span data-ttu-id="09191-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09191-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09191-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09191-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09191-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="09191-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="09191-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09191-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09191-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09191-115">Not supported.</span></span>|
|<span data-ttu-id="09191-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09191-116">Application</span></span>|<span data-ttu-id="09191-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09191-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09191-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09191-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="09191-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09191-119">Request headers</span></span>
|<span data-ttu-id="09191-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="09191-120">Header</span></span>|<span data-ttu-id="09191-121">Wert</span><span class="sxs-lookup"><span data-stu-id="09191-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09191-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09191-122">Authorization</span></span>|<span data-ttu-id="09191-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="09191-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09191-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="09191-124">Accept</span></span>|<span data-ttu-id="09191-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09191-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09191-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09191-126">Request body</span></span>
<span data-ttu-id="09191-127">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="09191-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="09191-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="09191-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="09191-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="09191-129">Property</span></span>|<span data-ttu-id="09191-130">Typ</span><span class="sxs-lookup"><span data-stu-id="09191-130">Type</span></span>|<span data-ttu-id="09191-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="09191-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09191-132">status</span><span class="sxs-lookup"><span data-stu-id="09191-132">status</span></span>|<span data-ttu-id="09191-133">String</span><span class="sxs-lookup"><span data-stu-id="09191-133">String</span></span>|<span data-ttu-id="09191-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="09191-134">Not yet documented</span></span>|
|<span data-ttu-id="09191-135">count</span><span class="sxs-lookup"><span data-stu-id="09191-135">count</span></span>|<span data-ttu-id="09191-136">Int64</span><span class="sxs-lookup"><span data-stu-id="09191-136">Int64</span></span>|<span data-ttu-id="09191-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="09191-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="09191-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="09191-138">Response</span></span>
<span data-ttu-id="09191-139">Bei erfolgreicher Ausführung gibt die Funktion den `200 OK` Antwortcode und eine [mobileApp](../resources/intune-apps-mobileapp.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="09191-139">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09191-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09191-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="09191-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09191-141">Request</span></span>
<span data-ttu-id="09191-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09191-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="09191-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="09191-143">Response</span></span>
<span data-ttu-id="09191-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09191-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 982

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




