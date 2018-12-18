---
title: deviceEnrollmentLimitConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentLimitConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 2d285ad19e907e40494c5ff7da9e112be3a20112
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329512"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="b7fef-103">deviceEnrollmentLimitConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b7fef-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="b7fef-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b7fef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7fef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b7fef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7fef-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b7fef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7fef-107">Aktualisieren der Eigenschaften eines [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b7fef-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b7fef-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b7fef-108">Prerequisites</span></span>
<span data-ttu-id="b7fef-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7fef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7fef-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b7fef-111">Permission type</span></span>|<span data-ttu-id="b7fef-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b7fef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7fef-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b7fef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7fef-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7fef-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b7fef-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b7fef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7fef-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7fef-116">Not supported.</span></span>|
|<span data-ttu-id="b7fef-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b7fef-117">Application</span></span>|<span data-ttu-id="b7fef-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7fef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7fef-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7fef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b7fef-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b7fef-120">Request headers</span></span>
|<span data-ttu-id="b7fef-121">Header</span><span class="sxs-lookup"><span data-stu-id="b7fef-121">Header</span></span>|<span data-ttu-id="b7fef-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b7fef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7fef-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b7fef-123">Authorization</span></span>|<span data-ttu-id="b7fef-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b7fef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7fef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b7fef-125">Accept</span></span>|<span data-ttu-id="b7fef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7fef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7fef-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b7fef-127">Request body</span></span>
<span data-ttu-id="b7fef-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das Objekt [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="b7fef-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="b7fef-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b7fef-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="b7fef-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b7fef-130">Property</span></span>|<span data-ttu-id="b7fef-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b7fef-131">Type</span></span>|<span data-ttu-id="b7fef-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7fef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7fef-133">id</span><span class="sxs-lookup"><span data-stu-id="b7fef-133">id</span></span>|<span data-ttu-id="b7fef-134">String</span><span class="sxs-lookup"><span data-stu-id="b7fef-134">String</span></span>|<span data-ttu-id="b7fef-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7fef-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b7fef-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b7fef-136">displayName</span></span>|<span data-ttu-id="b7fef-137">String</span><span class="sxs-lookup"><span data-stu-id="b7fef-137">String</span></span>|<span data-ttu-id="b7fef-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7fef-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b7fef-139">description</span><span class="sxs-lookup"><span data-stu-id="b7fef-139">description</span></span>|<span data-ttu-id="b7fef-140">String</span><span class="sxs-lookup"><span data-stu-id="b7fef-140">String</span></span>|<span data-ttu-id="b7fef-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7fef-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b7fef-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="b7fef-142">priority</span></span>|<span data-ttu-id="b7fef-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b7fef-143">Int32</span></span>|<span data-ttu-id="b7fef-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7fef-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b7fef-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7fef-145">createdDateTime</span></span>|<span data-ttu-id="b7fef-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7fef-146">DateTimeOffset</span></span>|<span data-ttu-id="b7fef-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7fef-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b7fef-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7fef-148">lastModifiedDateTime</span></span>|<span data-ttu-id="b7fef-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7fef-149">DateTimeOffset</span></span>|<span data-ttu-id="b7fef-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7fef-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b7fef-151">Version</span><span class="sxs-lookup"><span data-stu-id="b7fef-151">version</span></span>|<span data-ttu-id="b7fef-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b7fef-152">Int32</span></span>|<span data-ttu-id="b7fef-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7fef-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="b7fef-154">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="b7fef-154">limit</span></span>|<span data-ttu-id="b7fef-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b7fef-155">Int32</span></span>|<span data-ttu-id="b7fef-156">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b7fef-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b7fef-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7fef-157">Response</span></span>
<span data-ttu-id="b7fef-158">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7fef-158">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7fef-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b7fef-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="b7fef-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7fef-160">Request</span></span>
<span data-ttu-id="b7fef-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b7fef-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7fef-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7fef-162">Response</span></span>
<span data-ttu-id="b7fef-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7fef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





