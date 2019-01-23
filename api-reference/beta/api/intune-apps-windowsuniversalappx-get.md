---
title: Abrufen von „windowsUniversalAppX“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windowsUniversalAppX.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 25569c8362c3488b782ee0b34b3e69bccecf246f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409202"
---
# <a name="get-windowsuniversalappx"></a><span data-ttu-id="f1726-103">Abrufen von „windowsUniversalAppX“</span><span class="sxs-lookup"><span data-stu-id="f1726-103">Get windowsUniversalAppX</span></span>

> <span data-ttu-id="f1726-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f1726-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f1726-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1726-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1726-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f1726-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1726-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="f1726-107">Read properties and relationships of the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1726-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1726-108">Prerequisites</span></span>
<span data-ttu-id="f1726-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1726-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f1726-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1726-111">Permission type</span></span>|<span data-ttu-id="f1726-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1726-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1726-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1726-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1726-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1726-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f1726-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1726-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1726-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1726-116">Not supported.</span></span>|
|<span data-ttu-id="f1726-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1726-117">Application</span></span>|<span data-ttu-id="f1726-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1726-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1726-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1726-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1726-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f1726-120">Optional query parameters</span></span>
<span data-ttu-id="f1726-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f1726-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1726-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1726-122">Request headers</span></span>
|<span data-ttu-id="f1726-123">Header</span><span class="sxs-lookup"><span data-stu-id="f1726-123">Header</span></span>|<span data-ttu-id="f1726-124">Wert</span><span class="sxs-lookup"><span data-stu-id="f1726-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1726-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f1726-125">Authorization</span></span>|<span data-ttu-id="f1726-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1726-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1726-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f1726-127">Accept</span></span>|<span data-ttu-id="f1726-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f1726-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1726-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1726-129">Request body</span></span>
<span data-ttu-id="f1726-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f1726-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1726-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1726-131">Response</span></span>
<span data-ttu-id="f1726-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f1726-132">If successful, this method returns a `200 OK` response code and [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1726-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1726-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1726-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1726-134">Request</span></span>
<span data-ttu-id="f1726-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1726-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f1726-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1726-136">Response</span></span>
<span data-ttu-id="f1726-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1726-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




