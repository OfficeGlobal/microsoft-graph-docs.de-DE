---
title: deviceEnrollmentLimitConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentLimitConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bd4b1c581260a7cd1438ddad6bc2e486af1ac679
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832889"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="615f8-103">deviceEnrollmentLimitConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="615f8-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="615f8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="615f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="615f8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="615f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="615f8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="615f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="615f8-107">Aktualisieren der Eigenschaften eines [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="615f8-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="615f8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="615f8-108">Prerequisites</span></span>
<span data-ttu-id="615f8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="615f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="615f8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="615f8-111">Permission type</span></span>|<span data-ttu-id="615f8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="615f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="615f8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="615f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="615f8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615f8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="615f8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="615f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="615f8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="615f8-116">Not supported.</span></span>|
|<span data-ttu-id="615f8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="615f8-117">Application</span></span>|<span data-ttu-id="615f8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="615f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="615f8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="615f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="615f8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="615f8-120">Request headers</span></span>
|<span data-ttu-id="615f8-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="615f8-121">Header</span></span>|<span data-ttu-id="615f8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="615f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="615f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="615f8-123">Authorization</span></span>|<span data-ttu-id="615f8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="615f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="615f8-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="615f8-125">Accept</span></span>|<span data-ttu-id="615f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="615f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="615f8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="615f8-127">Request body</span></span>
<span data-ttu-id="615f8-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das Objekt [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="615f8-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="615f8-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="615f8-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="615f8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="615f8-130">Property</span></span>|<span data-ttu-id="615f8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="615f8-131">Type</span></span>|<span data-ttu-id="615f8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="615f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="615f8-133">id</span><span class="sxs-lookup"><span data-stu-id="615f8-133">id</span></span>|<span data-ttu-id="615f8-134">String</span><span class="sxs-lookup"><span data-stu-id="615f8-134">String</span></span>|<span data-ttu-id="615f8-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615f8-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="615f8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="615f8-136">displayName</span></span>|<span data-ttu-id="615f8-137">String</span><span class="sxs-lookup"><span data-stu-id="615f8-137">String</span></span>|<span data-ttu-id="615f8-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615f8-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="615f8-139">description</span><span class="sxs-lookup"><span data-stu-id="615f8-139">description</span></span>|<span data-ttu-id="615f8-140">String</span><span class="sxs-lookup"><span data-stu-id="615f8-140">String</span></span>|<span data-ttu-id="615f8-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615f8-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="615f8-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="615f8-142">priority</span></span>|<span data-ttu-id="615f8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="615f8-143">Int32</span></span>|<span data-ttu-id="615f8-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615f8-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="615f8-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="615f8-145">createdDateTime</span></span>|<span data-ttu-id="615f8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="615f8-146">DateTimeOffset</span></span>|<span data-ttu-id="615f8-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615f8-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="615f8-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="615f8-148">lastModifiedDateTime</span></span>|<span data-ttu-id="615f8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="615f8-149">DateTimeOffset</span></span>|<span data-ttu-id="615f8-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615f8-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="615f8-151">Version</span><span class="sxs-lookup"><span data-stu-id="615f8-151">version</span></span>|<span data-ttu-id="615f8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="615f8-152">Int32</span></span>|<span data-ttu-id="615f8-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="615f8-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="615f8-154">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="615f8-154">limit</span></span>|<span data-ttu-id="615f8-155">Int32</span><span class="sxs-lookup"><span data-stu-id="615f8-155">Int32</span></span>|<span data-ttu-id="615f8-156">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="615f8-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="615f8-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="615f8-157">Response</span></span>
<span data-ttu-id="615f8-158">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="615f8-158">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="615f8-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="615f8-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="615f8-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="615f8-160">Request</span></span>
<span data-ttu-id="615f8-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="615f8-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 196

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="615f8-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="615f8-162">Response</span></span>
<span data-ttu-id="615f8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="615f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





