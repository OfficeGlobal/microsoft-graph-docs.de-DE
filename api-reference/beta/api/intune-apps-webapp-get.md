---
title: webApp abrufen
description: Lesen von Eigenschaften und Beziehungen des webApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f207fd157fa02b2c3eecc85ff02ab5094faf3145
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394019"
---
# <a name="get-webapp"></a><span data-ttu-id="e765a-103">webApp abrufen</span><span class="sxs-lookup"><span data-stu-id="e765a-103">Get webApp</span></span>

> <span data-ttu-id="e765a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e765a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e765a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e765a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e765a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e765a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e765a-107">Lesen von Eigenschaften und Beziehungen des [webApp](../resources/intune-apps-webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e765a-107">Read properties and relationships of the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e765a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e765a-108">Prerequisites</span></span>
<span data-ttu-id="e765a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e765a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e765a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e765a-111">Permission type</span></span>|<span data-ttu-id="e765a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e765a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e765a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e765a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e765a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e765a-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e765a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e765a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e765a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e765a-116">Not supported.</span></span>|
|<span data-ttu-id="e765a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e765a-117">Application</span></span>|<span data-ttu-id="e765a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e765a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e765a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e765a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e765a-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e765a-120">Optional query parameters</span></span>
<span data-ttu-id="e765a-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e765a-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e765a-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e765a-122">Request headers</span></span>
|<span data-ttu-id="e765a-123">Header</span><span class="sxs-lookup"><span data-stu-id="e765a-123">Header</span></span>|<span data-ttu-id="e765a-124">Wert</span><span class="sxs-lookup"><span data-stu-id="e765a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e765a-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e765a-125">Authorization</span></span>|<span data-ttu-id="e765a-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e765a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e765a-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e765a-127">Accept</span></span>|<span data-ttu-id="e765a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e765a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e765a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e765a-129">Request body</span></span>
<span data-ttu-id="e765a-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e765a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e765a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e765a-131">Response</span></span>
<span data-ttu-id="e765a-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [webApp](../resources/intune-apps-webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e765a-132">If successful, this method returns a `200 OK` response code and [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e765a-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e765a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e765a-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e765a-134">Request</span></span>
<span data-ttu-id="e765a-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e765a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="e765a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e765a-136">Response</span></span>
<span data-ttu-id="e765a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e765a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 995

{
  "value": {
    "@odata.type": "#microsoft.graph.webApp",
    "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
    "appUrl": "https://example.com/appUrl/",
    "useManagedBrowser": true
  }
}
```




