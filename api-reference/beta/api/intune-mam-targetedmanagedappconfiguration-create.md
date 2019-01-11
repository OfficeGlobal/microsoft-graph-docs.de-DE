---
title: targetedManagedAppConfiguration erstellen
description: Erstellen eines neuen targetedManagedAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a196dee202ce55b6f342ade8f3b7d0d3ec9aea8c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857379"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="5c74e-103">targetedManagedAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="5c74e-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="5c74e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5c74e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c74e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5c74e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c74e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5c74e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c74e-107">Erstellen eines neuen [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c74e-107">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c74e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5c74e-108">Prerequisites</span></span>
<span data-ttu-id="5c74e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c74e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c74e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c74e-111">Permission type</span></span>|<span data-ttu-id="5c74e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c74e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c74e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c74e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c74e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c74e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c74e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c74e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c74e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c74e-116">Not supported.</span></span>|
|<span data-ttu-id="5c74e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c74e-117">Application</span></span>|<span data-ttu-id="5c74e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c74e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c74e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c74e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5c74e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c74e-120">Request headers</span></span>
|<span data-ttu-id="5c74e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5c74e-121">Header</span></span>|<span data-ttu-id="5c74e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5c74e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c74e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c74e-123">Authorization</span></span>|<span data-ttu-id="5c74e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5c74e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c74e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5c74e-125">Accept</span></span>|<span data-ttu-id="5c74e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c74e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c74e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c74e-127">Request body</span></span>
<span data-ttu-id="5c74e-128">Geben Sie im Anforderungstext eine JSON-Darstellung des targetedManagedAppConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5c74e-128">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="5c74e-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs targetedManagedAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="5c74e-129">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="5c74e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c74e-130">Property</span></span>|<span data-ttu-id="5c74e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5c74e-131">Type</span></span>|<span data-ttu-id="5c74e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c74e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c74e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5c74e-133">displayName</span></span>|<span data-ttu-id="5c74e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c74e-134">String</span></span>|<span data-ttu-id="5c74e-135">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="5c74e-135">Policy display name.</span></span> <span data-ttu-id="5c74e-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c74e-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c74e-137">description</span><span class="sxs-lookup"><span data-stu-id="5c74e-137">description</span></span>|<span data-ttu-id="5c74e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c74e-138">String</span></span>|<span data-ttu-id="5c74e-139">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="5c74e-139">The policy's description.</span></span> <span data-ttu-id="5c74e-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c74e-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c74e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c74e-141">createdDateTime</span></span>|<span data-ttu-id="5c74e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c74e-142">DateTimeOffset</span></span>|<span data-ttu-id="5c74e-143">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="5c74e-143">The date and time the policy was created.</span></span> <span data-ttu-id="5c74e-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c74e-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c74e-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c74e-145">lastModifiedDateTime</span></span>|<span data-ttu-id="5c74e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c74e-146">DateTimeOffset</span></span>|<span data-ttu-id="5c74e-147">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="5c74e-147">Last time the policy was modified.</span></span> <span data-ttu-id="5c74e-148">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c74e-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c74e-149">id</span><span class="sxs-lookup"><span data-stu-id="5c74e-149">id</span></span>|<span data-ttu-id="5c74e-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c74e-150">String</span></span>|<span data-ttu-id="5c74e-151">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5c74e-151">Key of the entity.</span></span> <span data-ttu-id="5c74e-152">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c74e-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c74e-153">Version</span><span class="sxs-lookup"><span data-stu-id="5c74e-153">version</span></span>|<span data-ttu-id="5c74e-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c74e-154">String</span></span>|<span data-ttu-id="5c74e-155">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="5c74e-155">Version of the entity.</span></span> <span data-ttu-id="5c74e-156">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c74e-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="5c74e-157">customSettings</span><span class="sxs-lookup"><span data-stu-id="5c74e-157">customSettings</span></span>|<span data-ttu-id="5c74e-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5c74e-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5c74e-159">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c74e-159">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="5c74e-160">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="5c74e-160">deployedAppCount</span></span>|<span data-ttu-id="5c74e-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5c74e-161">Int32</span></span>|<span data-ttu-id="5c74e-162">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="5c74e-162">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="5c74e-163">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5c74e-163">isAssigned</span></span>|<span data-ttu-id="5c74e-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5c74e-164">Boolean</span></span>|<span data-ttu-id="5c74e-165">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="5c74e-165">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="5c74e-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c74e-166">Response</span></span>
<span data-ttu-id="5c74e-167">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c74e-167">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c74e-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c74e-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c74e-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c74e-169">Request</span></span>
<span data-ttu-id="5c74e-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c74e-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="5c74e-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c74e-171">Response</span></span>
<span data-ttu-id="5c74e-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c74e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





