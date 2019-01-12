---
title: Erstellen von deviceManagementScriptUserState
description: Erstellen eines neuen DeviceManagementScriptUserState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 93aca9ce1689f3159594963af062616a2b1de7eb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940799"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="b92bc-103">Erstellen von deviceManagementScriptUserState</span><span class="sxs-lookup"><span data-stu-id="b92bc-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="b92bc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b92bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b92bc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b92bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b92bc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b92bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b92bc-107">Erstellen eines neuen [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b92bc-107">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b92bc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b92bc-108">Prerequisites</span></span>
<span data-ttu-id="b92bc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b92bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b92bc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b92bc-111">Permission type</span></span>|<span data-ttu-id="b92bc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b92bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b92bc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b92bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b92bc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b92bc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b92bc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b92bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b92bc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b92bc-116">Not supported.</span></span>|
|<span data-ttu-id="b92bc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b92bc-117">Application</span></span>|<span data-ttu-id="b92bc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b92bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b92bc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b92bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="b92bc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b92bc-120">Request headers</span></span>
|<span data-ttu-id="b92bc-121">Header</span><span class="sxs-lookup"><span data-stu-id="b92bc-121">Header</span></span>|<span data-ttu-id="b92bc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b92bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b92bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b92bc-123">Authorization</span></span>|<span data-ttu-id="b92bc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b92bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b92bc-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b92bc-125">Accept</span></span>|<span data-ttu-id="b92bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b92bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b92bc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b92bc-127">Request body</span></span>
<span data-ttu-id="b92bc-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceManagementScriptUserState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="b92bc-128">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="b92bc-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceManagementScriptUserState erstellen.</span><span class="sxs-lookup"><span data-stu-id="b92bc-129">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="b92bc-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b92bc-130">Property</span></span>|<span data-ttu-id="b92bc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b92bc-131">Type</span></span>|<span data-ttu-id="b92bc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b92bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b92bc-133">id</span><span class="sxs-lookup"><span data-stu-id="b92bc-133">id</span></span>|<span data-ttu-id="b92bc-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b92bc-134">String</span></span>|<span data-ttu-id="b92bc-135">Das Gerät Management Skript Zustand Benutzerentität-Taste.</span><span class="sxs-lookup"><span data-stu-id="b92bc-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="b92bc-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b92bc-136">successDeviceCount</span></span>|<span data-ttu-id="b92bc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b92bc-137">Int32</span></span>|<span data-ttu-id="b92bc-138">Anzahl der Erfolg Geräte für bestimmte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="b92bc-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="b92bc-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b92bc-139">errorDeviceCount</span></span>|<span data-ttu-id="b92bc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b92bc-140">Int32</span></span>|<span data-ttu-id="b92bc-141">Anzahl der Fehler Geräte für bestimmte Benutzer.</span><span class="sxs-lookup"><span data-stu-id="b92bc-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="b92bc-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b92bc-142">userPrincipalName</span></span>|<span data-ttu-id="b92bc-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b92bc-143">String</span></span>|<span data-ttu-id="b92bc-144">Prinzip-Benutzernamen eines bestimmten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="b92bc-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="b92bc-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="b92bc-145">Response</span></span>
<span data-ttu-id="b92bc-146">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b92bc-146">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b92bc-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b92bc-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="b92bc-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b92bc-148">Request</span></span>
<span data-ttu-id="b92bc-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b92bc-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b92bc-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="b92bc-150">Response</span></span>
<span data-ttu-id="b92bc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b92bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





