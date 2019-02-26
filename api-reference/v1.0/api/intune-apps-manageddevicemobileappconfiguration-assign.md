---
title: Aktion zuweisen
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: feb9e93247d26fedd21454d696f4566eeef4e8d0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255465"
---
# <a name="assign-action"></a><span data-ttu-id="4eb4b-103">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="4eb4b-103">assign action</span></span>

> <span data-ttu-id="4eb4b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4eb4b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eb4b-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4eb4b-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4eb4b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4eb4b-106">Prerequisites</span></span>
<span data-ttu-id="4eb4b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4eb4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4eb4b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4eb4b-109">Permission type</span></span>|<span data-ttu-id="4eb4b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4eb4b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eb4b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4eb4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4eb4b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eb4b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4eb4b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4eb4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eb4b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4eb4b-114">Not supported.</span></span>|
|<span data-ttu-id="4eb4b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4eb4b-115">Application</span></span>|<span data-ttu-id="4eb4b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4eb4b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eb4b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4eb4b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4eb4b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4eb4b-118">Request headers</span></span>
|<span data-ttu-id="4eb4b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4eb4b-119">Header</span></span>|<span data-ttu-id="4eb4b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4eb4b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eb4b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eb4b-121">Authorization</span></span>|<span data-ttu-id="4eb4b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4eb4b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eb4b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4eb4b-123">Accept</span></span>|<span data-ttu-id="4eb4b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4eb4b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eb4b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4eb4b-125">Request body</span></span>
<span data-ttu-id="4eb4b-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="4eb4b-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4eb4b-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4eb4b-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4eb4b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4eb4b-128">Property</span></span>|<span data-ttu-id="4eb4b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4eb4b-129">Type</span></span>|<span data-ttu-id="4eb4b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4eb4b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eb4b-131">assignments</span><span class="sxs-lookup"><span data-stu-id="4eb4b-131">assignments</span></span>|<span data-ttu-id="4eb4b-132">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4eb4b-132">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4eb4b-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="4eb4b-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4eb4b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4eb4b-134">Response</span></span>
<span data-ttu-id="4eb4b-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="4eb4b-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4eb4b-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4eb4b-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="4eb4b-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4eb4b-137">Request</span></span>
<span data-ttu-id="4eb4b-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4eb4b-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assign

Content-type: application/json
Content-length: 293

{
  "assignments": [
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

### <a name="response"></a><span data-ttu-id="4eb4b-139">Reaktion</span><span class="sxs-lookup"><span data-stu-id="4eb4b-139">Response</span></span>
<span data-ttu-id="4eb4b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4eb4b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



