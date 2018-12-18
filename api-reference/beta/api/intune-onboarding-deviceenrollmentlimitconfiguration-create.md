---
title: deviceEnrollmentLimitConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentLimitConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: fdb9fee09f43890280ef0beb79d6d57d9def67f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359668"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="a549e-103">deviceEnrollmentLimitConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="a549e-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="a549e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a549e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a549e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a549e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a549e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a549e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a549e-107">Erstellen eines neuen [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a549e-107">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a549e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a549e-108">Prerequisites</span></span>
<span data-ttu-id="a549e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a549e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a549e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a549e-111">Permission type</span></span>|<span data-ttu-id="a549e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a549e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a549e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a549e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a549e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a549e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a549e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a549e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a549e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a549e-116">Not supported.</span></span>|
|<span data-ttu-id="a549e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a549e-117">Application</span></span>|<span data-ttu-id="a549e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a549e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a549e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a549e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a549e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a549e-120">Request headers</span></span>
|<span data-ttu-id="a549e-121">Header</span><span class="sxs-lookup"><span data-stu-id="a549e-121">Header</span></span>|<span data-ttu-id="a549e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a549e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a549e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a549e-123">Authorization</span></span>|<span data-ttu-id="a549e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a549e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a549e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a549e-125">Accept</span></span>|<span data-ttu-id="a549e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a549e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a549e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a549e-127">Request body</span></span>
<span data-ttu-id="a549e-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentLimitConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="a549e-128">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="a549e-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentLimitConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a549e-129">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="a549e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a549e-130">Property</span></span>|<span data-ttu-id="a549e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a549e-131">Type</span></span>|<span data-ttu-id="a549e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a549e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a549e-133">id</span><span class="sxs-lookup"><span data-stu-id="a549e-133">id</span></span>|<span data-ttu-id="a549e-134">String</span><span class="sxs-lookup"><span data-stu-id="a549e-134">String</span></span>|<span data-ttu-id="a549e-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a549e-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a549e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a549e-136">displayName</span></span>|<span data-ttu-id="a549e-137">String</span><span class="sxs-lookup"><span data-stu-id="a549e-137">String</span></span>|<span data-ttu-id="a549e-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a549e-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a549e-139">description</span><span class="sxs-lookup"><span data-stu-id="a549e-139">description</span></span>|<span data-ttu-id="a549e-140">String</span><span class="sxs-lookup"><span data-stu-id="a549e-140">String</span></span>|<span data-ttu-id="a549e-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a549e-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a549e-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="a549e-142">priority</span></span>|<span data-ttu-id="a549e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a549e-143">Int32</span></span>|<span data-ttu-id="a549e-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a549e-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a549e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a549e-145">createdDateTime</span></span>|<span data-ttu-id="a549e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a549e-146">DateTimeOffset</span></span>|<span data-ttu-id="a549e-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a549e-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a549e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a549e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="a549e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a549e-149">DateTimeOffset</span></span>|<span data-ttu-id="a549e-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a549e-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a549e-151">Version</span><span class="sxs-lookup"><span data-stu-id="a549e-151">version</span></span>|<span data-ttu-id="a549e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a549e-152">Int32</span></span>|<span data-ttu-id="a549e-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a549e-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a549e-154">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="a549e-154">limit</span></span>|<span data-ttu-id="a549e-155">Int32</span><span class="sxs-lookup"><span data-stu-id="a549e-155">Int32</span></span>|<span data-ttu-id="a549e-156">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="a549e-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a549e-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="a549e-157">Response</span></span>
<span data-ttu-id="a549e-158">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a549e-158">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a549e-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a549e-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="a549e-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a549e-160">Request</span></span>
<span data-ttu-id="a549e-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a549e-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="a549e-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="a549e-162">Response</span></span>
<span data-ttu-id="a549e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a549e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





