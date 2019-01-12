---
title: deviceEnrollmentLimitConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentLimitConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c48737fc23bca51da51c3b93b035744c83025b13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943354"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="86e95-103">deviceEnrollmentLimitConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="86e95-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="86e95-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="86e95-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86e95-105">Aktualisieren der Eigenschaften eines [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="86e95-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="86e95-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="86e95-106">Prerequisites</span></span>
<span data-ttu-id="86e95-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86e95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86e95-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="86e95-109">Permission type</span></span>|<span data-ttu-id="86e95-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="86e95-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86e95-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="86e95-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86e95-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86e95-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="86e95-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="86e95-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86e95-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86e95-114">Not supported.</span></span>|
|<span data-ttu-id="86e95-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="86e95-115">Application</span></span>|<span data-ttu-id="86e95-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="86e95-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86e95-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="86e95-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="86e95-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="86e95-118">Request headers</span></span>
|<span data-ttu-id="86e95-119">Header</span><span class="sxs-lookup"><span data-stu-id="86e95-119">Header</span></span>|<span data-ttu-id="86e95-120">Wert</span><span class="sxs-lookup"><span data-stu-id="86e95-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86e95-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86e95-121">Authorization</span></span>|<span data-ttu-id="86e95-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="86e95-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86e95-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="86e95-123">Accept</span></span>|<span data-ttu-id="86e95-124">application/json</span><span class="sxs-lookup"><span data-stu-id="86e95-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86e95-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="86e95-125">Request body</span></span>
<span data-ttu-id="86e95-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das Objekt [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="86e95-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="86e95-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="86e95-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="86e95-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86e95-128">Property</span></span>|<span data-ttu-id="86e95-129">Typ</span><span class="sxs-lookup"><span data-stu-id="86e95-129">Type</span></span>|<span data-ttu-id="86e95-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86e95-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86e95-131">id</span><span class="sxs-lookup"><span data-stu-id="86e95-131">id</span></span>|<span data-ttu-id="86e95-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86e95-132">String</span></span>|<span data-ttu-id="86e95-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86e95-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86e95-134">displayName</span><span class="sxs-lookup"><span data-stu-id="86e95-134">displayName</span></span>|<span data-ttu-id="86e95-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86e95-135">String</span></span>|<span data-ttu-id="86e95-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86e95-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86e95-137">description</span><span class="sxs-lookup"><span data-stu-id="86e95-137">description</span></span>|<span data-ttu-id="86e95-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86e95-138">String</span></span>|<span data-ttu-id="86e95-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86e95-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86e95-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="86e95-140">priority</span></span>|<span data-ttu-id="86e95-141">Int32</span><span class="sxs-lookup"><span data-stu-id="86e95-141">Int32</span></span>|<span data-ttu-id="86e95-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86e95-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86e95-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86e95-143">createdDateTime</span></span>|<span data-ttu-id="86e95-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86e95-144">DateTimeOffset</span></span>|<span data-ttu-id="86e95-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86e95-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86e95-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86e95-146">lastModifiedDateTime</span></span>|<span data-ttu-id="86e95-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86e95-147">DateTimeOffset</span></span>|<span data-ttu-id="86e95-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86e95-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86e95-149">Version</span><span class="sxs-lookup"><span data-stu-id="86e95-149">version</span></span>|<span data-ttu-id="86e95-150">Int32</span><span class="sxs-lookup"><span data-stu-id="86e95-150">Int32</span></span>|<span data-ttu-id="86e95-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86e95-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="86e95-152">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="86e95-152">limit</span></span>|<span data-ttu-id="86e95-153">Int32</span><span class="sxs-lookup"><span data-stu-id="86e95-153">Int32</span></span>|<span data-ttu-id="86e95-154">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="86e95-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="86e95-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="86e95-155">Response</span></span>
<span data-ttu-id="86e95-156">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86e95-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86e95-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="86e95-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="86e95-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="86e95-158">Request</span></span>
<span data-ttu-id="86e95-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="86e95-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="86e95-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="86e95-160">Response</span></span>
<span data-ttu-id="86e95-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="86e95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



