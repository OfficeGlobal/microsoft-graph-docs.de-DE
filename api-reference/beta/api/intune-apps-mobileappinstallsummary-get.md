---
title: MobileAppInstallSummary abrufen
description: Lesen von Eigenschaften und Beziehungen des mobileAppInstallSummary-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2434c61d4d52b1953600d0a2c171b63b8ee39146
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986572"
---
# <a name="get-mobileappinstallsummary"></a><span data-ttu-id="ef615-103">MobileAppInstallSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="ef615-103">Get mobileAppInstallSummary</span></span>

> <span data-ttu-id="ef615-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ef615-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef615-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ef615-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef615-106">Lesen von Eigenschaften und Beziehungen des [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ef615-106">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef615-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ef615-107">Prerequisites</span></span>
<span data-ttu-id="ef615-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef615-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef615-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef615-110">Permission type</span></span>|<span data-ttu-id="ef615-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef615-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef615-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef615-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef615-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef615-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ef615-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef615-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef615-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef615-115">Not supported.</span></span>|
|<span data-ttu-id="ef615-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef615-116">Application</span></span>|<span data-ttu-id="ef615-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef615-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef615-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef615-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef615-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ef615-119">Optional query parameters</span></span>
<span data-ttu-id="ef615-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef615-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef615-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef615-121">Request headers</span></span>
|<span data-ttu-id="ef615-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ef615-122">Header</span></span>|<span data-ttu-id="ef615-123">Wert</span><span class="sxs-lookup"><span data-stu-id="ef615-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef615-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef615-124">Authorization</span></span>|<span data-ttu-id="ef615-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ef615-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef615-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ef615-126">Accept</span></span>|<span data-ttu-id="ef615-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ef615-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef615-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef615-128">Request body</span></span>
<span data-ttu-id="ef615-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ef615-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef615-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef615-130">Response</span></span>
<span data-ttu-id="ef615-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ef615-131">If successful, this method returns a `200 OK` response code and [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef615-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef615-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef615-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef615-133">Request</span></span>
<span data-ttu-id="ef615-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef615-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

### <a name="response"></a><span data-ttu-id="ef615-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef615-135">Response</span></span>
<span data-ttu-id="ef615-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef615-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 466

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
    "id": "06a792e9-92e9-06a7-e992-a706e992a706",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notApplicableDeviceCount": 8,
    "notInstalledDeviceCount": 7,
    "pendingInstallDeviceCount": 9,
    "installedUserCount": 2,
    "failedUserCount": 15,
    "notApplicableUserCount": 6,
    "notInstalledUserCount": 5,
    "pendingInstallUserCount": 7
  }
}
```




