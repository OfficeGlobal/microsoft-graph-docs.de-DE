---
title: Aktualisieren von „userInstallStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs userInstallStateSummary.
ms.openlocfilehash: b161cac0cc2d3ee0fd31662318ef2bb94232dc63
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064514"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="04bd1-103">Aktualisieren von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="04bd1-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="04bd1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="04bd1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04bd1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04bd1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04bd1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="04bd1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04bd1-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="04bd1-107">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04bd1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="04bd1-108">Prerequisites</span></span>
<span data-ttu-id="04bd1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04bd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04bd1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04bd1-111">Permission type</span></span>|<span data-ttu-id="04bd1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04bd1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04bd1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04bd1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04bd1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04bd1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04bd1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04bd1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04bd1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04bd1-116">Not supported.</span></span>|
|<span data-ttu-id="04bd1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04bd1-117">Application</span></span>|<span data-ttu-id="04bd1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04bd1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04bd1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04bd1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="04bd1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04bd1-120">Request headers</span></span>
|<span data-ttu-id="04bd1-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="04bd1-121">Header</span></span>|<span data-ttu-id="04bd1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="04bd1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04bd1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04bd1-123">Authorization</span></span>|<span data-ttu-id="04bd1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="04bd1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04bd1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04bd1-125">Accept</span></span>|<span data-ttu-id="04bd1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04bd1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04bd1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04bd1-127">Request body</span></span>
<span data-ttu-id="04bd1-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="04bd1-128">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="04bd1-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="04bd1-129">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="04bd1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04bd1-130">Property</span></span>|<span data-ttu-id="04bd1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="04bd1-131">Type</span></span>|<span data-ttu-id="04bd1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04bd1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04bd1-133">id</span><span class="sxs-lookup"><span data-stu-id="04bd1-133">id</span></span>|<span data-ttu-id="04bd1-134">String</span><span class="sxs-lookup"><span data-stu-id="04bd1-134">String</span></span>|<span data-ttu-id="04bd1-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="04bd1-135">Key of the entity.</span></span>|
|<span data-ttu-id="04bd1-136">userName</span><span class="sxs-lookup"><span data-stu-id="04bd1-136">userName</span></span>|<span data-ttu-id="04bd1-137">String</span><span class="sxs-lookup"><span data-stu-id="04bd1-137">String</span></span>|<span data-ttu-id="04bd1-138">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="04bd1-138">User name.</span></span>|
|<span data-ttu-id="04bd1-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="04bd1-139">installedDeviceCount</span></span>|<span data-ttu-id="04bd1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="04bd1-140">Int32</span></span>|<span data-ttu-id="04bd1-141">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="04bd1-141">Installed Device Count.</span></span>|
|<span data-ttu-id="04bd1-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="04bd1-142">failedDeviceCount</span></span>|<span data-ttu-id="04bd1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="04bd1-143">Int32</span></span>|<span data-ttu-id="04bd1-144">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="04bd1-144">Failed Device Count.</span></span>|
|<span data-ttu-id="04bd1-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="04bd1-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="04bd1-146">Int32</span><span class="sxs-lookup"><span data-stu-id="04bd1-146">Int32</span></span>|<span data-ttu-id="04bd1-147">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="04bd1-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="04bd1-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="04bd1-148">Response</span></span>
<span data-ttu-id="04bd1-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="04bd1-149">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04bd1-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04bd1-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="04bd1-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04bd1-151">Request</span></span>
<span data-ttu-id="04bd1-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04bd1-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
Content-type: application/json
Content-length: 127

{
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="04bd1-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="04bd1-153">Response</span></span>
<span data-ttu-id="04bd1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04bd1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```





