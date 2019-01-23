---
title: EnableLostMode Aktion
description: Verloren-Modus aktivieren
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 16a6bb61605272cc6412e788ae9a4af7a9e8340d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412618"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="2c5fb-103">EnableLostMode Aktion</span><span class="sxs-lookup"><span data-stu-id="2c5fb-103">enableLostMode action</span></span>

> <span data-ttu-id="2c5fb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2c5fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2c5fb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2c5fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c5fb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2c5fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c5fb-107">Verloren-Modus aktivieren</span><span class="sxs-lookup"><span data-stu-id="2c5fb-107">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c5fb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2c5fb-108">Prerequisites</span></span>
<span data-ttu-id="2c5fb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2c5fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2c5fb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2c5fb-111">Permission type</span></span>|<span data-ttu-id="2c5fb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2c5fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c5fb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2c5fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2c5fb-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2c5fb-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="2c5fb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2c5fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c5fb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c5fb-116">Not supported.</span></span>|
|<span data-ttu-id="2c5fb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2c5fb-117">Application</span></span>|<span data-ttu-id="2c5fb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c5fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c5fb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c5fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="2c5fb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2c5fb-120">Request headers</span></span>
|<span data-ttu-id="2c5fb-121">Header</span><span class="sxs-lookup"><span data-stu-id="2c5fb-121">Header</span></span>|<span data-ttu-id="2c5fb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2c5fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c5fb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="2c5fb-123">Authorization</span></span>|<span data-ttu-id="2c5fb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2c5fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c5fb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2c5fb-125">Accept</span></span>|<span data-ttu-id="2c5fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c5fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c5fb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2c5fb-127">Request body</span></span>
<span data-ttu-id="2c5fb-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="2c5fb-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2c5fb-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="2c5fb-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2c5fb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c5fb-130">Property</span></span>|<span data-ttu-id="2c5fb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2c5fb-131">Type</span></span>|<span data-ttu-id="2c5fb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c5fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c5fb-133">message</span><span class="sxs-lookup"><span data-stu-id="2c5fb-133">message</span></span>|<span data-ttu-id="2c5fb-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2c5fb-134">String</span></span>|<span data-ttu-id="2c5fb-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2c5fb-135">Not yet documented</span></span>|
|<span data-ttu-id="2c5fb-136">PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="2c5fb-136">phoneNumber</span></span>|<span data-ttu-id="2c5fb-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2c5fb-137">String</span></span>|<span data-ttu-id="2c5fb-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2c5fb-138">Not yet documented</span></span>|
|<span data-ttu-id="2c5fb-139">Fußzeile</span><span class="sxs-lookup"><span data-stu-id="2c5fb-139">footer</span></span>|<span data-ttu-id="2c5fb-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2c5fb-140">String</span></span>|<span data-ttu-id="2c5fb-141">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2c5fb-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2c5fb-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c5fb-142">Response</span></span>
<span data-ttu-id="2c5fb-143">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="2c5fb-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2c5fb-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2c5fb-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c5fb-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c5fb-145">Request</span></span>
<span data-ttu-id="2c5fb-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2c5fb-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="2c5fb-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c5fb-147">Response</span></span>
<span data-ttu-id="2c5fb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2c5fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




