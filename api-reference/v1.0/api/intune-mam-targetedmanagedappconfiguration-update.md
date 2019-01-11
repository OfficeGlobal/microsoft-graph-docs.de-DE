---
title: targetedManagedAppConfiguration aktualisieren
description: Aktualisieren der Eigenschaften eines targetedManagedAppConfiguration- Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8ee8ff72cbeda93922b47c5a8de2872ef282b26e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805600"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="301bc-103">targetedManagedAppConfiguration aktualisieren</span><span class="sxs-lookup"><span data-stu-id="301bc-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="301bc-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="301bc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="301bc-105">Aktualisieren der Eigenschaften eines [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)- Objekts.</span><span class="sxs-lookup"><span data-stu-id="301bc-105">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="301bc-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="301bc-106">Prerequisites</span></span>
<span data-ttu-id="301bc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="301bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="301bc-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="301bc-109">Permission type</span></span>|<span data-ttu-id="301bc-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="301bc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="301bc-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="301bc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="301bc-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="301bc-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="301bc-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="301bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="301bc-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="301bc-114">Not supported.</span></span>|
|<span data-ttu-id="301bc-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="301bc-115">Application</span></span>|<span data-ttu-id="301bc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="301bc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="301bc-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="301bc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="301bc-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="301bc-118">Request headers</span></span>
|<span data-ttu-id="301bc-119">Header</span><span class="sxs-lookup"><span data-stu-id="301bc-119">Header</span></span>|<span data-ttu-id="301bc-120">Wert</span><span class="sxs-lookup"><span data-stu-id="301bc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="301bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="301bc-121">Authorization</span></span>|<span data-ttu-id="301bc-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="301bc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="301bc-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="301bc-123">Accept</span></span>|<span data-ttu-id="301bc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="301bc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="301bc-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="301bc-125">Request body</span></span>
<span data-ttu-id="301bc-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="301bc-126">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="301bc-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="301bc-127">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="301bc-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="301bc-128">Property</span></span>|<span data-ttu-id="301bc-129">Typ</span><span class="sxs-lookup"><span data-stu-id="301bc-129">Type</span></span>|<span data-ttu-id="301bc-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="301bc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="301bc-131">displayName</span><span class="sxs-lookup"><span data-stu-id="301bc-131">displayName</span></span>|<span data-ttu-id="301bc-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="301bc-132">String</span></span>|<span data-ttu-id="301bc-133">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="301bc-133">Policy display name.</span></span> <span data-ttu-id="301bc-134">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="301bc-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="301bc-135">description</span><span class="sxs-lookup"><span data-stu-id="301bc-135">description</span></span>|<span data-ttu-id="301bc-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="301bc-136">String</span></span>|<span data-ttu-id="301bc-137">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="301bc-137">The policy's description.</span></span> <span data-ttu-id="301bc-138">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="301bc-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="301bc-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="301bc-139">createdDateTime</span></span>|<span data-ttu-id="301bc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="301bc-140">DateTimeOffset</span></span>|<span data-ttu-id="301bc-141">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="301bc-141">The date and time the policy was created.</span></span> <span data-ttu-id="301bc-142">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="301bc-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="301bc-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="301bc-143">lastModifiedDateTime</span></span>|<span data-ttu-id="301bc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="301bc-144">DateTimeOffset</span></span>|<span data-ttu-id="301bc-145">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="301bc-145">Last time the policy was modified.</span></span> <span data-ttu-id="301bc-146">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="301bc-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="301bc-147">id</span><span class="sxs-lookup"><span data-stu-id="301bc-147">id</span></span>|<span data-ttu-id="301bc-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="301bc-148">String</span></span>|<span data-ttu-id="301bc-149">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="301bc-149">Key of the entity.</span></span> <span data-ttu-id="301bc-150">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="301bc-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="301bc-151">Version</span><span class="sxs-lookup"><span data-stu-id="301bc-151">version</span></span>|<span data-ttu-id="301bc-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="301bc-152">String</span></span>|<span data-ttu-id="301bc-153">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="301bc-153">Version of the entity.</span></span> <span data-ttu-id="301bc-154">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="301bc-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="301bc-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="301bc-155">customSettings</span></span>|<span data-ttu-id="301bc-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="301bc-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="301bc-157">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="301bc-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="301bc-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="301bc-158">deployedAppCount</span></span>|<span data-ttu-id="301bc-159">Int32</span><span class="sxs-lookup"><span data-stu-id="301bc-159">Int32</span></span>|<span data-ttu-id="301bc-160">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="301bc-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="301bc-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="301bc-161">isAssigned</span></span>|<span data-ttu-id="301bc-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="301bc-162">Boolean</span></span>|<span data-ttu-id="301bc-163">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="301bc-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="301bc-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="301bc-164">Response</span></span>
<span data-ttu-id="301bc-165">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="301bc-165">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="301bc-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="301bc-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="301bc-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="301bc-167">Request</span></span>
<span data-ttu-id="301bc-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="301bc-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="301bc-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="301bc-169">Response</span></span>
<span data-ttu-id="301bc-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="301bc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



