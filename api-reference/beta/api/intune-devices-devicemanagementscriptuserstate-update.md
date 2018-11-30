---
title: DeviceManagementScriptUserState aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceManagementScriptUserState-Objekts.
ms.openlocfilehash: f6428579bc19a005a1bf10b769916ac302304485
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064861"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="5b14e-103">DeviceManagementScriptUserState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5b14e-103">Update deviceManagementScriptUserState</span></span>

> <span data-ttu-id="5b14e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5b14e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b14e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b14e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b14e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5b14e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b14e-107">Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5b14e-107">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b14e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5b14e-108">Prerequisites</span></span>
<span data-ttu-id="5b14e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b14e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b14e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b14e-111">Permission type</span></span>|<span data-ttu-id="5b14e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b14e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b14e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b14e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b14e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b14e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5b14e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b14e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b14e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b14e-116">Not supported.</span></span>|
|<span data-ttu-id="5b14e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b14e-117">Application</span></span>|<span data-ttu-id="5b14e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b14e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b14e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b14e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="5b14e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b14e-120">Request headers</span></span>
|<span data-ttu-id="5b14e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5b14e-121">Header</span></span>|<span data-ttu-id="5b14e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5b14e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b14e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b14e-123">Authorization</span></span>|<span data-ttu-id="5b14e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5b14e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b14e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b14e-125">Accept</span></span>|<span data-ttu-id="5b14e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b14e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b14e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b14e-127">Request body</span></span>
<span data-ttu-id="5b14e-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5b14e-128">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="5b14e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="5b14e-129">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="5b14e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b14e-130">Property</span></span>|<span data-ttu-id="5b14e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5b14e-131">Type</span></span>|<span data-ttu-id="5b14e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b14e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b14e-133">id</span><span class="sxs-lookup"><span data-stu-id="5b14e-133">id</span></span>|<span data-ttu-id="5b14e-134">String</span><span class="sxs-lookup"><span data-stu-id="5b14e-134">String</span></span>|<span data-ttu-id="5b14e-135">Das Gerät Management Skript Zustand Benutzerentität-Taste.</span><span class="sxs-lookup"><span data-stu-id="5b14e-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="5b14e-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5b14e-136">successDeviceCount</span></span>|<span data-ttu-id="5b14e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5b14e-137">Int32</span></span>|<span data-ttu-id="5b14e-138">Anzahl der Erfolg Geräte für bestimmte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="5b14e-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="5b14e-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5b14e-139">errorDeviceCount</span></span>|<span data-ttu-id="5b14e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5b14e-140">Int32</span></span>|<span data-ttu-id="5b14e-141">Anzahl der Fehler Geräte für bestimmte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="5b14e-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="5b14e-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5b14e-142">userPrincipalName</span></span>|<span data-ttu-id="5b14e-143">String</span><span class="sxs-lookup"><span data-stu-id="5b14e-143">String</span></span>|<span data-ttu-id="5b14e-144">Prinzip-Benutzernamen eines bestimmten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="5b14e-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="5b14e-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b14e-145">Response</span></span>
<span data-ttu-id="5b14e-146">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5b14e-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b14e-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b14e-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b14e-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b14e-148">Request</span></span>
<span data-ttu-id="5b14e-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b14e-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
Content-type: application/json
Content-length: 110

{
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="5b14e-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b14e-150">Response</span></span>
<span data-ttu-id="5b14e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b14e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





