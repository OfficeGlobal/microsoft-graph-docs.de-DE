---
title: AndroidForWorkTrustedRootCertificate erstellen
description: Erstellen eines neuen androidForWorkTrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0be3334f34cc60ac945970222fbe6eead98b8a7a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975581"
---
# <a name="create-androidforworktrustedrootcertificate"></a><span data-ttu-id="0a5a9-103">AndroidForWorkTrustedRootCertificate erstellen</span><span class="sxs-lookup"><span data-stu-id="0a5a9-103">Create androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="0a5a9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a5a9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a5a9-106">Erstellen eines neuen [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-106">Create a new [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a5a9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0a5a9-107">Prerequisites</span></span>
<span data-ttu-id="0a5a9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a5a9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a5a9-110">Permission type</span></span>|<span data-ttu-id="0a5a9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a5a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a5a9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a5a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a5a9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a5a9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a5a9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a5a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a5a9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a5a9-115">Not supported.</span></span>|
|<span data-ttu-id="0a5a9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a5a9-116">Application</span></span>|<span data-ttu-id="0a5a9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a5a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a5a9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a5a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0a5a9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a5a9-119">Request headers</span></span>
|<span data-ttu-id="0a5a9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0a5a9-120">Header</span></span>|<span data-ttu-id="0a5a9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0a5a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a5a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a5a9-122">Authorization</span></span>|<span data-ttu-id="0a5a9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0a5a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a5a9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0a5a9-124">Accept</span></span>|<span data-ttu-id="0a5a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a5a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a5a9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a5a9-126">Request body</span></span>
<span data-ttu-id="0a5a9-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das androidForWorkTrustedRootCertificate-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-127">In the request body, supply a JSON representation for the androidForWorkTrustedRootCertificate object.</span></span>

<span data-ttu-id="0a5a9-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der androidForWorkTrustedRootCertificate erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-128">The following table shows the properties that are required when you create the androidForWorkTrustedRootCertificate.</span></span>

|<span data-ttu-id="0a5a9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a5a9-129">Property</span></span>|<span data-ttu-id="0a5a9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0a5a9-130">Type</span></span>|<span data-ttu-id="0a5a9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a5a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a5a9-132">id</span><span class="sxs-lookup"><span data-stu-id="0a5a9-132">id</span></span>|<span data-ttu-id="0a5a9-133">String</span><span class="sxs-lookup"><span data-stu-id="0a5a9-133">String</span></span>|<span data-ttu-id="0a5a9-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0a5a9-134">Key of the entity.</span></span> <span data-ttu-id="0a5a9-135">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a5a9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a5a9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0a5a9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a5a9-137">DateTimeOffset</span></span>|<span data-ttu-id="0a5a9-138">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0a5a9-139">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a5a9-140">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="0a5a9-140">roleScopeTagIds</span></span>|<span data-ttu-id="0a5a9-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0a5a9-141">String collection</span></span>|<span data-ttu-id="0a5a9-142">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0a5a9-143">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a5a9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0a5a9-144">supportsScopeTags</span></span>|<span data-ttu-id="0a5a9-145">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0a5a9-145">Boolean</span></span>|<span data-ttu-id="0a5a9-146">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereichs Tags unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0a5a9-147">Das Zuweisen zur ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert auf false festgelegt ist und Entitäten für bereichsbezogene Benutzer nicht sichtbar sind.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0a5a9-148">Dies geschieht für in Silverlight erstellte Legacy Richtlinien und kann durch Löschen und erneutes Erstellen der Richtlinie im Azure-Portal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0a5a9-149">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-149">This property is read-only.</span></span> <span data-ttu-id="0a5a9-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a5a9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a5a9-151">createdDateTime</span></span>|<span data-ttu-id="0a5a9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a5a9-152">DateTimeOffset</span></span>|<span data-ttu-id="0a5a9-153">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-153">DateTime the object was created.</span></span> <span data-ttu-id="0a5a9-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a5a9-155">description</span><span class="sxs-lookup"><span data-stu-id="0a5a9-155">description</span></span>|<span data-ttu-id="0a5a9-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0a5a9-156">String</span></span>|<span data-ttu-id="0a5a9-157">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0a5a9-158">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a5a9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0a5a9-159">displayName</span></span>|<span data-ttu-id="0a5a9-160">String</span><span class="sxs-lookup"><span data-stu-id="0a5a9-160">String</span></span>|<span data-ttu-id="0a5a9-161">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0a5a9-162">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a5a9-163">Version</span><span class="sxs-lookup"><span data-stu-id="0a5a9-163">version</span></span>|<span data-ttu-id="0a5a9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0a5a9-164">Int32</span></span>|<span data-ttu-id="0a5a9-165">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-165">Version of the device configuration.</span></span> <span data-ttu-id="0a5a9-166">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0a5a9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0a5a9-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0a5a9-167">trustedRootCertificate</span></span>|<span data-ttu-id="0a5a9-168">Binär</span><span class="sxs-lookup"><span data-stu-id="0a5a9-168">Binary</span></span>|<span data-ttu-id="0a5a9-169">Vertrauenswürdiges Stammzertifikat</span><span class="sxs-lookup"><span data-stu-id="0a5a9-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="0a5a9-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="0a5a9-170">certFileName</span></span>|<span data-ttu-id="0a5a9-171">String</span><span class="sxs-lookup"><span data-stu-id="0a5a9-171">String</span></span>|<span data-ttu-id="0a5a9-172">Dateiname, der in der Benutzeroberfläche angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-172">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="0a5a9-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a5a9-173">Response</span></span>
<span data-ttu-id="0a5a9-174">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-174">If successful, this method returns a `201 Created` response code and a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a5a9-175">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a5a9-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a5a9-176">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a5a9-176">Request</span></span>
<span data-ttu-id="0a5a9-177">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a5a9-178">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a5a9-178">Response</span></span>
<span data-ttu-id="0a5a9-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a5a9-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




