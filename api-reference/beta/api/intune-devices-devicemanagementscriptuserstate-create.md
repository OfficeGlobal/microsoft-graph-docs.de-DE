---
title: Erstellen von deviceManagementScriptUserState
description: Erstellen eines neuen DeviceManagementScriptUserState-Objekts.
ms.openlocfilehash: 4d6aba6ae11f2d6250d20524a1e6f47e55bbda2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062018"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="49732-103">Erstellen von deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="49732-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="49732-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="49732-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49732-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49732-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49732-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="49732-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49732-107">Erstellen eines neuen [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="49732-107">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49732-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="49732-108">Prerequisites</span></span>
<span data-ttu-id="49732-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49732-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49732-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49732-111">Permission type</span></span>|<span data-ttu-id="49732-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49732-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49732-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49732-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49732-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49732-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="49732-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49732-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49732-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49732-116">Not supported.</span></span>|
|<span data-ttu-id="49732-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49732-117">Application</span></span>|<span data-ttu-id="49732-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49732-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49732-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49732-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="49732-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49732-120">Request headers</span></span>
|<span data-ttu-id="49732-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="49732-121">Header</span></span>|<span data-ttu-id="49732-122">Wert</span><span class="sxs-lookup"><span data-stu-id="49732-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49732-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49732-123">Authorization</span></span>|<span data-ttu-id="49732-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="49732-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49732-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49732-125">Accept</span></span>|<span data-ttu-id="49732-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49732-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49732-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49732-127">Request body</span></span>
<span data-ttu-id="49732-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceManagementScriptUserState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="49732-128">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="49732-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceManagementScriptUserState erstellen.</span><span class="sxs-lookup"><span data-stu-id="49732-129">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="49732-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49732-130">Property</span></span>|<span data-ttu-id="49732-131">Typ</span><span class="sxs-lookup"><span data-stu-id="49732-131">Type</span></span>|<span data-ttu-id="49732-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49732-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49732-133">id</span><span class="sxs-lookup"><span data-stu-id="49732-133">id</span></span>|<span data-ttu-id="49732-134">String</span><span class="sxs-lookup"><span data-stu-id="49732-134">String</span></span>|<span data-ttu-id="49732-135">Das Gerät Management Skript Zustand Benutzerentität-Taste.</span><span class="sxs-lookup"><span data-stu-id="49732-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="49732-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="49732-136">successDeviceCount</span></span>|<span data-ttu-id="49732-137">Int32</span><span class="sxs-lookup"><span data-stu-id="49732-137">Int32</span></span>|<span data-ttu-id="49732-138">Anzahl der Erfolg Geräte für bestimmte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="49732-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="49732-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="49732-139">errorDeviceCount</span></span>|<span data-ttu-id="49732-140">Int32</span><span class="sxs-lookup"><span data-stu-id="49732-140">Int32</span></span>|<span data-ttu-id="49732-141">Anzahl der Fehler Geräte für bestimmte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="49732-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="49732-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="49732-142">userPrincipalName</span></span>|<span data-ttu-id="49732-143">String</span><span class="sxs-lookup"><span data-stu-id="49732-143">String</span></span>|<span data-ttu-id="49732-144">Prinzip-Benutzernamen eines bestimmten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="49732-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="49732-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="49732-145">Response</span></span>
<span data-ttu-id="49732-146">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="49732-146">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49732-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49732-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="49732-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49732-148">Request</span></span>
<span data-ttu-id="49732-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49732-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="49732-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="49732-150">Response</span></span>
<span data-ttu-id="49732-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49732-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





