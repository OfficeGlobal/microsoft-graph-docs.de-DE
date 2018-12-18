---
title: Liste importedDeviceIdentityResults
description: Listeneigenschaften und Beziehungen der ImportedDeviceIdentityResult-Objekte.
author: tfitzmac
ms.openlocfilehash: e7d876c649d3f088d238e2fc804e61fbcddbf8b0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355601"
---
# <a name="list-importeddeviceidentityresults"></a><span data-ttu-id="576bf-103">Liste importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="576bf-103">List importedDeviceIdentityResults</span></span>

> <span data-ttu-id="576bf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="576bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="576bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="576bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="576bf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="576bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="576bf-107">Listeneigenschaften und Beziehungen der [ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="576bf-107">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="576bf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="576bf-108">Prerequisites</span></span>
<span data-ttu-id="576bf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="576bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="576bf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="576bf-111">Permission type</span></span>|<span data-ttu-id="576bf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="576bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="576bf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="576bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="576bf-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="576bf-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="576bf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="576bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="576bf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="576bf-116">Not supported.</span></span>|
|<span data-ttu-id="576bf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="576bf-117">Application</span></span>|<span data-ttu-id="576bf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="576bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="576bf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="576bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="576bf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="576bf-120">Request headers</span></span>
|<span data-ttu-id="576bf-121">Header</span><span class="sxs-lookup"><span data-stu-id="576bf-121">Header</span></span>|<span data-ttu-id="576bf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="576bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="576bf-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="576bf-123">Authorization</span></span>|<span data-ttu-id="576bf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="576bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="576bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="576bf-125">Accept</span></span>|<span data-ttu-id="576bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="576bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="576bf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="576bf-127">Request body</span></span>
<span data-ttu-id="576bf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="576bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="576bf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="576bf-129">Response</span></span>
<span data-ttu-id="576bf-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="576bf-130">If successful, this method returns a `200 OK` response code and a collection of [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="576bf-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="576bf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="576bf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="576bf-132">Request</span></span>
<span data-ttu-id="576bf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="576bf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="576bf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="576bf-134">Response</span></span>
<span data-ttu-id="576bf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="576bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





