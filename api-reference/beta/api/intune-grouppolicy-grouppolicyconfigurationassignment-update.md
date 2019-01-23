---
title: GroupPolicyConfigurationAssignment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyConfigurationAssignment-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08ff87b70b833dc1f8423a8465b5b880660fd462
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431562"
---
# <a name="update-grouppolicyconfigurationassignment"></a><span data-ttu-id="d9597-103">GroupPolicyConfigurationAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d9597-103">Update groupPolicyConfigurationAssignment</span></span>

> <span data-ttu-id="d9597-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d9597-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d9597-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9597-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9597-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d9597-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9597-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d9597-107">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9597-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d9597-108">Prerequisites</span></span>
<span data-ttu-id="d9597-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d9597-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d9597-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9597-111">Permission type</span></span>|<span data-ttu-id="d9597-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9597-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9597-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9597-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9597-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9597-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d9597-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9597-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9597-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9597-116">Not supported.</span></span>|
|<span data-ttu-id="d9597-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9597-117">Application</span></span>|<span data-ttu-id="d9597-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9597-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9597-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9597-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d9597-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d9597-120">Request headers</span></span>
|<span data-ttu-id="d9597-121">Header</span><span class="sxs-lookup"><span data-stu-id="d9597-121">Header</span></span>|<span data-ttu-id="d9597-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d9597-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9597-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d9597-123">Authorization</span></span>|<span data-ttu-id="d9597-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d9597-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9597-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d9597-125">Accept</span></span>|<span data-ttu-id="d9597-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9597-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9597-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d9597-127">Request body</span></span>
<span data-ttu-id="d9597-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="d9597-128">In the request body, supply a JSON representation for the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>

<span data-ttu-id="d9597-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="d9597-129">The following table shows the properties that are required when you create the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>

|<span data-ttu-id="d9597-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d9597-130">Property</span></span>|<span data-ttu-id="d9597-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d9597-131">Type</span></span>|<span data-ttu-id="d9597-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9597-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9597-133">id</span><span class="sxs-lookup"><span data-stu-id="d9597-133">id</span></span>|<span data-ttu-id="d9597-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d9597-134">String</span></span>|<span data-ttu-id="d9597-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d9597-135">Key of the entity.</span></span>|
|<span data-ttu-id="d9597-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9597-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d9597-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9597-137">DateTimeOffset</span></span>|<span data-ttu-id="d9597-138">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="d9597-138">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="d9597-139">target</span><span class="sxs-lookup"><span data-stu-id="d9597-139">target</span></span>|[<span data-ttu-id="d9597-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d9597-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d9597-141">Der Typ der Gruppen angegeben, die Gruppenrichtlinienkonfiguration vorgesehen sind.</span><span class="sxs-lookup"><span data-stu-id="d9597-141">The type of groups targeted the group policy configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="d9597-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9597-142">Response</span></span>
<span data-ttu-id="d9597-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d9597-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9597-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9597-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9597-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9597-145">Request</span></span>
<span data-ttu-id="d9597-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d9597-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d9597-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9597-147">Response</span></span>
<span data-ttu-id="d9597-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d9597-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




