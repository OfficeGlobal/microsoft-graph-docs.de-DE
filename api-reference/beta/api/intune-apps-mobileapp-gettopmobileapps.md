---
title: GetTopMobileApps-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f5a380145c51ba61fe76638941c42352f254606e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980209"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="df7bc-103">GetTopMobileApps-Funktion</span><span class="sxs-lookup"><span data-stu-id="df7bc-103">getTopMobileApps function</span></span>

> <span data-ttu-id="df7bc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df7bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df7bc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df7bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df7bc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="df7bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df7bc-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="df7bc-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df7bc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="df7bc-108">Prerequisites</span></span>
<span data-ttu-id="df7bc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df7bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df7bc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df7bc-111">Permission type</span></span>|<span data-ttu-id="df7bc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df7bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df7bc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df7bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df7bc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="df7bc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="df7bc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df7bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df7bc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df7bc-116">Not supported.</span></span>|
|<span data-ttu-id="df7bc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df7bc-117">Application</span></span>|<span data-ttu-id="df7bc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df7bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df7bc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df7bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="df7bc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="df7bc-120">Request headers</span></span>
|<span data-ttu-id="df7bc-121">Header</span><span class="sxs-lookup"><span data-stu-id="df7bc-121">Header</span></span>|<span data-ttu-id="df7bc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="df7bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df7bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df7bc-123">Authorization</span></span>|<span data-ttu-id="df7bc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="df7bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df7bc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="df7bc-125">Accept</span></span>|<span data-ttu-id="df7bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df7bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df7bc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df7bc-127">Request body</span></span>
<span data-ttu-id="df7bc-128">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="df7bc-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="df7bc-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="df7bc-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="df7bc-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df7bc-130">Property</span></span>|<span data-ttu-id="df7bc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="df7bc-131">Type</span></span>|<span data-ttu-id="df7bc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df7bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df7bc-133">status</span><span class="sxs-lookup"><span data-stu-id="df7bc-133">status</span></span>|<span data-ttu-id="df7bc-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df7bc-134">String</span></span>|<span data-ttu-id="df7bc-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="df7bc-135">Not yet documented</span></span>|
|<span data-ttu-id="df7bc-136">count</span><span class="sxs-lookup"><span data-stu-id="df7bc-136">count</span></span>|<span data-ttu-id="df7bc-137">Int64</span><span class="sxs-lookup"><span data-stu-id="df7bc-137">Int64</span></span>|<span data-ttu-id="df7bc-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="df7bc-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="df7bc-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="df7bc-139">Response</span></span>
<span data-ttu-id="df7bc-140">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [MobileApp](../resources/intune-apps-mobileapp.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="df7bc-140">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df7bc-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df7bc-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="df7bc-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="df7bc-142">Request</span></span>
<span data-ttu-id="df7bc-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="df7bc-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="df7bc-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="df7bc-144">Response</span></span>
<span data-ttu-id="df7bc-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df7bc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 881

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
      "publishingState": "processing"
    }
  ]
}
```





