---
title: deviceEnrollmentLimitConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentLimitConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 4a3f9230b29fbe78e4a3771812bdfa435b1e2c5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310423"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="c3e0e-103">deviceEnrollmentLimitConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="c3e0e-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="c3e0e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c3e0e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3e0e-105">Erstellen eines neuen [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c3e0e-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3e0e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c3e0e-106">Prerequisites</span></span>
<span data-ttu-id="c3e0e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3e0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3e0e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c3e0e-109">Permission type</span></span>|<span data-ttu-id="c3e0e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c3e0e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3e0e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c3e0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3e0e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3e0e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c3e0e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c3e0e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3e0e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3e0e-114">Not supported.</span></span>|
|<span data-ttu-id="c3e0e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c3e0e-115">Application</span></span>|<span data-ttu-id="c3e0e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3e0e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3e0e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3e0e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c3e0e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c3e0e-118">Request headers</span></span>
|<span data-ttu-id="c3e0e-119">Header</span><span class="sxs-lookup"><span data-stu-id="c3e0e-119">Header</span></span>|<span data-ttu-id="c3e0e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c3e0e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3e0e-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c3e0e-121">Authorization</span></span>|<span data-ttu-id="c3e0e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c3e0e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3e0e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c3e0e-123">Accept</span></span>|<span data-ttu-id="c3e0e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c3e0e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3e0e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c3e0e-125">Request body</span></span>
<span data-ttu-id="c3e0e-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentLimitConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c3e0e-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="c3e0e-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentLimitConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c3e0e-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="c3e0e-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3e0e-128">Property</span></span>|<span data-ttu-id="c3e0e-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c3e0e-129">Type</span></span>|<span data-ttu-id="c3e0e-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3e0e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3e0e-131">id</span><span class="sxs-lookup"><span data-stu-id="c3e0e-131">id</span></span>|<span data-ttu-id="c3e0e-132">String</span><span class="sxs-lookup"><span data-stu-id="c3e0e-132">String</span></span>|<span data-ttu-id="c3e0e-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3e0e-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c3e0e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c3e0e-134">displayName</span></span>|<span data-ttu-id="c3e0e-135">String</span><span class="sxs-lookup"><span data-stu-id="c3e0e-135">String</span></span>|<span data-ttu-id="c3e0e-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3e0e-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c3e0e-137">description</span><span class="sxs-lookup"><span data-stu-id="c3e0e-137">description</span></span>|<span data-ttu-id="c3e0e-138">String</span><span class="sxs-lookup"><span data-stu-id="c3e0e-138">String</span></span>|<span data-ttu-id="c3e0e-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3e0e-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c3e0e-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="c3e0e-140">priority</span></span>|<span data-ttu-id="c3e0e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c3e0e-141">Int32</span></span>|<span data-ttu-id="c3e0e-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3e0e-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c3e0e-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3e0e-143">createdDateTime</span></span>|<span data-ttu-id="c3e0e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3e0e-144">DateTimeOffset</span></span>|<span data-ttu-id="c3e0e-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3e0e-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c3e0e-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3e0e-146">lastModifiedDateTime</span></span>|<span data-ttu-id="c3e0e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3e0e-147">DateTimeOffset</span></span>|<span data-ttu-id="c3e0e-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3e0e-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c3e0e-149">Version</span><span class="sxs-lookup"><span data-stu-id="c3e0e-149">version</span></span>|<span data-ttu-id="c3e0e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c3e0e-150">Int32</span></span>|<span data-ttu-id="c3e0e-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c3e0e-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c3e0e-152">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="c3e0e-152">limit</span></span>|<span data-ttu-id="c3e0e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c3e0e-153">Int32</span></span>|<span data-ttu-id="c3e0e-154">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c3e0e-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c3e0e-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3e0e-155">Response</span></span>
<span data-ttu-id="c3e0e-156">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3e0e-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3e0e-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c3e0e-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3e0e-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3e0e-158">Request</span></span>
<span data-ttu-id="c3e0e-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c3e0e-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="c3e0e-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3e0e-160">Response</span></span>
<span data-ttu-id="c3e0e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3e0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```



