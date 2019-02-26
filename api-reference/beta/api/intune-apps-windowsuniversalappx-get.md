---
title: Abrufen von „windowsUniversalAppX“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windowsUniversalAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01a2fc7b37d425374323f625534d3fe7e9567b4f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165240"
---
# <a name="get-windowsuniversalappx"></a><span data-ttu-id="244d0-103">Abrufen von „windowsUniversalAppX“</span><span class="sxs-lookup"><span data-stu-id="244d0-103">Get windowsUniversalAppX</span></span>

> <span data-ttu-id="244d0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="244d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="244d0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="244d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="244d0-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="244d0-106">Read properties and relationships of the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="244d0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="244d0-107">Prerequisites</span></span>
<span data-ttu-id="244d0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="244d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="244d0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="244d0-110">Permission type</span></span>|<span data-ttu-id="244d0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="244d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="244d0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="244d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="244d0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="244d0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="244d0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="244d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="244d0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="244d0-115">Not supported.</span></span>|
|<span data-ttu-id="244d0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="244d0-116">Application</span></span>|<span data-ttu-id="244d0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="244d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="244d0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="244d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="244d0-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="244d0-119">Optional query parameters</span></span>
<span data-ttu-id="244d0-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="244d0-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="244d0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="244d0-121">Request headers</span></span>
|<span data-ttu-id="244d0-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="244d0-122">Header</span></span>|<span data-ttu-id="244d0-123">Wert</span><span class="sxs-lookup"><span data-stu-id="244d0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="244d0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="244d0-124">Authorization</span></span>|<span data-ttu-id="244d0-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="244d0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="244d0-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="244d0-126">Accept</span></span>|<span data-ttu-id="244d0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="244d0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="244d0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="244d0-128">Request body</span></span>
<span data-ttu-id="244d0-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="244d0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="244d0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="244d0-130">Response</span></span>
<span data-ttu-id="244d0-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="244d0-131">If successful, this method returns a `200 OK` response code and [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="244d0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="244d0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="244d0-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="244d0-133">Request</span></span>
<span data-ttu-id="244d0-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="244d0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="244d0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="244d0-135">Response</span></span>
<span data-ttu-id="244d0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="244d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1667

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUniversalAppX",
    "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
    ],
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "applicableArchitectures": "x86",
    "applicableDeviceTypes": "desktop",
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
    "isBundle": true,
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true,
      "v10_1607": true,
      "v10_1703": true,
      "v10_1709": true,
      "v10_1803": true
    },
    "identityVersion": "Identity Version value"
  }
}
```




