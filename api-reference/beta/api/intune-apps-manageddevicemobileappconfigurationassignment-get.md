---
title: managedDeviceMobileAppConfigurationAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des managedDeviceMobileAppConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3bcd0e90933a44bab21fba693429fe048e7acdf
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982917"
---
# <a name="get-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="43104-103">managedDeviceMobileAppConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="43104-103">Get managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="43104-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43104-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43104-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="43104-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43104-106">Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="43104-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43104-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="43104-107">Prerequisites</span></span>
<span data-ttu-id="43104-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43104-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43104-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="43104-110">Permission type</span></span>|<span data-ttu-id="43104-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="43104-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43104-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="43104-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43104-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43104-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="43104-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="43104-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43104-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43104-115">Not supported.</span></span>|
|<span data-ttu-id="43104-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="43104-116">Application</span></span>|<span data-ttu-id="43104-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="43104-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43104-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="43104-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43104-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="43104-119">Optional query parameters</span></span>
<span data-ttu-id="43104-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="43104-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43104-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="43104-121">Request headers</span></span>
|<span data-ttu-id="43104-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="43104-122">Header</span></span>|<span data-ttu-id="43104-123">Wert</span><span class="sxs-lookup"><span data-stu-id="43104-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43104-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="43104-124">Authorization</span></span>|<span data-ttu-id="43104-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="43104-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43104-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="43104-126">Accept</span></span>|<span data-ttu-id="43104-127">application/json</span><span class="sxs-lookup"><span data-stu-id="43104-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43104-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="43104-128">Request body</span></span>
<span data-ttu-id="43104-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="43104-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43104-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="43104-130">Response</span></span>
<span data-ttu-id="43104-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43104-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43104-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="43104-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="43104-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="43104-133">Request</span></span>
<span data-ttu-id="43104-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="43104-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="43104-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="43104-135">Response</span></span>
<span data-ttu-id="43104-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43104-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
    "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




