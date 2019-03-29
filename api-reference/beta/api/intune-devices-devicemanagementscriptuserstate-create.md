---
title: DeviceManagementScriptUserState erstellen
description: Erstellen eines neuen deviceManagementScriptUserState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aff7161ebd220924bd8c8c05bff4cd138b3ea59e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967657"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="8f075-103">DeviceManagementScriptUserState erstellen</span><span class="sxs-lookup"><span data-stu-id="8f075-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="8f075-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8f075-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f075-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8f075-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f075-106">Erstellen eines neuen [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f075-106">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f075-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8f075-107">Prerequisites</span></span>
<span data-ttu-id="8f075-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f075-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f075-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8f075-110">Permission type</span></span>|<span data-ttu-id="8f075-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8f075-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f075-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8f075-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f075-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f075-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8f075-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8f075-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f075-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f075-115">Not supported.</span></span>|
|<span data-ttu-id="8f075-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8f075-116">Application</span></span>|<span data-ttu-id="8f075-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f075-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f075-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f075-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="8f075-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8f075-119">Request headers</span></span>
|<span data-ttu-id="8f075-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8f075-120">Header</span></span>|<span data-ttu-id="8f075-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8f075-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f075-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f075-122">Authorization</span></span>|<span data-ttu-id="8f075-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8f075-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f075-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8f075-124">Accept</span></span>|<span data-ttu-id="8f075-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f075-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f075-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8f075-126">Request body</span></span>
<span data-ttu-id="8f075-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceManagementScriptUserState-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="8f075-127">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="8f075-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceManagementScriptUserState erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8f075-128">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="8f075-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f075-129">Property</span></span>|<span data-ttu-id="8f075-130">Typ</span><span class="sxs-lookup"><span data-stu-id="8f075-130">Type</span></span>|<span data-ttu-id="8f075-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f075-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f075-132">id</span><span class="sxs-lookup"><span data-stu-id="8f075-132">id</span></span>|<span data-ttu-id="8f075-133">String</span><span class="sxs-lookup"><span data-stu-id="8f075-133">String</span></span>|<span data-ttu-id="8f075-134">Schlüssel der Benutzerstatus Entität des Device Management-Skripts.</span><span class="sxs-lookup"><span data-stu-id="8f075-134">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="8f075-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8f075-135">successDeviceCount</span></span>|<span data-ttu-id="8f075-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8f075-136">Int32</span></span>|<span data-ttu-id="8f075-137">Anzahl der erfolgreichen Geräte für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="8f075-137">Success device count for specific user.</span></span>|
|<span data-ttu-id="8f075-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8f075-138">errorDeviceCount</span></span>|<span data-ttu-id="8f075-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8f075-139">Int32</span></span>|<span data-ttu-id="8f075-140">Fehlergeräte Anzahl für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="8f075-140">Error device count for specific user.</span></span>|
|<span data-ttu-id="8f075-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8f075-141">userPrincipalName</span></span>|<span data-ttu-id="8f075-142">String</span><span class="sxs-lookup"><span data-stu-id="8f075-142">String</span></span>|<span data-ttu-id="8f075-143">Benutzerprinzipalname des jeweiligen Benutzers.</span><span class="sxs-lookup"><span data-stu-id="8f075-143">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="8f075-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f075-144">Response</span></span>
<span data-ttu-id="8f075-145">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8f075-145">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f075-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8f075-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f075-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f075-147">Request</span></span>
<span data-ttu-id="8f075-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8f075-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="8f075-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f075-149">Response</span></span>
<span data-ttu-id="8f075-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f075-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```




