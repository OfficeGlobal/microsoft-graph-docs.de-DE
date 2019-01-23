---
title: AssignUserToDevice Aktion
description: Autopilot Geräte Benutzer zugewiesen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2003f8517a7863a485f1929cdee8c750b04d6d76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412282"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="e1423-103">AssignUserToDevice Aktion</span><span class="sxs-lookup"><span data-stu-id="e1423-103">assignUserToDevice action</span></span>

> <span data-ttu-id="e1423-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e1423-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1423-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e1423-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1423-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1423-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1423-107">Autopilot Geräte Benutzer zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="e1423-107">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1423-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e1423-108">Prerequisites</span></span>
<span data-ttu-id="e1423-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1423-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e1423-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1423-111">Permission type</span></span>|<span data-ttu-id="e1423-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1423-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1423-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1423-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1423-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1423-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e1423-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1423-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1423-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1423-116">Not supported.</span></span>|
|<span data-ttu-id="e1423-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1423-117">Application</span></span>|<span data-ttu-id="e1423-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1423-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1423-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1423-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="e1423-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1423-120">Request headers</span></span>
|<span data-ttu-id="e1423-121">Header</span><span class="sxs-lookup"><span data-stu-id="e1423-121">Header</span></span>|<span data-ttu-id="e1423-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e1423-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1423-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e1423-123">Authorization</span></span>|<span data-ttu-id="e1423-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e1423-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1423-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e1423-125">Accept</span></span>|<span data-ttu-id="e1423-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1423-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1423-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e1423-127">Request body</span></span>
<span data-ttu-id="e1423-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="e1423-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e1423-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e1423-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e1423-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e1423-130">Property</span></span>|<span data-ttu-id="e1423-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e1423-131">Type</span></span>|<span data-ttu-id="e1423-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1423-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1423-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1423-133">userPrincipalName</span></span>|<span data-ttu-id="e1423-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1423-134">String</span></span>|<span data-ttu-id="e1423-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e1423-135">Not yet documented</span></span>|
|<span data-ttu-id="e1423-136">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="e1423-136">addressableUserName</span></span>|<span data-ttu-id="e1423-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e1423-137">String</span></span>|<span data-ttu-id="e1423-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e1423-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e1423-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1423-139">Response</span></span>
<span data-ttu-id="e1423-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="e1423-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e1423-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1423-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1423-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1423-142">Request</span></span>
<span data-ttu-id="e1423-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1423-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="e1423-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1423-144">Response</span></span>
<span data-ttu-id="e1423-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1423-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




