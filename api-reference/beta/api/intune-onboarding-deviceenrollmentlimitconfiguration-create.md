---
title: deviceEnrollmentLimitConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentLimitConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95431986b1b8a47c723f493295b64989bb3db3d5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165352"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="06294-103">deviceEnrollmentLimitConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="06294-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="06294-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06294-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06294-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="06294-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06294-106">Erstellen eines neuen [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="06294-106">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06294-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="06294-107">Prerequisites</span></span>
<span data-ttu-id="06294-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="06294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="06294-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06294-110">Permission type</span></span>|<span data-ttu-id="06294-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06294-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06294-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06294-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06294-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06294-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="06294-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06294-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06294-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06294-115">Not supported.</span></span>|
|<span data-ttu-id="06294-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06294-116">Application</span></span>|<span data-ttu-id="06294-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06294-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06294-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06294-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="06294-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06294-119">Request headers</span></span>
|<span data-ttu-id="06294-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="06294-120">Header</span></span>|<span data-ttu-id="06294-121">Wert</span><span class="sxs-lookup"><span data-stu-id="06294-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06294-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06294-122">Authorization</span></span>|<span data-ttu-id="06294-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="06294-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06294-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="06294-124">Accept</span></span>|<span data-ttu-id="06294-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06294-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06294-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06294-126">Request body</span></span>
<span data-ttu-id="06294-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentLimitConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="06294-127">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="06294-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentLimitConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="06294-128">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="06294-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06294-129">Property</span></span>|<span data-ttu-id="06294-130">Typ</span><span class="sxs-lookup"><span data-stu-id="06294-130">Type</span></span>|<span data-ttu-id="06294-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06294-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06294-132">id</span><span class="sxs-lookup"><span data-stu-id="06294-132">id</span></span>|<span data-ttu-id="06294-133">string</span><span class="sxs-lookup"><span data-stu-id="06294-133">String</span></span>|<span data-ttu-id="06294-134">ID der von [DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) geerbten Konfiguration der Registrierungs Status Seite</span><span class="sxs-lookup"><span data-stu-id="06294-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06294-135">displayName</span><span class="sxs-lookup"><span data-stu-id="06294-135">displayName</span></span>|<span data-ttu-id="06294-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06294-136">String</span></span>|<span data-ttu-id="06294-137">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06294-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06294-138">description</span><span class="sxs-lookup"><span data-stu-id="06294-138">description</span></span>|<span data-ttu-id="06294-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06294-139">String</span></span>|<span data-ttu-id="06294-140">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06294-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06294-141">Priorität</span><span class="sxs-lookup"><span data-stu-id="06294-141">priority</span></span>|<span data-ttu-id="06294-142">Int32</span><span class="sxs-lookup"><span data-stu-id="06294-142">Int32</span></span>|<span data-ttu-id="06294-143">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06294-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06294-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06294-144">createdDateTime</span></span>|<span data-ttu-id="06294-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06294-145">DateTimeOffset</span></span>|<span data-ttu-id="06294-146">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06294-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06294-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06294-147">lastModifiedDateTime</span></span>|<span data-ttu-id="06294-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06294-148">DateTimeOffset</span></span>|<span data-ttu-id="06294-149">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06294-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06294-150">Version</span><span class="sxs-lookup"><span data-stu-id="06294-150">version</span></span>|<span data-ttu-id="06294-151">Int32</span><span class="sxs-lookup"><span data-stu-id="06294-151">Int32</span></span>|<span data-ttu-id="06294-152">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06294-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="06294-153">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="06294-153">limit</span></span>|<span data-ttu-id="06294-154">Int32</span><span class="sxs-lookup"><span data-stu-id="06294-154">Int32</span></span>|<span data-ttu-id="06294-155">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="06294-155">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="06294-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="06294-156">Response</span></span>
<span data-ttu-id="06294-157">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06294-157">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06294-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06294-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="06294-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06294-159">Request</span></span>
<span data-ttu-id="06294-160">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06294-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="06294-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="06294-161">Response</span></span>
<span data-ttu-id="06294-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06294-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




