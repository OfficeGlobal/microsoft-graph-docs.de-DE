---
title: mobileLobApp abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des mobileLobApp-Objekts auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d7f51ddcdea56a80cb8b04ad444e9ba05702f78c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401691"
---
# <a name="get-mobilelobapp"></a><span data-ttu-id="6fc1e-103">mobileLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="6fc1e-103">Get mobileLobApp</span></span>

> <span data-ttu-id="6fc1e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6fc1e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6fc1e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6fc1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fc1e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6fc1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fc1e-107">Liest die Eigenschaften und Beziehungen von Objekten des [mobileLobApp](../resources/intune-apps-mobilelobapp.md)-Objekts auf.</span><span class="sxs-lookup"><span data-stu-id="6fc1e-107">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fc1e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6fc1e-108">Prerequisites</span></span>
<span data-ttu-id="6fc1e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6fc1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6fc1e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6fc1e-111">Permission type</span></span>|<span data-ttu-id="6fc1e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6fc1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fc1e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6fc1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6fc1e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fc1e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6fc1e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6fc1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fc1e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fc1e-116">Not supported.</span></span>|
|<span data-ttu-id="6fc1e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6fc1e-117">Application</span></span>|<span data-ttu-id="6fc1e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6fc1e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fc1e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fc1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6fc1e-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6fc1e-120">Optional query parameters</span></span>
<span data-ttu-id="6fc1e-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6fc1e-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6fc1e-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6fc1e-122">Request headers</span></span>
|<span data-ttu-id="6fc1e-123">Header</span><span class="sxs-lookup"><span data-stu-id="6fc1e-123">Header</span></span>|<span data-ttu-id="6fc1e-124">Wert</span><span class="sxs-lookup"><span data-stu-id="6fc1e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fc1e-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6fc1e-125">Authorization</span></span>|<span data-ttu-id="6fc1e-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6fc1e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fc1e-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6fc1e-127">Accept</span></span>|<span data-ttu-id="6fc1e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6fc1e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fc1e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6fc1e-129">Request body</span></span>
<span data-ttu-id="6fc1e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6fc1e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fc1e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fc1e-131">Response</span></span>
<span data-ttu-id="6fc1e-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [mobileLobApp](../resources/intune-apps-mobilelobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6fc1e-132">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fc1e-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6fc1e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fc1e-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6fc1e-134">Request</span></span>
<span data-ttu-id="6fc1e-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6fc1e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="6fc1e-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6fc1e-136">Response</span></span>
<span data-ttu-id="6fc1e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6fc1e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1042

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileLobApp",
    "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
    "size": 4
  }
}
```




