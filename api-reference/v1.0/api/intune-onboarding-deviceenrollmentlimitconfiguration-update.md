---
title: deviceEnrollmentLimitConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentLimitConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 842c9d6c1cf6e805850317bb804cb8905c189134
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254177"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="4f2b5-103">deviceEnrollmentLimitConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4f2b5-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="4f2b5-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4f2b5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f2b5-105">Aktualisieren der Eigenschaften eines [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4f2b5-105">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f2b5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4f2b5-106">Prerequisites</span></span>
<span data-ttu-id="4f2b5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f2b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4f2b5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4f2b5-109">Permission type</span></span>|<span data-ttu-id="4f2b5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4f2b5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f2b5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4f2b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4f2b5-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f2b5-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4f2b5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4f2b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f2b5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f2b5-114">Not supported.</span></span>|
|<span data-ttu-id="4f2b5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4f2b5-115">Application</span></span>|<span data-ttu-id="4f2b5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f2b5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f2b5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f2b5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4f2b5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4f2b5-118">Request headers</span></span>
|<span data-ttu-id="4f2b5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4f2b5-119">Header</span></span>|<span data-ttu-id="4f2b5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4f2b5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f2b5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f2b5-121">Authorization</span></span>|<span data-ttu-id="4f2b5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4f2b5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f2b5-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4f2b5-123">Accept</span></span>|<span data-ttu-id="4f2b5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4f2b5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f2b5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4f2b5-125">Request body</span></span>
<span data-ttu-id="4f2b5-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das Objekt [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="4f2b5-126">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="4f2b5-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4f2b5-127">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="4f2b5-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4f2b5-128">Property</span></span>|<span data-ttu-id="4f2b5-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4f2b5-129">Type</span></span>|<span data-ttu-id="4f2b5-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f2b5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f2b5-131">id</span><span class="sxs-lookup"><span data-stu-id="4f2b5-131">id</span></span>|<span data-ttu-id="4f2b5-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f2b5-132">String</span></span>|<span data-ttu-id="4f2b5-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2b5-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4f2b5-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4f2b5-134">displayName</span></span>|<span data-ttu-id="4f2b5-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f2b5-135">String</span></span>|<span data-ttu-id="4f2b5-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2b5-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4f2b5-137">description</span><span class="sxs-lookup"><span data-stu-id="4f2b5-137">description</span></span>|<span data-ttu-id="4f2b5-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f2b5-138">String</span></span>|<span data-ttu-id="4f2b5-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2b5-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4f2b5-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="4f2b5-140">priority</span></span>|<span data-ttu-id="4f2b5-141">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2b5-141">Int32</span></span>|<span data-ttu-id="4f2b5-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2b5-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4f2b5-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f2b5-143">createdDateTime</span></span>|<span data-ttu-id="4f2b5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f2b5-144">DateTimeOffset</span></span>|<span data-ttu-id="4f2b5-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2b5-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4f2b5-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f2b5-146">lastModifiedDateTime</span></span>|<span data-ttu-id="4f2b5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f2b5-147">DateTimeOffset</span></span>|<span data-ttu-id="4f2b5-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2b5-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4f2b5-149">Version</span><span class="sxs-lookup"><span data-stu-id="4f2b5-149">version</span></span>|<span data-ttu-id="4f2b5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2b5-150">Int32</span></span>|<span data-ttu-id="4f2b5-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2b5-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="4f2b5-152">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="4f2b5-152">limit</span></span>|<span data-ttu-id="4f2b5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2b5-153">Int32</span></span>|<span data-ttu-id="4f2b5-154">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4f2b5-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4f2b5-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f2b5-155">Response</span></span>
<span data-ttu-id="4f2b5-156">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f2b5-156">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f2b5-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4f2b5-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f2b5-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f2b5-158">Request</span></span>
<span data-ttu-id="4f2b5-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4f2b5-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f2b5-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f2b5-160">Response</span></span>
<span data-ttu-id="4f2b5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f2b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



