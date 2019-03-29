---
title: Auflisten von „managedDeviceMobileAppConfigurationAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedDeviceMobileAppConfigurationAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: edaf791c95839a43a37a52a30dfe97e8550b2fb2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983190"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="9604f-103">Auflisten von „managedDeviceMobileAppConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="9604f-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="9604f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9604f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9604f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9604f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9604f-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="9604f-106">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9604f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9604f-107">Prerequisites</span></span>
<span data-ttu-id="9604f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9604f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9604f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9604f-110">Permission type</span></span>|<span data-ttu-id="9604f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9604f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9604f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9604f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9604f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9604f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9604f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9604f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9604f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9604f-115">Not supported.</span></span>|
|<span data-ttu-id="9604f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9604f-116">Application</span></span>|<span data-ttu-id="9604f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9604f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9604f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9604f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9604f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9604f-119">Request headers</span></span>
|<span data-ttu-id="9604f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9604f-120">Header</span></span>|<span data-ttu-id="9604f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9604f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9604f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9604f-122">Authorization</span></span>|<span data-ttu-id="9604f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9604f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9604f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9604f-124">Accept</span></span>|<span data-ttu-id="9604f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9604f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9604f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9604f-126">Request body</span></span>
<span data-ttu-id="9604f-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9604f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9604f-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9604f-128">Response</span></span>
<span data-ttu-id="9604f-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9604f-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9604f-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9604f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9604f-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9604f-131">Request</span></span>
<span data-ttu-id="9604f-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9604f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="9604f-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9604f-133">Response</span></span>
<span data-ttu-id="9604f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9604f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




