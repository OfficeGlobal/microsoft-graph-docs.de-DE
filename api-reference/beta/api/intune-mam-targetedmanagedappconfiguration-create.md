---
title: targetedManagedAppConfiguration erstellen
description: Erstellen eines neuen targetedManagedAppConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2849e545fd34c616ea9b7c4962607fa1b94fdea6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394418"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="10d3f-103">targetedManagedAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="10d3f-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="10d3f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="10d3f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="10d3f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10d3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10d3f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10d3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10d3f-107">Erstellen eines neuen [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="10d3f-107">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10d3f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="10d3f-108">Prerequisites</span></span>
<span data-ttu-id="10d3f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="10d3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="10d3f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10d3f-111">Permission type</span></span>|<span data-ttu-id="10d3f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10d3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10d3f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10d3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10d3f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10d3f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="10d3f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10d3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10d3f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10d3f-116">Not supported.</span></span>|
|<span data-ttu-id="10d3f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10d3f-117">Application</span></span>|<span data-ttu-id="10d3f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10d3f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10d3f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10d3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="10d3f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10d3f-120">Request headers</span></span>
|<span data-ttu-id="10d3f-121">Header</span><span class="sxs-lookup"><span data-stu-id="10d3f-121">Header</span></span>|<span data-ttu-id="10d3f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="10d3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10d3f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="10d3f-123">Authorization</span></span>|<span data-ttu-id="10d3f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="10d3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10d3f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="10d3f-125">Accept</span></span>|<span data-ttu-id="10d3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10d3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10d3f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10d3f-127">Request body</span></span>
<span data-ttu-id="10d3f-128">Geben Sie im Anforderungstext eine JSON-Darstellung des targetedManagedAppConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="10d3f-128">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="10d3f-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs targetedManagedAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="10d3f-129">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="10d3f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10d3f-130">Property</span></span>|<span data-ttu-id="10d3f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="10d3f-131">Type</span></span>|<span data-ttu-id="10d3f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10d3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10d3f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="10d3f-133">displayName</span></span>|<span data-ttu-id="10d3f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10d3f-134">String</span></span>|<span data-ttu-id="10d3f-135">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="10d3f-135">Policy display name.</span></span> <span data-ttu-id="10d3f-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="10d3f-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="10d3f-137">description</span><span class="sxs-lookup"><span data-stu-id="10d3f-137">description</span></span>|<span data-ttu-id="10d3f-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10d3f-138">String</span></span>|<span data-ttu-id="10d3f-139">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="10d3f-139">The policy's description.</span></span> <span data-ttu-id="10d3f-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="10d3f-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="10d3f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10d3f-141">createdDateTime</span></span>|<span data-ttu-id="10d3f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10d3f-142">DateTimeOffset</span></span>|<span data-ttu-id="10d3f-143">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="10d3f-143">The date and time the policy was created.</span></span> <span data-ttu-id="10d3f-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="10d3f-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="10d3f-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10d3f-145">lastModifiedDateTime</span></span>|<span data-ttu-id="10d3f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10d3f-146">DateTimeOffset</span></span>|<span data-ttu-id="10d3f-147">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="10d3f-147">Last time the policy was modified.</span></span> <span data-ttu-id="10d3f-148">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="10d3f-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="10d3f-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="10d3f-149">roleScopeTagIds</span></span>|<span data-ttu-id="10d3f-150">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="10d3f-150">String collection</span></span>|<span data-ttu-id="10d3f-151">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="10d3f-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="10d3f-152">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="10d3f-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="10d3f-153">id</span><span class="sxs-lookup"><span data-stu-id="10d3f-153">id</span></span>|<span data-ttu-id="10d3f-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10d3f-154">String</span></span>|<span data-ttu-id="10d3f-155">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="10d3f-155">Key of the entity.</span></span> <span data-ttu-id="10d3f-156">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="10d3f-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="10d3f-157">Version</span><span class="sxs-lookup"><span data-stu-id="10d3f-157">version</span></span>|<span data-ttu-id="10d3f-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10d3f-158">String</span></span>|<span data-ttu-id="10d3f-159">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="10d3f-159">Version of the entity.</span></span> <span data-ttu-id="10d3f-160">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="10d3f-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="10d3f-161">customSettings</span><span class="sxs-lookup"><span data-stu-id="10d3f-161">customSettings</span></span>|<span data-ttu-id="10d3f-162">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="10d3f-162">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="10d3f-163">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10d3f-163">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="10d3f-164">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="10d3f-164">deployedAppCount</span></span>|<span data-ttu-id="10d3f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="10d3f-165">Int32</span></span>|<span data-ttu-id="10d3f-166">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="10d3f-166">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="10d3f-167">isAssigned</span><span class="sxs-lookup"><span data-stu-id="10d3f-167">isAssigned</span></span>|<span data-ttu-id="10d3f-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="10d3f-168">Boolean</span></span>|<span data-ttu-id="10d3f-169">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="10d3f-169">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="10d3f-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="10d3f-170">Response</span></span>
<span data-ttu-id="10d3f-171">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10d3f-171">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10d3f-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10d3f-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="10d3f-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="10d3f-173">Request</span></span>
<span data-ttu-id="10d3f-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="10d3f-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="10d3f-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="10d3f-175">Response</span></span>
<span data-ttu-id="10d3f-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10d3f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```




