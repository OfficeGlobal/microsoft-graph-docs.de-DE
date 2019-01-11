---
title: Liste iosVppAppAssignedDeviceLicenses
description: Listeneigenschaften und Beziehungen der IosVppAppAssignedDeviceLicense-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 611b4c317b3d2edb03ee89c272be9b4e2027d7fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833292"
---
# <a name="list-iosvppappassigneddevicelicenses"></a><span data-ttu-id="c57fc-103">Liste iosVppAppAssignedDeviceLicenses</span><span class="sxs-lookup"><span data-stu-id="c57fc-103">List iosVppAppAssignedDeviceLicenses</span></span>

> <span data-ttu-id="c57fc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c57fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c57fc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c57fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c57fc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c57fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c57fc-107">Listeneigenschaften und Beziehungen der [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="c57fc-107">List properties and relationships of the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c57fc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c57fc-108">Prerequisites</span></span>
<span data-ttu-id="c57fc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c57fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c57fc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c57fc-111">Permission type</span></span>|<span data-ttu-id="c57fc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c57fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c57fc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c57fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c57fc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c57fc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c57fc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c57fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c57fc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c57fc-116">Not supported.</span></span>|
|<span data-ttu-id="c57fc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c57fc-117">Application</span></span>|<span data-ttu-id="c57fc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c57fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c57fc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c57fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="c57fc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c57fc-120">Request headers</span></span>
|<span data-ttu-id="c57fc-121">Header</span><span class="sxs-lookup"><span data-stu-id="c57fc-121">Header</span></span>|<span data-ttu-id="c57fc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c57fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c57fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c57fc-123">Authorization</span></span>|<span data-ttu-id="c57fc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c57fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c57fc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c57fc-125">Accept</span></span>|<span data-ttu-id="c57fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c57fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c57fc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c57fc-127">Request body</span></span>
<span data-ttu-id="c57fc-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c57fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c57fc-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c57fc-129">Response</span></span>
<span data-ttu-id="c57fc-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .</span><span class="sxs-lookup"><span data-stu-id="c57fc-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c57fc-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c57fc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c57fc-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c57fc-132">Request</span></span>
<span data-ttu-id="c57fc-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c57fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="c57fc-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c57fc-134">Response</span></span>
<span data-ttu-id="c57fc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c57fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
      "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value"
    }
  ]
}
```





