---
title: enrollmentConfigurationAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines enrollmentConfigurationAssignment-Objekts.
ms.openlocfilehash: b23b532ae66f3fe4102ad3e03c2ba6e1aff6daa8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064194"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="e9972-103">enrollmentConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e9972-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="e9972-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e9972-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9972-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e9972-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9972-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e9972-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9972-107">Aktualisieren der Eigenschaften eines [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e9972-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9972-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e9972-108">Prerequisites</span></span>
<span data-ttu-id="e9972-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9972-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9972-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e9972-111">Permission type</span></span>|<span data-ttu-id="e9972-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e9972-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9972-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e9972-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9972-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9972-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e9972-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e9972-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9972-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9972-116">Not supported.</span></span>|
|<span data-ttu-id="e9972-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e9972-117">Application</span></span>|<span data-ttu-id="e9972-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e9972-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9972-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9972-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e9972-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e9972-120">Request headers</span></span>
|<span data-ttu-id="e9972-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e9972-121">Header</span></span>|<span data-ttu-id="e9972-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e9972-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9972-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9972-123">Authorization</span></span>|<span data-ttu-id="e9972-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e9972-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9972-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9972-125">Accept</span></span>|<span data-ttu-id="e9972-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9972-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9972-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e9972-127">Request body</span></span>
<span data-ttu-id="e9972-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="e9972-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="e9972-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e9972-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="e9972-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e9972-130">Property</span></span>|<span data-ttu-id="e9972-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e9972-131">Type</span></span>|<span data-ttu-id="e9972-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9972-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9972-133">id</span><span class="sxs-lookup"><span data-stu-id="e9972-133">id</span></span>|<span data-ttu-id="e9972-134">String</span><span class="sxs-lookup"><span data-stu-id="e9972-134">String</span></span>|<span data-ttu-id="e9972-135">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e9972-135">Not yet documented</span></span>|
|<span data-ttu-id="e9972-136">target</span><span class="sxs-lookup"><span data-stu-id="e9972-136">target</span></span>|[<span data-ttu-id="e9972-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e9972-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e9972-138">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="e9972-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e9972-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9972-139">Response</span></span>
<span data-ttu-id="e9972-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e9972-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9972-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e9972-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9972-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e9972-142">Request</span></span>
<span data-ttu-id="e9972-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e9972-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e9972-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e9972-144">Response</span></span>
<span data-ttu-id="e9972-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e9972-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





