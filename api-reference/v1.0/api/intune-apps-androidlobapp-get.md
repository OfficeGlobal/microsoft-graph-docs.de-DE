---
title: androidLobApp abrufen
description: Lesen von Eigenschaften und Beziehungen des androidLobApp-Objekts.
ms.openlocfilehash: 191f8ee543bedb09704fb58f81d4053d17fb3a87
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017291"
---
# <a name="get-androidlobapp"></a><span data-ttu-id="ffc18-103">androidLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="ffc18-103">Get androidLobApp</span></span>

> <span data-ttu-id="ffc18-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ffc18-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffc18-105">Lesen von Eigenschaften und Beziehungen des [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ffc18-105">Read properties and relationships of the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffc18-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ffc18-106">Prerequisites</span></span>
<span data-ttu-id="ffc18-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffc18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffc18-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ffc18-109">Permission type</span></span>|<span data-ttu-id="ffc18-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ffc18-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffc18-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ffc18-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ffc18-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ffc18-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ffc18-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ffc18-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffc18-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffc18-114">Not supported.</span></span>|
|<span data-ttu-id="ffc18-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ffc18-115">Application</span></span>|<span data-ttu-id="ffc18-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ffc18-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffc18-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffc18-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffc18-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ffc18-118">Optional query parameters</span></span>
<span data-ttu-id="ffc18-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ffc18-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ffc18-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ffc18-120">Request headers</span></span>
|<span data-ttu-id="ffc18-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ffc18-121">Header</span></span>|<span data-ttu-id="ffc18-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ffc18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffc18-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffc18-123">Authorization</span></span>|<span data-ttu-id="ffc18-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ffc18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffc18-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffc18-125">Accept</span></span>|<span data-ttu-id="ffc18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffc18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffc18-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ffc18-127">Request body</span></span>
<span data-ttu-id="ffc18-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ffc18-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffc18-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffc18-129">Response</span></span>
<span data-ttu-id="ffc18-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [androidLobApp](../resources/intune-apps-androidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffc18-130">If successful, this method returns a `200 OK` response code and [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffc18-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ffc18-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffc18-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ffc18-132">Request</span></span>
<span data-ttu-id="ffc18-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ffc18-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="ffc18-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ffc18-134">Response</span></span>
<span data-ttu-id="ffc18-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ffc18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1338

{
  "value": {
    "@odata.type": "#microsoft.graph.androidLobApp",
    "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
    "publishingState": "processing",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "packageId": "Package Id value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true
    },
    "versionName": "Version Name value",
    "versionCode": "Version Code value"
  }
}
```


