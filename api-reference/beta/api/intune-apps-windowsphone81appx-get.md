---
title: WindowsPhone81AppX abrufen
description: Lesen von Eigenschaften und Beziehungen des windowsPhone81AppX-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ade6a396f00f4b8bbf53ef18d494e77805fedffc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976225"
---
# <a name="get-windowsphone81appx"></a><span data-ttu-id="0c488-103">WindowsPhone81AppX abrufen</span><span class="sxs-lookup"><span data-stu-id="0c488-103">Get windowsPhone81AppX</span></span>

> <span data-ttu-id="0c488-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c488-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c488-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0c488-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c488-106">Lesen von Eigenschaften und Beziehungen des [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c488-106">Read properties and relationships of the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c488-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0c488-107">Prerequisites</span></span>
<span data-ttu-id="0c488-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c488-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c488-110">Permission type</span></span>|<span data-ttu-id="0c488-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c488-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c488-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c488-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c488-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c488-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0c488-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c488-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c488-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c488-115">Not supported.</span></span>|
|<span data-ttu-id="0c488-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c488-116">Application</span></span>|<span data-ttu-id="0c488-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c488-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c488-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c488-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c488-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0c488-119">Optional query parameters</span></span>
<span data-ttu-id="0c488-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0c488-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c488-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c488-121">Request headers</span></span>
|<span data-ttu-id="0c488-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0c488-122">Header</span></span>|<span data-ttu-id="0c488-123">Wert</span><span class="sxs-lookup"><span data-stu-id="0c488-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c488-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c488-124">Authorization</span></span>|<span data-ttu-id="0c488-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0c488-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c488-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0c488-126">Accept</span></span>|<span data-ttu-id="0c488-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0c488-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c488-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c488-128">Request body</span></span>
<span data-ttu-id="0c488-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0c488-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c488-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c488-130">Response</span></span>
<span data-ttu-id="0c488-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0c488-131">If successful, this method returns a `200 OK` response code and [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c488-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c488-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c488-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c488-133">Request</span></span>
<span data-ttu-id="0c488-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c488-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="0c488-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c488-135">Response</span></span>
<span data-ttu-id="0c488-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c488-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1719

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81AppX",
    "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
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
    "phoneProductIdentifier": "Phone Product Identifier value",
    "phonePublisherId": "Phone Publisher Id value",
    "identityVersion": "Identity Version value"
  }
}
```




