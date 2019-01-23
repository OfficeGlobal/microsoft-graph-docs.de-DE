---
title: Erstellen von androidForWorkTrustedRootCertificate
description: Erstellen eines neuen AndroidForWorkTrustedRootCertificate-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0831d39fb891acfca6f3ce3581ee1a9dc1fded0e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413514"
---
# <a name="create-androidforworktrustedrootcertificate"></a><span data-ttu-id="33484-103">Erstellen von androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="33484-103">Create androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="33484-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="33484-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="33484-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33484-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33484-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="33484-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33484-107">Erstellen eines neuen [AndroidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="33484-107">Create a new [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33484-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33484-108">Prerequisites</span></span>
<span data-ttu-id="33484-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="33484-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="33484-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33484-111">Permission type</span></span>|<span data-ttu-id="33484-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33484-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33484-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33484-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33484-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33484-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33484-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33484-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33484-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33484-116">Not supported.</span></span>|
|<span data-ttu-id="33484-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33484-117">Application</span></span>|<span data-ttu-id="33484-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33484-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33484-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33484-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="33484-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33484-120">Request headers</span></span>
|<span data-ttu-id="33484-121">Header</span><span class="sxs-lookup"><span data-stu-id="33484-121">Header</span></span>|<span data-ttu-id="33484-122">Wert</span><span class="sxs-lookup"><span data-stu-id="33484-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33484-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="33484-123">Authorization</span></span>|<span data-ttu-id="33484-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33484-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33484-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="33484-125">Accept</span></span>|<span data-ttu-id="33484-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33484-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33484-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33484-127">Request body</span></span>
<span data-ttu-id="33484-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidForWorkTrustedRootCertificate eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="33484-128">In the request body, supply a JSON representation for the androidForWorkTrustedRootCertificate object.</span></span>

<span data-ttu-id="33484-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidForWorkTrustedRootCertificate erstellen.</span><span class="sxs-lookup"><span data-stu-id="33484-129">The following table shows the properties that are required when you create the androidForWorkTrustedRootCertificate.</span></span>

|<span data-ttu-id="33484-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33484-130">Property</span></span>|<span data-ttu-id="33484-131">Typ</span><span class="sxs-lookup"><span data-stu-id="33484-131">Type</span></span>|<span data-ttu-id="33484-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33484-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33484-133">id</span><span class="sxs-lookup"><span data-stu-id="33484-133">id</span></span>|<span data-ttu-id="33484-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33484-134">String</span></span>|<span data-ttu-id="33484-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="33484-135">Key of the entity.</span></span> <span data-ttu-id="33484-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33484-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33484-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33484-137">lastModifiedDateTime</span></span>|<span data-ttu-id="33484-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33484-138">DateTimeOffset</span></span>|<span data-ttu-id="33484-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33484-139">DateTime the object was last modified.</span></span> <span data-ttu-id="33484-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33484-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33484-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="33484-141">roleScopeTagIds</span></span>|<span data-ttu-id="33484-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="33484-142">String collection</span></span>|<span data-ttu-id="33484-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="33484-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="33484-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33484-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33484-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="33484-145">supportsScopeTags</span></span>|<span data-ttu-id="33484-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="33484-146">Boolean</span></span>|<span data-ttu-id="33484-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33484-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="33484-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="33484-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="33484-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="33484-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="33484-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="33484-150">This property is read-only.</span></span> <span data-ttu-id="33484-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33484-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33484-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33484-152">createdDateTime</span></span>|<span data-ttu-id="33484-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33484-153">DateTimeOffset</span></span>|<span data-ttu-id="33484-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="33484-154">DateTime the object was created.</span></span> <span data-ttu-id="33484-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33484-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33484-156">description</span><span class="sxs-lookup"><span data-stu-id="33484-156">description</span></span>|<span data-ttu-id="33484-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33484-157">String</span></span>|<span data-ttu-id="33484-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33484-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="33484-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33484-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33484-160">displayName</span><span class="sxs-lookup"><span data-stu-id="33484-160">displayName</span></span>|<span data-ttu-id="33484-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33484-161">String</span></span>|<span data-ttu-id="33484-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="33484-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="33484-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33484-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33484-164">Version</span><span class="sxs-lookup"><span data-stu-id="33484-164">version</span></span>|<span data-ttu-id="33484-165">Int32</span><span class="sxs-lookup"><span data-stu-id="33484-165">Int32</span></span>|<span data-ttu-id="33484-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="33484-166">Version of the device configuration.</span></span> <span data-ttu-id="33484-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="33484-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="33484-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="33484-168">trustedRootCertificate</span></span>|<span data-ttu-id="33484-169">Binär</span><span class="sxs-lookup"><span data-stu-id="33484-169">Binary</span></span>|<span data-ttu-id="33484-170">Vertrauenswürdiges Zertifikat</span><span class="sxs-lookup"><span data-stu-id="33484-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="33484-171">Aus</span><span class="sxs-lookup"><span data-stu-id="33484-171">certFileName</span></span>|<span data-ttu-id="33484-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33484-172">String</span></span>|<span data-ttu-id="33484-173">Der Dateiname in der Benutzeroberfläche angezeigt.</span><span class="sxs-lookup"><span data-stu-id="33484-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="33484-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="33484-174">Response</span></span>
<span data-ttu-id="33484-175">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="33484-175">If successful, this method returns a `201 Created` response code and a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33484-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33484-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="33484-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33484-177">Request</span></span>
<span data-ttu-id="33484-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33484-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="33484-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="33484-179">Response</span></span>
<span data-ttu-id="33484-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33484-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
  "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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




