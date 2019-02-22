---
title: Aktualisieren von „androidForWorkSettings“
description: Aktualisiert die Eigenschaften eines androidForWorkSettings-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65550bc588eb5fb0f4d2f11ac785d458e8821a7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170791"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="70c5f-103">Aktualisieren von „androidForWorkSettings“</span><span class="sxs-lookup"><span data-stu-id="70c5f-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="70c5f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="70c5f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70c5f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="70c5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70c5f-106">Aktualisiert die Eigenschaften eines [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="70c5f-106">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70c5f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="70c5f-107">Prerequisites</span></span>
<span data-ttu-id="70c5f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="70c5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="70c5f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="70c5f-110">Permission type</span></span>|<span data-ttu-id="70c5f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="70c5f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70c5f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="70c5f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70c5f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70c5f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="70c5f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="70c5f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70c5f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70c5f-115">Not supported.</span></span>|
|<span data-ttu-id="70c5f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="70c5f-116">Application</span></span>|<span data-ttu-id="70c5f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="70c5f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70c5f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="70c5f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="70c5f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="70c5f-119">Request headers</span></span>
|<span data-ttu-id="70c5f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="70c5f-120">Header</span></span>|<span data-ttu-id="70c5f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="70c5f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70c5f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70c5f-122">Authorization</span></span>|<span data-ttu-id="70c5f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="70c5f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70c5f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="70c5f-124">Accept</span></span>|<span data-ttu-id="70c5f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70c5f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70c5f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="70c5f-126">Request body</span></span>
<span data-ttu-id="70c5f-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="70c5f-127">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="70c5f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="70c5f-128">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="70c5f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70c5f-129">Property</span></span>|<span data-ttu-id="70c5f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="70c5f-130">Type</span></span>|<span data-ttu-id="70c5f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="70c5f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70c5f-132">id</span><span class="sxs-lookup"><span data-stu-id="70c5f-132">id</span></span>|<span data-ttu-id="70c5f-133">String</span><span class="sxs-lookup"><span data-stu-id="70c5f-133">String</span></span>|<span data-ttu-id="70c5f-134">Android for Work-Einstellungsbezeichner.</span><span class="sxs-lookup"><span data-stu-id="70c5f-134">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="70c5f-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="70c5f-135">bindStatus</span></span>|[<span data-ttu-id="70c5f-136">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="70c5f-136">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="70c5f-137">Binden des Status des Mandanten mit der Google EMM-API.</span><span class="sxs-lookup"><span data-stu-id="70c5f-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="70c5f-138">Mögliche Werte: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="70c5f-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="70c5f-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="70c5f-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="70c5f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70c5f-140">DateTimeOffset</span></span>|<span data-ttu-id="70c5f-141">Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="70c5f-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="70c5f-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="70c5f-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="70c5f-143">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="70c5f-143">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="70c5f-144">Ergebnis der letzten Anwendungssynchronisierung.</span><span class="sxs-lookup"><span data-stu-id="70c5f-144">Last application sync result.</span></span> <span data-ttu-id="70c5f-145">Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.</span><span class="sxs-lookup"><span data-stu-id="70c5f-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="70c5f-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70c5f-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="70c5f-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70c5f-147">String</span></span>|<span data-ttu-id="70c5f-148">Besitzer-UPN, der das Unternehmen erstellt hat</span><span class="sxs-lookup"><span data-stu-id="70c5f-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="70c5f-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="70c5f-149">ownerOrganizationName</span></span>|<span data-ttu-id="70c5f-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="70c5f-150">String</span></span>|<span data-ttu-id="70c5f-151">Organisationsname, der beim Android for Work-Onboarding verwendet wird</span><span class="sxs-lookup"><span data-stu-id="70c5f-151">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="70c5f-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70c5f-152">lastModifiedDateTime</span></span>|<span data-ttu-id="70c5f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70c5f-153">DateTimeOffset</span></span>|<span data-ttu-id="70c5f-154">Zeitpunkt, zu dem die Android for Work-Einstellungen zuletzt geändert wurden</span><span class="sxs-lookup"><span data-stu-id="70c5f-154">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="70c5f-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="70c5f-155">enrollmentTarget</span></span>|[<span data-ttu-id="70c5f-156">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="70c5f-156">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="70c5f-157">Gibt an, welche Benutzer Geräte in Android für die Arbeitsgeräte Verwaltung registrieren können.</span><span class="sxs-lookup"><span data-stu-id="70c5f-157">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="70c5f-158">Mögliche Werte: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="70c5f-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="70c5f-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="70c5f-159">targetGroupIds</span></span>|<span data-ttu-id="70c5f-160">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="70c5f-160">String collection</span></span>|<span data-ttu-id="70c5f-161">Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.</span><span class="sxs-lookup"><span data-stu-id="70c5f-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="70c5f-162">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="70c5f-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="70c5f-163">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="70c5f-163">Boolean</span></span>|<span data-ttu-id="70c5f-164">Gibt an, ob dieses Konto für die Verwaltung von Android-Geräte Besitzern mit CloudDPC läuft.</span><span class="sxs-lookup"><span data-stu-id="70c5f-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="70c5f-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="70c5f-165">Response</span></span>
<span data-ttu-id="70c5f-166">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="70c5f-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70c5f-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="70c5f-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="70c5f-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="70c5f-168">Request</span></span>
<span data-ttu-id="70c5f-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="70c5f-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="70c5f-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="70c5f-170">Response</span></span>
<span data-ttu-id="70c5f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="70c5f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```




