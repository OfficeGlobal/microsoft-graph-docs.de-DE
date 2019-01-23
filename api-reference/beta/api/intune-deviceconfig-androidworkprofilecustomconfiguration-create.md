---
title: Erstellen von androidWorkProfileCustomConfiguration
description: Erstellen eines neuen AndroidWorkProfileCustomConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ad206d600880d72c77f257669a03efa72a2acb5d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417931"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="4b8ba-103">Erstellen von androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b8ba-103">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="4b8ba-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b8ba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b8ba-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b8ba-107">Erstellen eines neuen [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-107">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b8ba-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4b8ba-108">Prerequisites</span></span>
<span data-ttu-id="4b8ba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4b8ba-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b8ba-111">Permission type</span></span>|<span data-ttu-id="4b8ba-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b8ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b8ba-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b8ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b8ba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b8ba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b8ba-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b8ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b8ba-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b8ba-116">Not supported.</span></span>|
|<span data-ttu-id="4b8ba-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b8ba-117">Application</span></span>|<span data-ttu-id="4b8ba-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b8ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b8ba-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b8ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4b8ba-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b8ba-120">Request headers</span></span>
|<span data-ttu-id="4b8ba-121">Header</span><span class="sxs-lookup"><span data-stu-id="4b8ba-121">Header</span></span>|<span data-ttu-id="4b8ba-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4b8ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b8ba-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4b8ba-123">Authorization</span></span>|<span data-ttu-id="4b8ba-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4b8ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b8ba-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4b8ba-125">Accept</span></span>|<span data-ttu-id="4b8ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b8ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b8ba-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b8ba-127">Request body</span></span>
<span data-ttu-id="4b8ba-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidWorkProfileCustomConfiguration eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-128">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="4b8ba-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidWorkProfileCustomConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-129">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="4b8ba-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b8ba-130">Property</span></span>|<span data-ttu-id="4b8ba-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4b8ba-131">Type</span></span>|<span data-ttu-id="4b8ba-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b8ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b8ba-133">id</span><span class="sxs-lookup"><span data-stu-id="4b8ba-133">id</span></span>|<span data-ttu-id="4b8ba-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b8ba-134">String</span></span>|<span data-ttu-id="4b8ba-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4b8ba-135">Key of the entity.</span></span> <span data-ttu-id="4b8ba-136">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b8ba-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b8ba-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4b8ba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b8ba-138">DateTimeOffset</span></span>|<span data-ttu-id="4b8ba-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4b8ba-140">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b8ba-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b8ba-141">roleScopeTagIds</span></span>|<span data-ttu-id="4b8ba-142">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4b8ba-142">String collection</span></span>|<span data-ttu-id="4b8ba-143">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4b8ba-144">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b8ba-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4b8ba-145">supportsScopeTags</span></span>|<span data-ttu-id="4b8ba-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b8ba-146">Boolean</span></span>|<span data-ttu-id="4b8ba-147">Gibt an, ob die zugrunde liegende Gerätekonfiguration die Zuweisung von Bereich Kategorien unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4b8ba-148">Zuweisen der ScopeTags-Eigenschaft ist nicht zulässig, wenn dieser Wert false ist und Entitäten nicht bereichsbezogenen Benutzern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4b8ba-149">Dies tritt für Legacy-Richtlinien in Silverlight erstellt und kann durch Löschen und Neuerstellen der Richtlinie in der Azure-Verwaltungsportal aufgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4b8ba-150">Diese Eigenschaft ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-150">This property is read-only.</span></span> <span data-ttu-id="4b8ba-151">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b8ba-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b8ba-152">createdDateTime</span></span>|<span data-ttu-id="4b8ba-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b8ba-153">DateTimeOffset</span></span>|<span data-ttu-id="4b8ba-154">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-154">DateTime the object was created.</span></span> <span data-ttu-id="4b8ba-155">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b8ba-156">description</span><span class="sxs-lookup"><span data-stu-id="4b8ba-156">description</span></span>|<span data-ttu-id="4b8ba-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b8ba-157">String</span></span>|<span data-ttu-id="4b8ba-158">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b8ba-159">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b8ba-160">displayName</span><span class="sxs-lookup"><span data-stu-id="4b8ba-160">displayName</span></span>|<span data-ttu-id="4b8ba-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b8ba-161">String</span></span>|<span data-ttu-id="4b8ba-162">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b8ba-163">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b8ba-164">Version</span><span class="sxs-lookup"><span data-stu-id="4b8ba-164">version</span></span>|<span data-ttu-id="4b8ba-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4b8ba-165">Int32</span></span>|<span data-ttu-id="4b8ba-166">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-166">Version of the device configuration.</span></span> <span data-ttu-id="4b8ba-167">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b8ba-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b8ba-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="4b8ba-168">omaSettings</span></span>|<span data-ttu-id="4b8ba-169">Collection von Objekten des Typs [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b8ba-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="4b8ba-170">OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-170">OMA settings.</span></span> <span data-ttu-id="4b8ba-171">Diese Collection darf maximal 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4b8ba-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b8ba-172">Response</span></span>
<span data-ttu-id="4b8ba-173">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-173">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b8ba-174">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b8ba-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b8ba-175">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b8ba-175">Request</span></span>
<span data-ttu-id="4b8ba-176">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 505

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4b8ba-177">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b8ba-177">Response</span></span>
<span data-ttu-id="4b8ba-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b8ba-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 677

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




