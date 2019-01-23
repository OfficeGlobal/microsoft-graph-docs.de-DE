---
title: Auflisten von „iosLobApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosLobApp auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 259f90a990b4ada50ae2106bddf266d16a30e76b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421522"
---
# <a name="list-ioslobapps"></a><span data-ttu-id="43fcf-103">Auflisten von „iosLobApp“</span><span class="sxs-lookup"><span data-stu-id="43fcf-103">List iosLobApps</span></span>

> <span data-ttu-id="43fcf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="43fcf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43fcf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43fcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43fcf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="43fcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43fcf-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosLobApp](../resources/intune-apps-ioslobapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="43fcf-107">List properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43fcf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="43fcf-108">Prerequisites</span></span>
<span data-ttu-id="43fcf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="43fcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="43fcf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43fcf-111">Permission type</span></span>|<span data-ttu-id="43fcf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43fcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43fcf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43fcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43fcf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43fcf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="43fcf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43fcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43fcf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43fcf-116">Not supported.</span></span>|
|<span data-ttu-id="43fcf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43fcf-117">Application</span></span>|<span data-ttu-id="43fcf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43fcf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43fcf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43fcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="43fcf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43fcf-120">Request headers</span></span>
|<span data-ttu-id="43fcf-121">Header</span><span class="sxs-lookup"><span data-stu-id="43fcf-121">Header</span></span>|<span data-ttu-id="43fcf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="43fcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43fcf-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="43fcf-123">Authorization</span></span>|<span data-ttu-id="43fcf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="43fcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43fcf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="43fcf-125">Accept</span></span>|<span data-ttu-id="43fcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43fcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43fcf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43fcf-127">Request body</span></span>
<span data-ttu-id="43fcf-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="43fcf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43fcf-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="43fcf-129">Response</span></span>
<span data-ttu-id="43fcf-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosLobApp](../resources/intune-apps-ioslobapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="43fcf-130">If successful, this method returns a `200 OK` response code and a collection of [iosLobApp](../resources/intune-apps-ioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43fcf-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43fcf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="43fcf-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43fcf-132">Request</span></span>
<span data-ttu-id="43fcf-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43fcf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="43fcf-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="43fcf-134">Response</span></span>
<span data-ttu-id="43fcf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43fcf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1749

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosLobApp",
      "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
      "bundleId": "Bundle Id value",
      "applicableDeviceType": {
        "@odata.type": "microsoft.graph.iosDeviceType",
        "iPad": true,
        "iPhoneAndIPod": true
      },
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
        "v8_0": true,
        "v9_0": true,
        "v10_0": true,
        "v11_0": true,
        "v12_0": true
      },
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "versionNumber": "Version Number value",
      "buildNumber": "Build Number value",
      "identityVersion": "Identity Version value"
    }
  ]
}
```




