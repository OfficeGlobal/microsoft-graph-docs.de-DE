---
title: deviceEnrollmentLimitConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentLimitConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: afcd7a866275d8178dc1ab929bdde614e3d519a6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416489"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="27217-103">deviceEnrollmentLimitConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="27217-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="27217-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="27217-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="27217-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="27217-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27217-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="27217-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27217-107">Aktualisieren der Eigenschaften eines [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="27217-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27217-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="27217-108">Prerequisites</span></span>
<span data-ttu-id="27217-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="27217-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="27217-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="27217-111">Permission type</span></span>|<span data-ttu-id="27217-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="27217-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27217-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="27217-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27217-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27217-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="27217-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="27217-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27217-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27217-116">Not supported.</span></span>|
|<span data-ttu-id="27217-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="27217-117">Application</span></span>|<span data-ttu-id="27217-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27217-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27217-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="27217-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="27217-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="27217-120">Request headers</span></span>
|<span data-ttu-id="27217-121">Header</span><span class="sxs-lookup"><span data-stu-id="27217-121">Header</span></span>|<span data-ttu-id="27217-122">Wert</span><span class="sxs-lookup"><span data-stu-id="27217-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27217-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="27217-123">Authorization</span></span>|<span data-ttu-id="27217-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="27217-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27217-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="27217-125">Accept</span></span>|<span data-ttu-id="27217-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27217-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27217-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="27217-127">Request body</span></span>
<span data-ttu-id="27217-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das Objekt [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="27217-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="27217-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="27217-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="27217-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27217-130">Property</span></span>|<span data-ttu-id="27217-131">Typ</span><span class="sxs-lookup"><span data-stu-id="27217-131">Type</span></span>|<span data-ttu-id="27217-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27217-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27217-133">id</span><span class="sxs-lookup"><span data-stu-id="27217-133">id</span></span>|<span data-ttu-id="27217-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27217-134">String</span></span>|<span data-ttu-id="27217-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27217-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27217-136">displayName</span><span class="sxs-lookup"><span data-stu-id="27217-136">displayName</span></span>|<span data-ttu-id="27217-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27217-137">String</span></span>|<span data-ttu-id="27217-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27217-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27217-139">description</span><span class="sxs-lookup"><span data-stu-id="27217-139">description</span></span>|<span data-ttu-id="27217-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27217-140">String</span></span>|<span data-ttu-id="27217-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27217-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27217-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="27217-142">priority</span></span>|<span data-ttu-id="27217-143">Int32</span><span class="sxs-lookup"><span data-stu-id="27217-143">Int32</span></span>|<span data-ttu-id="27217-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27217-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27217-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27217-145">createdDateTime</span></span>|<span data-ttu-id="27217-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27217-146">DateTimeOffset</span></span>|<span data-ttu-id="27217-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27217-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27217-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27217-148">lastModifiedDateTime</span></span>|<span data-ttu-id="27217-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27217-149">DateTimeOffset</span></span>|<span data-ttu-id="27217-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27217-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27217-151">Version</span><span class="sxs-lookup"><span data-stu-id="27217-151">version</span></span>|<span data-ttu-id="27217-152">Int32</span><span class="sxs-lookup"><span data-stu-id="27217-152">Int32</span></span>|<span data-ttu-id="27217-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="27217-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="27217-154">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="27217-154">limit</span></span>|<span data-ttu-id="27217-155">Int32</span><span class="sxs-lookup"><span data-stu-id="27217-155">Int32</span></span>|<span data-ttu-id="27217-156">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="27217-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="27217-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="27217-157">Response</span></span>
<span data-ttu-id="27217-158">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="27217-158">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27217-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="27217-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="27217-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="27217-160">Request</span></span>
<span data-ttu-id="27217-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="27217-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="27217-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="27217-162">Response</span></span>
<span data-ttu-id="27217-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="27217-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




