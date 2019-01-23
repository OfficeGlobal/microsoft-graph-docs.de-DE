---
title: Erstellen von macOSTrustedRootCertificate
description: Erstellen eines neuen MacOSTrustedRootCertificate-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e8428113174a2be44f1f17ac507ac16bdf6c7ec0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403917"
---
# <a name="create-macostrustedrootcertificate"></a><span data-ttu-id="a6e65-103">Erstellen von macOSTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a6e65-103">Create macOSTrustedRootCertificate</span></span>

> <span data-ttu-id="a6e65-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a6e65-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a6e65-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6e65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6e65-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a6e65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6e65-107">Erstellen eines neuen [MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6e65-107">Create a new [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6e65-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a6e65-108">Prerequisites</span></span>
<span data-ttu-id="a6e65-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a6e65-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6e65-111">Permission type</span></span>|<span data-ttu-id="a6e65-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6e65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6e65-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6e65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6e65-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6e65-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6e65-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6e65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6e65-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6e65-116">Not supported.</span></span>|
|<span data-ttu-id="a6e65-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6e65-117">Application</span></span>|<span data-ttu-id="a6e65-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6e65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6e65-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6e65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a6e65-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6e65-120">Request headers</span></span>
|<span data-ttu-id="a6e65-121">Header</span><span class="sxs-lookup"><span data-stu-id="a6e65-121">Header</span></span>|<span data-ttu-id="a6e65-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a6e65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6e65-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a6e65-123">Authorization</span></span>|<span data-ttu-id="a6e65-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a6e65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6e65-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a6e65-125">Accept</span></span>|<span data-ttu-id="a6e65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6e65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6e65-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6e65-127">Request body</span></span>
<span data-ttu-id="a6e65-128">Geben Sie im Textkörper Anforderung für das Objekt MacOSTrustedRootCertificate eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a6e65-128">In the request body, supply a JSON representation for the macOSTrustedRootCertificate object.</span></span>

<span data-ttu-id="a6e65-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MacOSTrustedRootCertificate erstellen.</span><span class="sxs-lookup"><span data-stu-id="a6e65-129">The following table shows the properties that are required when you create the macOSTrustedRootCertificate.</span></span>

|<span data-ttu-id="a6e65-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6e65-130">Property</span></span>|<span data-ttu-id="a6e65-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a6e65-131">Type</span></span>|<span data-ttu-id="a6e65-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6e65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6e65-133">id</span><span class="sxs-lookup"><span data-stu-id="a6e65-133">id</span></span>|<span data-ttu-id="a6e65-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a6e65-134">String</span></span>|<span data-ttu-id="a6e65-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a6e65-135">Key of the entity.</span></span> <span data-ttu-id="a6e65-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6e65-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a6e65-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6e65-138">DateTimeOffset</span></span>|<span data-ttu-id="a6e65-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6e65-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a6e65-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a6e65-141">roleScopeTagIds</span></span>|<span data-ttu-id="a6e65-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a6e65-142">String collection</span></span>|<span data-ttu-id="a6e65-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="a6e65-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a6e65-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a6e65-145">supportsScopeTags</span></span>|<span data-ttu-id="a6e65-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6e65-146">Boolean</span></span>|<span data-ttu-id="a6e65-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6e65-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a6e65-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a6e65-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a6e65-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="a6e65-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a6e65-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a6e65-150">This property is read-only.</span></span> <span data-ttu-id="a6e65-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6e65-152">createdDateTime</span></span>|<span data-ttu-id="a6e65-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6e65-153">DateTimeOffset</span></span>|<span data-ttu-id="a6e65-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6e65-154">DateTime the object was created.</span></span> <span data-ttu-id="a6e65-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-156">description</span><span class="sxs-lookup"><span data-stu-id="a6e65-156">description</span></span>|<span data-ttu-id="a6e65-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a6e65-157">String</span></span>|<span data-ttu-id="a6e65-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a6e65-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a6e65-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a6e65-160">displayName</span></span>|<span data-ttu-id="a6e65-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a6e65-161">String</span></span>|<span data-ttu-id="a6e65-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a6e65-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a6e65-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-164">Version</span><span class="sxs-lookup"><span data-stu-id="a6e65-164">version</span></span>|<span data-ttu-id="a6e65-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a6e65-165">Int32</span></span>|<span data-ttu-id="a6e65-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a6e65-166">Version of the device configuration.</span></span> <span data-ttu-id="a6e65-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a6e65-168">trustedRootCertificate</span></span>|<span data-ttu-id="a6e65-169">Binär</span><span class="sxs-lookup"><span data-stu-id="a6e65-169">Binary</span></span>|<span data-ttu-id="a6e65-170">Zertifikat der vertrauenswürdigen Stammzertifizierungsstellen.</span><span class="sxs-lookup"><span data-stu-id="a6e65-170">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="a6e65-171">Aus</span><span class="sxs-lookup"><span data-stu-id="a6e65-171">certFileName</span></span>|<span data-ttu-id="a6e65-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a6e65-172">String</span></span>|<span data-ttu-id="a6e65-173">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a6e65-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="a6e65-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6e65-174">Response</span></span>
<span data-ttu-id="a6e65-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MacOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a6e65-175">If successful, this method returns a `201 Created` response code and a [macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6e65-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6e65-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6e65-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6e65-177">Request</span></span>
<span data-ttu-id="a6e65-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6e65-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 365

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="a6e65-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6e65-179">Response</span></span>
<span data-ttu-id="a6e65-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6e65-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 537

{
  "@odata.type": "#microsoft.graph.macOSTrustedRootCertificate",
  "id": "c5fac954-c954-c5fa-54c9-fac554c9fac5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```




