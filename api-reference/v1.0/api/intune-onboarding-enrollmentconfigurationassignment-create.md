---
title: enrollmentConfigurationAssignment erstellen
description: Erstellen eines neuen enrollmentConfigurationAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d378b9f4663a6f3770d00a0f7971d1bc4c3b01b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844087"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="da2aa-103">enrollmentConfigurationAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="da2aa-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="da2aa-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="da2aa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da2aa-105">Erstellen eines neuen [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="da2aa-105">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da2aa-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="da2aa-106">Prerequisites</span></span>
<span data-ttu-id="da2aa-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da2aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da2aa-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da2aa-109">Permission type</span></span>|<span data-ttu-id="da2aa-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da2aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da2aa-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da2aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="da2aa-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2aa-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="da2aa-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da2aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da2aa-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da2aa-114">Not supported.</span></span>|
|<span data-ttu-id="da2aa-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da2aa-115">Application</span></span>|<span data-ttu-id="da2aa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da2aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da2aa-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da2aa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="da2aa-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da2aa-118">Request headers</span></span>
|<span data-ttu-id="da2aa-119">Header</span><span class="sxs-lookup"><span data-stu-id="da2aa-119">Header</span></span>|<span data-ttu-id="da2aa-120">Wert</span><span class="sxs-lookup"><span data-stu-id="da2aa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da2aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="da2aa-121">Authorization</span></span>|<span data-ttu-id="da2aa-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="da2aa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da2aa-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="da2aa-123">Accept</span></span>|<span data-ttu-id="da2aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="da2aa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da2aa-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da2aa-125">Request body</span></span>
<span data-ttu-id="da2aa-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs enrollmentConfigurationAssignment an.</span><span class="sxs-lookup"><span data-stu-id="da2aa-126">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="da2aa-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des enrollmentConfigurationAssignment-Objekts erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="da2aa-127">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="da2aa-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da2aa-128">Property</span></span>|<span data-ttu-id="da2aa-129">Typ</span><span class="sxs-lookup"><span data-stu-id="da2aa-129">Type</span></span>|<span data-ttu-id="da2aa-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da2aa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da2aa-131">id</span><span class="sxs-lookup"><span data-stu-id="da2aa-131">id</span></span>|<span data-ttu-id="da2aa-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da2aa-132">String</span></span>|<span data-ttu-id="da2aa-133">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="da2aa-133">Not yet documented</span></span>|
|<span data-ttu-id="da2aa-134">target</span><span class="sxs-lookup"><span data-stu-id="da2aa-134">target</span></span>|[<span data-ttu-id="da2aa-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="da2aa-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="da2aa-136">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="da2aa-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="da2aa-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="da2aa-137">Response</span></span>
<span data-ttu-id="da2aa-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="da2aa-138">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da2aa-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da2aa-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="da2aa-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da2aa-140">Request</span></span>
<span data-ttu-id="da2aa-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da2aa-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="da2aa-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="da2aa-142">Response</span></span>
<span data-ttu-id="da2aa-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da2aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



