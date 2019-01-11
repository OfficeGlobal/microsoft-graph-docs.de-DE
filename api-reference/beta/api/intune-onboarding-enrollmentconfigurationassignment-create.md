---
title: enrollmentConfigurationAssignment erstellen
description: Erstellen eines neuen enrollmentConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5541b89a01ea0384506803f605ee33abc6fe32aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873829"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="85114-103">enrollmentConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="85114-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="85114-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="85114-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85114-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="85114-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85114-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="85114-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85114-107">Erstellen eines neuen [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="85114-107">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85114-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="85114-108">Prerequisites</span></span>
<span data-ttu-id="85114-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85114-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85114-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85114-111">Permission type</span></span>|<span data-ttu-id="85114-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85114-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85114-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85114-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85114-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85114-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="85114-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85114-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85114-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85114-116">Not supported.</span></span>|
|<span data-ttu-id="85114-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85114-117">Application</span></span>|<span data-ttu-id="85114-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85114-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85114-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85114-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="85114-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85114-120">Request headers</span></span>
|<span data-ttu-id="85114-121">Header</span><span class="sxs-lookup"><span data-stu-id="85114-121">Header</span></span>|<span data-ttu-id="85114-122">Wert</span><span class="sxs-lookup"><span data-stu-id="85114-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85114-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85114-123">Authorization</span></span>|<span data-ttu-id="85114-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="85114-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85114-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="85114-125">Accept</span></span>|<span data-ttu-id="85114-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85114-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85114-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85114-127">Request body</span></span>
<span data-ttu-id="85114-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentConfigurationAssignment an.</span><span class="sxs-lookup"><span data-stu-id="85114-128">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="85114-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des enrollmentConfigurationAssignment-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="85114-129">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="85114-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="85114-130">Property</span></span>|<span data-ttu-id="85114-131">Typ</span><span class="sxs-lookup"><span data-stu-id="85114-131">Type</span></span>|<span data-ttu-id="85114-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85114-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85114-133">id</span><span class="sxs-lookup"><span data-stu-id="85114-133">id</span></span>|<span data-ttu-id="85114-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="85114-134">String</span></span>|<span data-ttu-id="85114-135">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="85114-135">Not yet documented</span></span>|
|<span data-ttu-id="85114-136">target</span><span class="sxs-lookup"><span data-stu-id="85114-136">target</span></span>|[<span data-ttu-id="85114-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="85114-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="85114-138">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="85114-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="85114-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="85114-139">Response</span></span>
<span data-ttu-id="85114-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="85114-140">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85114-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85114-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="85114-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85114-142">Request</span></span>
<span data-ttu-id="85114-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85114-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="85114-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="85114-144">Response</span></span>
<span data-ttu-id="85114-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85114-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





