---
title: Aktualisieren von „deviceAppManagement“
description: Aktualisiert die Eigenschaften von Objekten des Typs deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f100e91f6943d24dd63be9c28ba0e96213cfc012
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991496"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="1df57-103">Aktualisieren von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="1df57-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="1df57-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1df57-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1df57-105">Aktualisiert die Eigenschaften von Objekten des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="1df57-105">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1df57-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1df57-106">Prerequisites</span></span>
<span data-ttu-id="1df57-107">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="1df57-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1df57-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1df57-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="1df57-109">Beachten Sie, dass die entsprechende Berechtigungen gemäß den Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="1df57-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="1df57-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1df57-110">Permission type</span></span>|<span data-ttu-id="1df57-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1df57-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1df57-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1df57-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1df57-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1df57-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1df57-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1df57-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1df57-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1df57-115">Not supported.</span></span>|
|<span data-ttu-id="1df57-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1df57-116">Application</span></span>|<span data-ttu-id="1df57-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1df57-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1df57-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1df57-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="1df57-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1df57-119">Request headers</span></span>
|<span data-ttu-id="1df57-120">Header</span><span class="sxs-lookup"><span data-stu-id="1df57-120">Header</span></span>|<span data-ttu-id="1df57-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1df57-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1df57-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1df57-122">Authorization</span></span>|<span data-ttu-id="1df57-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1df57-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1df57-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1df57-124">Accept</span></span>|<span data-ttu-id="1df57-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1df57-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1df57-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1df57-126">Request body</span></span>
<span data-ttu-id="1df57-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="1df57-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="1df57-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1df57-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="1df57-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1df57-129">Property</span></span>|<span data-ttu-id="1df57-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1df57-130">Type</span></span>|<span data-ttu-id="1df57-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1df57-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1df57-132">id</span><span class="sxs-lookup"><span data-stu-id="1df57-132">id</span></span>|<span data-ttu-id="1df57-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1df57-133">String</span></span>|<span data-ttu-id="1df57-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1df57-134">Key of the entity.</span></span>|
|<span data-ttu-id="1df57-135">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="1df57-135">**Onboarding**</span></span>|
|<span data-ttu-id="1df57-136">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="1df57-136">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="1df57-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1df57-137">Boolean</span></span>|<span data-ttu-id="1df57-138">Gibt an, ob das Konto Anwendungen mit dem Microsoft Store für Unternehmen synchronisieren darf.</span><span class="sxs-lookup"><span data-stu-id="1df57-138">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="1df57-139">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="1df57-139">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="1df57-140">String</span><span class="sxs-lookup"><span data-stu-id="1df57-140">String</span></span>|<span data-ttu-id="1df57-141">Die Gebietsschemainformationen, die zur Synchronisierung von Anwendungen mit dem Microsoft Store für Unternehmen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="1df57-141">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="1df57-142">Angegeben werden Kulturen, die für ein Land bzw. eine Region spezifisch sind.</span><span class="sxs-lookup"><span data-stu-id="1df57-142">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="1df57-143">Die Namen dieser Kulturen folgen dem Standard RFC 4646 (Windows Vista und höher).</span><span class="sxs-lookup"><span data-stu-id="1df57-143">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="1df57-144">Das Format lautet <languagecode2>-<country/regioncode2>. Dabei ist <languagecode2> ein klein geschriebener Code aus zwei Buchstaben nach ISO 639-1 und <country/regioncode2> ein groß geschriebener Code aus zwei Buchstaben nach ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="1df57-144">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="1df57-145">Beispiel für eine spezifische Kultur: „en-US“ für „Englisch (Vereinigte Staaten)“.</span><span class="sxs-lookup"><span data-stu-id="1df57-145">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="1df57-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="1df57-146">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="1df57-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1df57-147">DateTimeOffset</span></span>|<span data-ttu-id="1df57-148">Zeitpunkt der letzten Anwendungssynchronisierung mit dem Microsoft Store für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="1df57-148">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="1df57-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1df57-149">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="1df57-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1df57-150">DateTimeOffset</span></span>|<span data-ttu-id="1df57-151">Zeitpunkt, zu dem das Konto die Apps letztmals erfolgreich mit dem Microsoft Store für Unternehmen synchronisiert hat</span><span class="sxs-lookup"><span data-stu-id="1df57-151">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="1df57-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="1df57-152">Response</span></span>
<span data-ttu-id="1df57-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1df57-153">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="1df57-154">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="1df57-154">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="1df57-155">Beispielantwort</span><span class="sxs-lookup"><span data-stu-id="1df57-155">Example response</span></span>

<span data-ttu-id="1df57-156">Der Kürze halber werden möglicherweise im Response-Objekt dargestellten abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="1df57-156">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1df57-157">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1df57-157">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



