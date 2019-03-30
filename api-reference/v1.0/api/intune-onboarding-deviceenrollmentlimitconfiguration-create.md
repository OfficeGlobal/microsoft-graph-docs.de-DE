---
title: deviceEnrollmentLimitConfiguration erstellen
description: Erstellen eines neuen deviceEnrollmentLimitConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a331e49ea65450012d5f632b88579044382c9a1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986376"
---
# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="ce494-103">deviceEnrollmentLimitConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="ce494-103">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="ce494-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ce494-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce494-105">Erstellen eines neuen [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ce494-105">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce494-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ce494-106">Prerequisites</span></span>
<span data-ttu-id="ce494-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce494-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce494-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce494-109">Permission type</span></span>|<span data-ttu-id="ce494-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce494-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce494-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce494-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce494-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce494-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ce494-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce494-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce494-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce494-114">Not supported.</span></span>|
|<span data-ttu-id="ce494-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce494-115">Application</span></span>|<span data-ttu-id="ce494-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce494-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce494-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce494-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ce494-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce494-118">Request headers</span></span>
|<span data-ttu-id="ce494-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ce494-119">Header</span></span>|<span data-ttu-id="ce494-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ce494-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce494-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce494-121">Authorization</span></span>|<span data-ttu-id="ce494-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ce494-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce494-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ce494-123">Accept</span></span>|<span data-ttu-id="ce494-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ce494-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce494-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce494-125">Request body</span></span>
<span data-ttu-id="ce494-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceEnrollmentLimitConfiguration-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ce494-126">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="ce494-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceEnrollmentLimitConfiguration erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ce494-127">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="ce494-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce494-128">Property</span></span>|<span data-ttu-id="ce494-129">Typ</span><span class="sxs-lookup"><span data-stu-id="ce494-129">Type</span></span>|<span data-ttu-id="ce494-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce494-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce494-131">id</span><span class="sxs-lookup"><span data-stu-id="ce494-131">id</span></span>|<span data-ttu-id="ce494-132">String</span><span class="sxs-lookup"><span data-stu-id="ce494-132">String</span></span>|<span data-ttu-id="ce494-133">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce494-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce494-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ce494-134">displayName</span></span>|<span data-ttu-id="ce494-135">String</span><span class="sxs-lookup"><span data-stu-id="ce494-135">String</span></span>|<span data-ttu-id="ce494-136">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce494-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce494-137">description</span><span class="sxs-lookup"><span data-stu-id="ce494-137">description</span></span>|<span data-ttu-id="ce494-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce494-138">String</span></span>|<span data-ttu-id="ce494-139">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce494-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce494-140">Priorität</span><span class="sxs-lookup"><span data-stu-id="ce494-140">priority</span></span>|<span data-ttu-id="ce494-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ce494-141">Int32</span></span>|<span data-ttu-id="ce494-142">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce494-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce494-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce494-143">createdDateTime</span></span>|<span data-ttu-id="ce494-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce494-144">DateTimeOffset</span></span>|<span data-ttu-id="ce494-145">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce494-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce494-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce494-146">lastModifiedDateTime</span></span>|<span data-ttu-id="ce494-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce494-147">DateTimeOffset</span></span>|<span data-ttu-id="ce494-148">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce494-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce494-149">Version</span><span class="sxs-lookup"><span data-stu-id="ce494-149">version</span></span>|<span data-ttu-id="ce494-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ce494-150">Int32</span></span>|<span data-ttu-id="ce494-151">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce494-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ce494-152">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="ce494-152">limit</span></span>|<span data-ttu-id="ce494-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ce494-153">Int32</span></span>|<span data-ttu-id="ce494-154">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ce494-154">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ce494-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce494-155">Response</span></span>
<span data-ttu-id="ce494-156">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce494-156">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce494-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce494-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce494-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce494-158">Request</span></span>
<span data-ttu-id="ce494-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce494-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ce494-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce494-160">Response</span></span>
<span data-ttu-id="ce494-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce494-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



