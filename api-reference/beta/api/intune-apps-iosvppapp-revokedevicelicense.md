---
title: RevokeDeviceLicense Aktion
description: REVOKE zugewiesen iOS VPP Gerätenlizenz für app zu reparieren.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b58fe7440b1b77e5dc651a4a7c802dae8e5139c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410406"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="b921c-103">RevokeDeviceLicense Aktion</span><span class="sxs-lookup"><span data-stu-id="b921c-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="b921c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b921c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b921c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b921c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b921c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b921c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b921c-107">REVOKE zugewiesen iOS VPP Gerätenlizenz für app zu reparieren.</span><span class="sxs-lookup"><span data-stu-id="b921c-107">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b921c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b921c-108">Prerequisites</span></span>
<span data-ttu-id="b921c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b921c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b921c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b921c-111">Permission type</span></span>|<span data-ttu-id="b921c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b921c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b921c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b921c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b921c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b921c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b921c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b921c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b921c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b921c-116">Not supported.</span></span>|
|<span data-ttu-id="b921c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b921c-117">Application</span></span>|<span data-ttu-id="b921c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b921c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b921c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b921c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="b921c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b921c-120">Request headers</span></span>
|<span data-ttu-id="b921c-121">Header</span><span class="sxs-lookup"><span data-stu-id="b921c-121">Header</span></span>|<span data-ttu-id="b921c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b921c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b921c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b921c-123">Authorization</span></span>|<span data-ttu-id="b921c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b921c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b921c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b921c-125">Accept</span></span>|<span data-ttu-id="b921c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b921c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b921c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b921c-127">Request body</span></span>
<span data-ttu-id="b921c-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="b921c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b921c-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b921c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b921c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b921c-130">Property</span></span>|<span data-ttu-id="b921c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b921c-131">Type</span></span>|<span data-ttu-id="b921c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b921c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b921c-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="b921c-133">managedDeviceId</span></span>|<span data-ttu-id="b921c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b921c-134">String</span></span>|<span data-ttu-id="b921c-135">Geräte-ID für die zugewiesenen app-Lizenz ist gesperrt werden</span><span class="sxs-lookup"><span data-stu-id="b921c-135">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="b921c-136">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="b921c-136">notifyManagedDevices</span></span>|<span data-ttu-id="b921c-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b921c-137">Boolean</span></span>|<span data-ttu-id="b921c-138">Boolescher Wert, der angibt, ob Revoke-Benachrichtigung an Gerät gesendet werden sollen</span><span class="sxs-lookup"><span data-stu-id="b921c-138">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="b921c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="b921c-139">Response</span></span>
<span data-ttu-id="b921c-140">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="b921c-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b921c-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b921c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b921c-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b921c-142">Request</span></span>
<span data-ttu-id="b921c-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b921c-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="b921c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="b921c-144">Response</span></span>
<span data-ttu-id="b921c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b921c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




