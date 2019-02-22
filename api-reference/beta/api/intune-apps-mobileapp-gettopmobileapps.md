---
title: Gettopmobileappcount-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e233feb9966fc90a56f38eff91c6bdab141b7462
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169727"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="b99b2-103">Gettopmobileappcount-Funktion</span><span class="sxs-lookup"><span data-stu-id="b99b2-103">getTopMobileApps function</span></span>

> <span data-ttu-id="b99b2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b99b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b99b2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b99b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b99b2-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b99b2-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b99b2-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b99b2-107">Prerequisites</span></span>
<span data-ttu-id="b99b2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b99b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b99b2-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b99b2-110">Permission type</span></span>|<span data-ttu-id="b99b2-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b99b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b99b2-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b99b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b99b2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99b2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b99b2-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b99b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b99b2-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b99b2-115">Not supported.</span></span>|
|<span data-ttu-id="b99b2-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b99b2-116">Application</span></span>|<span data-ttu-id="b99b2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b99b2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b99b2-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b99b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b99b2-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b99b2-119">Request headers</span></span>
|<span data-ttu-id="b99b2-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b99b2-120">Header</span></span>|<span data-ttu-id="b99b2-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b99b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b99b2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b99b2-122">Authorization</span></span>|<span data-ttu-id="b99b2-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b99b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b99b2-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b99b2-124">Accept</span></span>|<span data-ttu-id="b99b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b99b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b99b2-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b99b2-126">Request body</span></span>
<span data-ttu-id="b99b2-127">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="b99b2-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b99b2-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b99b2-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b99b2-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b99b2-129">Property</span></span>|<span data-ttu-id="b99b2-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b99b2-130">Type</span></span>|<span data-ttu-id="b99b2-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b99b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b99b2-132">status</span><span class="sxs-lookup"><span data-stu-id="b99b2-132">status</span></span>|<span data-ttu-id="b99b2-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b99b2-133">String</span></span>|<span data-ttu-id="b99b2-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b99b2-134">Not yet documented</span></span>|
|<span data-ttu-id="b99b2-135">count</span><span class="sxs-lookup"><span data-stu-id="b99b2-135">count</span></span>|<span data-ttu-id="b99b2-136">Int64</span><span class="sxs-lookup"><span data-stu-id="b99b2-136">Int64</span></span>|<span data-ttu-id="b99b2-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="b99b2-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b99b2-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="b99b2-138">Response</span></span>
<span data-ttu-id="b99b2-139">Bei erfolgreicher Ausführung gibt die Funktion den `200 OK` Antwortcode und eine [mobileApp](../resources/intune-apps-mobileapp.md) -Auflistung im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b99b2-139">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b99b2-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b99b2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b99b2-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b99b2-141">Request</span></span>
<span data-ttu-id="b99b2-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b99b2-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="b99b2-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b99b2-143">Response</span></span>
<span data-ttu-id="b99b2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b99b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




