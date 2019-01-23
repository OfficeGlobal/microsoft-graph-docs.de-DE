---
title: eBookInstallSummary aktualisieren
description: Aktualisieren der Eigenschaften des eBookInstallSummary-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 85e94a16799b9ee56c28041549b1d21692013599
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421165"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="beb71-103">eBookInstallSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="beb71-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="beb71-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="beb71-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="beb71-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="beb71-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="beb71-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="beb71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beb71-107">Aktualisieren der Eigenschaften des [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="beb71-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="beb71-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="beb71-108">Prerequisites</span></span>
<span data-ttu-id="beb71-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="beb71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="beb71-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="beb71-111">Permission type</span></span>|<span data-ttu-id="beb71-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="beb71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beb71-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="beb71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="beb71-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb71-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="beb71-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="beb71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beb71-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beb71-116">Not supported.</span></span>|
|<span data-ttu-id="beb71-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="beb71-117">Application</span></span>|<span data-ttu-id="beb71-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beb71-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="beb71-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="beb71-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="beb71-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="beb71-120">Request headers</span></span>
|<span data-ttu-id="beb71-121">Header</span><span class="sxs-lookup"><span data-stu-id="beb71-121">Header</span></span>|<span data-ttu-id="beb71-122">Wert</span><span class="sxs-lookup"><span data-stu-id="beb71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beb71-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="beb71-123">Authorization</span></span>|<span data-ttu-id="beb71-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="beb71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beb71-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="beb71-125">Accept</span></span>|<span data-ttu-id="beb71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="beb71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beb71-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="beb71-127">Request body</span></span>
<span data-ttu-id="beb71-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="beb71-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="beb71-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="beb71-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="beb71-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="beb71-130">Property</span></span>|<span data-ttu-id="beb71-131">Typ</span><span class="sxs-lookup"><span data-stu-id="beb71-131">Type</span></span>|<span data-ttu-id="beb71-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="beb71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beb71-133">id</span><span class="sxs-lookup"><span data-stu-id="beb71-133">id</span></span>|<span data-ttu-id="beb71-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="beb71-134">String</span></span>|<span data-ttu-id="beb71-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="beb71-135">Key of the entity.</span></span>|
|<span data-ttu-id="beb71-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="beb71-136">installedDeviceCount</span></span>|<span data-ttu-id="beb71-137">Int32</span><span class="sxs-lookup"><span data-stu-id="beb71-137">Int32</span></span>|<span data-ttu-id="beb71-138">Die Anzahl der Geräte, auf denen das Buch erfolgreich installiert wurde.</span><span class="sxs-lookup"><span data-stu-id="beb71-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="beb71-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="beb71-139">failedDeviceCount</span></span>|<span data-ttu-id="beb71-140">Int32</span><span class="sxs-lookup"><span data-stu-id="beb71-140">Int32</span></span>|<span data-ttu-id="beb71-141">Die Anzahl der Geräte, auf denen die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="beb71-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="beb71-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="beb71-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="beb71-143">Int32</span><span class="sxs-lookup"><span data-stu-id="beb71-143">Int32</span></span>|<span data-ttu-id="beb71-144">Die Anzahl von Geräten, auf denen das Buch nicht installiert ist.</span><span class="sxs-lookup"><span data-stu-id="beb71-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="beb71-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="beb71-145">installedUserCount</span></span>|<span data-ttu-id="beb71-146">Int32</span><span class="sxs-lookup"><span data-stu-id="beb71-146">Int32</span></span>|<span data-ttu-id="beb71-147">Die Anzahl der Benutzer, deren Geräte das Buch erfolgreich installiert haben.</span><span class="sxs-lookup"><span data-stu-id="beb71-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="beb71-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="beb71-148">failedUserCount</span></span>|<span data-ttu-id="beb71-149">Int32</span><span class="sxs-lookup"><span data-stu-id="beb71-149">Int32</span></span>|<span data-ttu-id="beb71-150">Die Anzahl der Benutzer, die mindestens ein Gerät besitzen, auf dem die Installation des Buchs fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="beb71-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="beb71-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="beb71-151">notInstalledUserCount</span></span>|<span data-ttu-id="beb71-152">Int32</span><span class="sxs-lookup"><span data-stu-id="beb71-152">Int32</span></span>|<span data-ttu-id="beb71-153">Die Anzahl der Benutzer, die das Buch nicht installiert haben.</span><span class="sxs-lookup"><span data-stu-id="beb71-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="beb71-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="beb71-154">Response</span></span>
<span data-ttu-id="beb71-155">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="beb71-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beb71-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="beb71-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="beb71-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="beb71-157">Request</span></span>
<span data-ttu-id="beb71-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="beb71-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="beb71-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="beb71-159">Response</span></span>
<span data-ttu-id="beb71-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="beb71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```




