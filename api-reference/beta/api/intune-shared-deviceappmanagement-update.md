---
title: Aktualisieren von „deviceAppManagement“
description: Aktualisiert die Eigenschaften von Objekten des Typs deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0a70c1544ac862b5bbe11f0883d9d2c274a1ad27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920310"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="93f29-103">Aktualisieren von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="93f29-103">Update deviceAppManagement</span></span>

> <span data-ttu-id="93f29-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="93f29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93f29-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93f29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93f29-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="93f29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93f29-107">Aktualisiert die Eigenschaften von Objekten des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="93f29-107">Update the properties of a [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93f29-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="93f29-108">Prerequisites</span></span>
<span data-ttu-id="93f29-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="93f29-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="93f29-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f29-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="93f29-111">Beachten Sie, dass die entsprechende Berechtigungen gemäß den Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="93f29-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="93f29-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93f29-112">Permission type</span></span>|<span data-ttu-id="93f29-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93f29-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="93f29-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93f29-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="93f29-115">&nbsp;&nbsp; **Apps**, **Bücher**oder **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="93f29-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="93f29-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93f29-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="93f29-117">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="93f29-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="93f29-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93f29-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="93f29-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93f29-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93f29-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93f29-120">Not supported.</span></span> |
| <span data-ttu-id="93f29-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93f29-121">Application</span></span> | <span data-ttu-id="93f29-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93f29-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="93f29-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93f29-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="93f29-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93f29-124">Request headers</span></span>
|<span data-ttu-id="93f29-125">Header</span><span class="sxs-lookup"><span data-stu-id="93f29-125">Header</span></span>|<span data-ttu-id="93f29-126">Wert</span><span class="sxs-lookup"><span data-stu-id="93f29-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93f29-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="93f29-127">Authorization</span></span>|<span data-ttu-id="93f29-128">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="93f29-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93f29-129">Annehmen</span><span class="sxs-lookup"><span data-stu-id="93f29-129">Accept</span></span>|<span data-ttu-id="93f29-130">application/json</span><span class="sxs-lookup"><span data-stu-id="93f29-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93f29-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93f29-131">Request body</span></span>
<span data-ttu-id="93f29-132">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) an.</span><span class="sxs-lookup"><span data-stu-id="93f29-132">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="93f29-133">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="93f29-133">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span></span>

|<span data-ttu-id="93f29-134">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93f29-134">Property</span></span>|<span data-ttu-id="93f29-135">Typ</span><span class="sxs-lookup"><span data-stu-id="93f29-135">Type</span></span>|<span data-ttu-id="93f29-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93f29-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93f29-137">id</span><span class="sxs-lookup"><span data-stu-id="93f29-137">id</span></span>|<span data-ttu-id="93f29-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93f29-138">String</span></span>|<span data-ttu-id="93f29-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="93f29-139">Key of the entity.</span></span>|
|<span data-ttu-id="93f29-140">**Klicken Sie auf mittels Fingereingabe**</span><span class="sxs-lookup"><span data-stu-id="93f29-140">**On-boarding**</span></span>|
|<span data-ttu-id="93f29-141">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="93f29-141">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="93f29-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="93f29-142">Boolean</span></span>|<span data-ttu-id="93f29-143">Gibt an, ob das Konto Anwendungen mit dem Microsoft Store für Unternehmen synchronisieren darf.</span><span class="sxs-lookup"><span data-stu-id="93f29-143">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="93f29-144">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="93f29-144">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="93f29-145">String</span><span class="sxs-lookup"><span data-stu-id="93f29-145">String</span></span>|<span data-ttu-id="93f29-146">Die Gebietsschemainformationen, die zur Synchronisierung von Anwendungen mit dem Microsoft Store für Unternehmen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="93f29-146">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="93f29-147">Angegeben werden Kulturen, die für ein Land bzw. eine Region spezifisch sind.</span><span class="sxs-lookup"><span data-stu-id="93f29-147">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="93f29-148">Die Namen dieser Kulturen folgen dem Standard RFC 4646 (Windows Vista und höher).</span><span class="sxs-lookup"><span data-stu-id="93f29-148">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="93f29-149">Das Format lautet <languagecode2>-<country/regioncode2>. Dabei ist <languagecode2> ein klein geschriebener Code aus zwei Buchstaben nach ISO 639-1 und <country/regioncode2> ein groß geschriebener Code aus zwei Buchstaben nach ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="93f29-149">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="93f29-150">Beispiel für eine spezifische Kultur: „en-US“ für „Englisch (Vereinigte Staaten)“.</span><span class="sxs-lookup"><span data-stu-id="93f29-150">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="93f29-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="93f29-151">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="93f29-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93f29-152">DateTimeOffset</span></span>|<span data-ttu-id="93f29-153">Zeitpunkt der letzten Anwendungssynchronisierung mit dem Microsoft Store für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="93f29-153">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="93f29-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="93f29-154">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="93f29-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93f29-155">DateTimeOffset</span></span>|<span data-ttu-id="93f29-156">Zeitpunkt, zu dem das Konto die Apps letztmals erfolgreich mit dem Microsoft Store für Unternehmen synchronisiert hat</span><span class="sxs-lookup"><span data-stu-id="93f29-156">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="93f29-157">microsoftStoreForBusinessPortalSelection</span><span class="sxs-lookup"><span data-stu-id="93f29-157">microsoftStoreForBusinessPortalSelection</span></span>|[<span data-ttu-id="93f29-158">microsoftStoreForBusinessPortalSelectionOptions</span><span class="sxs-lookup"><span data-stu-id="93f29-158">microsoftStoreForBusinessPortalSelectionOptions</span></span>](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|<span data-ttu-id="93f29-159">Die Endbenutzer Portal-Informationen werden verwendet, aus dem Microsoft Store for Business Applications, Intune Unternehmen Portal synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="93f29-159">The end user portal information is used to sync applications from the Microsoft Store for Business to Intune Company Portal.</span></span> <span data-ttu-id="93f29-160">Es gibt drei Optionen zur Auswahl \['Des Unternehmens nur Portal', 'Unternehmen Portal und privaten speichern', 'Privaten Speicher'\].</span><span class="sxs-lookup"><span data-stu-id="93f29-160">There are three options to pick from \['Company portal only', 'Company portal and private store', 'Private store only'\].</span></span> <span data-ttu-id="93f29-161">Mögliche Werte sind: `none`, `companyPortal` und `privateStore`.</span><span class="sxs-lookup"><span data-stu-id="93f29-161">Possible values are: `none`, `companyPortal`, `privateStore`.</span></span>|

<span data-ttu-id="93f29-162">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93f29-162">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="93f29-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="93f29-163">Response</span></span>
<span data-ttu-id="93f29-164">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="93f29-164">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93f29-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93f29-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="93f29-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93f29-166">Request</span></span>

<span data-ttu-id="93f29-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93f29-167">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="93f29-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="93f29-168">Response</span></span>

<span data-ttu-id="93f29-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93f29-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



