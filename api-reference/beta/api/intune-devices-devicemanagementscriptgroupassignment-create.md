---
title: Erstellen von deviceManagementScriptGroupAssignment
description: Erstellen eines neuen DeviceManagementScriptGroupAssignment-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a26c777cbdbf6ea6bb8f8ab6b2435934d90fc915
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411414"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="84fce-103">Erstellen von deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="84fce-103">Create deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="84fce-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="84fce-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84fce-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84fce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84fce-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="84fce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84fce-107">Erstellen eines neuen [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="84fce-107">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84fce-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84fce-108">Prerequisites</span></span>
<span data-ttu-id="84fce-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="84fce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="84fce-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84fce-111">Permission type</span></span>|<span data-ttu-id="84fce-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84fce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84fce-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84fce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84fce-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84fce-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="84fce-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84fce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84fce-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84fce-116">Not supported.</span></span>|
|<span data-ttu-id="84fce-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84fce-117">Application</span></span>|<span data-ttu-id="84fce-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84fce-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84fce-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84fce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="84fce-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84fce-120">Request headers</span></span>
|<span data-ttu-id="84fce-121">Header</span><span class="sxs-lookup"><span data-stu-id="84fce-121">Header</span></span>|<span data-ttu-id="84fce-122">Wert</span><span class="sxs-lookup"><span data-stu-id="84fce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84fce-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="84fce-123">Authorization</span></span>|<span data-ttu-id="84fce-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84fce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84fce-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="84fce-125">Accept</span></span>|<span data-ttu-id="84fce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84fce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84fce-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84fce-127">Request body</span></span>
<span data-ttu-id="84fce-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceManagementScriptGroupAssignment eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="84fce-128">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="84fce-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceManagementScriptGroupAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="84fce-129">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="84fce-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="84fce-130">Property</span></span>|<span data-ttu-id="84fce-131">Typ</span><span class="sxs-lookup"><span data-stu-id="84fce-131">Type</span></span>|<span data-ttu-id="84fce-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84fce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84fce-133">id</span><span class="sxs-lookup"><span data-stu-id="84fce-133">id</span></span>|<span data-ttu-id="84fce-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84fce-134">String</span></span>|<span data-ttu-id="84fce-135">Taste der Gerät Management Skript Gruppe Zuordnung Entität.</span><span class="sxs-lookup"><span data-stu-id="84fce-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="84fce-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="84fce-136">targetGroupId</span></span>|<span data-ttu-id="84fce-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84fce-137">String</span></span>|<span data-ttu-id="84fce-138">Die Id des Azure Active Directory-Gruppe verwenden wir das Skript Inhaltsadressierung für.</span><span class="sxs-lookup"><span data-stu-id="84fce-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="84fce-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="84fce-139">Response</span></span>
<span data-ttu-id="84fce-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="84fce-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84fce-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84fce-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="84fce-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84fce-142">Request</span></span>
<span data-ttu-id="84fce-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84fce-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="84fce-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="84fce-144">Response</span></span>
<span data-ttu-id="84fce-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84fce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```




