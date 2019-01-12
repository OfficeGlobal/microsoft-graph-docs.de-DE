---
title: deviceEnrollmentLimitConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines deviceEnrollmentLimitConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 651649b36b2aa08c651640caa0f854f2b2ff98fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926512"
---
# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="29d0b-103">deviceEnrollmentLimitConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="29d0b-103">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="29d0b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="29d0b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29d0b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="29d0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29d0b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="29d0b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29d0b-107">Aktualisieren der Eigenschaften eines [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="29d0b-107">Update the properties of a [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29d0b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="29d0b-108">Prerequisites</span></span>
<span data-ttu-id="29d0b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29d0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29d0b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29d0b-111">Permission type</span></span>|<span data-ttu-id="29d0b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29d0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29d0b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29d0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29d0b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29d0b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="29d0b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29d0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29d0b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29d0b-116">Not supported.</span></span>|
|<span data-ttu-id="29d0b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29d0b-117">Application</span></span>|<span data-ttu-id="29d0b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29d0b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29d0b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29d0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="29d0b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29d0b-120">Request headers</span></span>
|<span data-ttu-id="29d0b-121">Header</span><span class="sxs-lookup"><span data-stu-id="29d0b-121">Header</span></span>|<span data-ttu-id="29d0b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="29d0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29d0b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29d0b-123">Authorization</span></span>|<span data-ttu-id="29d0b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="29d0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29d0b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="29d0b-125">Accept</span></span>|<span data-ttu-id="29d0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29d0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29d0b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29d0b-127">Request body</span></span>
<span data-ttu-id="29d0b-128">Geben Sie im Anforderungstext eine JSON-Darstellung für das Objekt [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="29d0b-128">In the request body, supply a JSON representation for the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="29d0b-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="29d0b-129">The following table shows the properties that are required when you create the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md).</span></span>

|<span data-ttu-id="29d0b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="29d0b-130">Property</span></span>|<span data-ttu-id="29d0b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="29d0b-131">Type</span></span>|<span data-ttu-id="29d0b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29d0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29d0b-133">id</span><span class="sxs-lookup"><span data-stu-id="29d0b-133">id</span></span>|<span data-ttu-id="29d0b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29d0b-134">String</span></span>|<span data-ttu-id="29d0b-135">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29d0b-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29d0b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="29d0b-136">displayName</span></span>|<span data-ttu-id="29d0b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29d0b-137">String</span></span>|<span data-ttu-id="29d0b-138">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29d0b-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29d0b-139">description</span><span class="sxs-lookup"><span data-stu-id="29d0b-139">description</span></span>|<span data-ttu-id="29d0b-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="29d0b-140">String</span></span>|<span data-ttu-id="29d0b-141">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29d0b-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29d0b-142">Priorität</span><span class="sxs-lookup"><span data-stu-id="29d0b-142">priority</span></span>|<span data-ttu-id="29d0b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="29d0b-143">Int32</span></span>|<span data-ttu-id="29d0b-144">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29d0b-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29d0b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29d0b-145">createdDateTime</span></span>|<span data-ttu-id="29d0b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29d0b-146">DateTimeOffset</span></span>|<span data-ttu-id="29d0b-147">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29d0b-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29d0b-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29d0b-148">lastModifiedDateTime</span></span>|<span data-ttu-id="29d0b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29d0b-149">DateTimeOffset</span></span>|<span data-ttu-id="29d0b-150">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29d0b-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29d0b-151">Version</span><span class="sxs-lookup"><span data-stu-id="29d0b-151">version</span></span>|<span data-ttu-id="29d0b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="29d0b-152">Int32</span></span>|<span data-ttu-id="29d0b-153">Noch nicht dokumentiert. Geerbt von [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29d0b-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="29d0b-154">Begrenzung</span><span class="sxs-lookup"><span data-stu-id="29d0b-154">limit</span></span>|<span data-ttu-id="29d0b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="29d0b-155">Int32</span></span>|<span data-ttu-id="29d0b-156">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="29d0b-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="29d0b-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="29d0b-157">Response</span></span>
<span data-ttu-id="29d0b-158">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29d0b-158">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29d0b-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29d0b-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="29d0b-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29d0b-160">Request</span></span>
<span data-ttu-id="29d0b-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29d0b-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="29d0b-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="29d0b-162">Response</span></span>
<span data-ttu-id="29d0b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29d0b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





