---
title: DeviceManagementScriptGroupAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceManagementScriptGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d6988bec87e9470e3c46a7c47c483529ca1e2c86
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869237"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="5a655-103">DeviceManagementScriptGroupAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5a655-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="5a655-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5a655-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a655-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5a655-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a655-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5a655-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a655-107">Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a655-107">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a655-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5a655-108">Prerequisites</span></span>
<span data-ttu-id="5a655-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a655-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a655-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a655-111">Permission type</span></span>|<span data-ttu-id="5a655-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a655-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a655-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a655-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a655-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a655-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5a655-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a655-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a655-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a655-116">Not supported.</span></span>|
|<span data-ttu-id="5a655-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a655-117">Application</span></span>|<span data-ttu-id="5a655-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a655-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a655-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a655-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5a655-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a655-120">Request headers</span></span>
|<span data-ttu-id="5a655-121">Header</span><span class="sxs-lookup"><span data-stu-id="5a655-121">Header</span></span>|<span data-ttu-id="5a655-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5a655-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a655-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a655-123">Authorization</span></span>|<span data-ttu-id="5a655-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5a655-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a655-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5a655-125">Accept</span></span>|<span data-ttu-id="5a655-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a655-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a655-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a655-127">Request body</span></span>
<span data-ttu-id="5a655-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5a655-128">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="5a655-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="5a655-129">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="5a655-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5a655-130">Property</span></span>|<span data-ttu-id="5a655-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5a655-131">Type</span></span>|<span data-ttu-id="5a655-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a655-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a655-133">id</span><span class="sxs-lookup"><span data-stu-id="5a655-133">id</span></span>|<span data-ttu-id="5a655-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5a655-134">String</span></span>|<span data-ttu-id="5a655-135">Taste der Gerät Management Skript Gruppe Zuordnung Entität.</span><span class="sxs-lookup"><span data-stu-id="5a655-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="5a655-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="5a655-136">targetGroupId</span></span>|<span data-ttu-id="5a655-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5a655-137">String</span></span>|<span data-ttu-id="5a655-138">Die Id des Azure Active Directory-Gruppe verwenden wir das Skript Inhaltsadressierung für.</span><span class="sxs-lookup"><span data-stu-id="5a655-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="5a655-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a655-139">Response</span></span>
<span data-ttu-id="5a655-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5a655-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a655-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a655-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a655-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a655-142">Request</span></span>
<span data-ttu-id="5a655-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a655-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 48

{
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="5a655-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a655-144">Response</span></span>
<span data-ttu-id="5a655-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a655-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```





