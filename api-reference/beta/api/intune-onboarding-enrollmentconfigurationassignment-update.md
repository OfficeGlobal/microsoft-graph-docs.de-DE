---
title: enrollmentConfigurationAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines enrollmentConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 01d17a5f4cb1f5d61e05e1e9d0b14a4708dce8b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963185"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="8851f-103">enrollmentConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8851f-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="8851f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8851f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8851f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8851f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8851f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8851f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8851f-107">Aktualisieren der Eigenschaften eines [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8851f-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8851f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8851f-108">Prerequisites</span></span>
<span data-ttu-id="8851f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8851f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8851f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8851f-111">Permission type</span></span>|<span data-ttu-id="8851f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8851f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8851f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8851f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8851f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8851f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8851f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8851f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8851f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8851f-116">Not supported.</span></span>|
|<span data-ttu-id="8851f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8851f-117">Application</span></span>|<span data-ttu-id="8851f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8851f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8851f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8851f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8851f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8851f-120">Request headers</span></span>
|<span data-ttu-id="8851f-121">Header</span><span class="sxs-lookup"><span data-stu-id="8851f-121">Header</span></span>|<span data-ttu-id="8851f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8851f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8851f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8851f-123">Authorization</span></span>|<span data-ttu-id="8851f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8851f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8851f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8851f-125">Accept</span></span>|<span data-ttu-id="8851f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8851f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8851f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8851f-127">Request body</span></span>
<span data-ttu-id="8851f-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="8851f-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="8851f-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8851f-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="8851f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8851f-130">Property</span></span>|<span data-ttu-id="8851f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8851f-131">Type</span></span>|<span data-ttu-id="8851f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8851f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8851f-133">id</span><span class="sxs-lookup"><span data-stu-id="8851f-133">id</span></span>|<span data-ttu-id="8851f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8851f-134">String</span></span>|<span data-ttu-id="8851f-135">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8851f-135">Not yet documented</span></span>|
|<span data-ttu-id="8851f-136">target</span><span class="sxs-lookup"><span data-stu-id="8851f-136">target</span></span>|[<span data-ttu-id="8851f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8851f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8851f-138">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="8851f-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8851f-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="8851f-139">Response</span></span>
<span data-ttu-id="8851f-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8851f-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8851f-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8851f-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="8851f-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8851f-142">Request</span></span>
<span data-ttu-id="8851f-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8851f-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="8851f-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="8851f-144">Response</span></span>
<span data-ttu-id="8851f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8851f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





