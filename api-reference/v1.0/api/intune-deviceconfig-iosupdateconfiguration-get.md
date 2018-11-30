---
title: iosUpdateConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des iosUpdateConfiguration-Objekts.
ms.openlocfilehash: f6dfded1e1e809cb69ca976edd1fde31fd2937fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016176"
---
# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="994a9-103">iosUpdateConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="994a9-103">Get iosUpdateConfiguration</span></span>

> <span data-ttu-id="994a9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="994a9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="994a9-105">Lesen von Eigenschaften und Beziehungen des [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="994a9-105">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="994a9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="994a9-106">Prerequisites</span></span>
<span data-ttu-id="994a9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="994a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="994a9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="994a9-109">Permission type</span></span>|<span data-ttu-id="994a9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="994a9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="994a9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="994a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="994a9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="994a9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="994a9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="994a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="994a9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="994a9-114">Not supported.</span></span>|
|<span data-ttu-id="994a9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="994a9-115">Application</span></span>|<span data-ttu-id="994a9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="994a9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="994a9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="994a9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="994a9-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="994a9-118">Optional query parameters</span></span>
<span data-ttu-id="994a9-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="994a9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="994a9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="994a9-120">Request headers</span></span>
|<span data-ttu-id="994a9-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="994a9-121">Header</span></span>|<span data-ttu-id="994a9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="994a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="994a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="994a9-123">Authorization</span></span>|<span data-ttu-id="994a9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="994a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="994a9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="994a9-125">Accept</span></span>|<span data-ttu-id="994a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="994a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="994a9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="994a9-127">Request body</span></span>
<span data-ttu-id="994a9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="994a9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="994a9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="994a9-129">Response</span></span>
<span data-ttu-id="994a9-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="994a9-130">If successful, this method returns a `200 OK` response code and [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="994a9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="994a9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="994a9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="994a9-132">Request</span></span>
<span data-ttu-id="994a9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="994a9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="994a9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="994a9-134">Response</span></span>
<span data-ttu-id="994a9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="994a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6
  }
}
```



