---
title: getEncryptionPublicKey-Funktion
description: Abrufen eines öffentlichen Schlüssels zum Verschlüsseln des Apple-Geräte Registrierungsprogramm-Tokens
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd34c3e6e88d432601aacf6bd8c8df851c90baef
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965627"
---
# <a name="getencryptionpublickey-function"></a><span data-ttu-id="46e08-103">getEncryptionPublicKey-Funktion</span><span class="sxs-lookup"><span data-stu-id="46e08-103">getEncryptionPublicKey function</span></span>

> <span data-ttu-id="46e08-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46e08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46e08-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="46e08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46e08-106">Abrufen eines öffentlichen Schlüssels zum Verschlüsseln des Apple-Geräte Registrierungsprogramm-Tokens</span><span class="sxs-lookup"><span data-stu-id="46e08-106">Get a public key to use to encrypt the Apple device enrollment program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46e08-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="46e08-107">Prerequisites</span></span>
<span data-ttu-id="46e08-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46e08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46e08-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46e08-110">Permission type</span></span>|<span data-ttu-id="46e08-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46e08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46e08-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46e08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46e08-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="46e08-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="46e08-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46e08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46e08-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46e08-115">Not supported.</span></span>|
|<span data-ttu-id="46e08-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46e08-116">Application</span></span>|<span data-ttu-id="46e08-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46e08-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46e08-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46e08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

## <a name="request-headers"></a><span data-ttu-id="46e08-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46e08-119">Request headers</span></span>
|<span data-ttu-id="46e08-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="46e08-120">Header</span></span>|<span data-ttu-id="46e08-121">Wert</span><span class="sxs-lookup"><span data-stu-id="46e08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46e08-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46e08-122">Authorization</span></span>|<span data-ttu-id="46e08-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="46e08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46e08-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="46e08-124">Accept</span></span>|<span data-ttu-id="46e08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46e08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46e08-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46e08-126">Request body</span></span>
<span data-ttu-id="46e08-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="46e08-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46e08-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="46e08-128">Response</span></span>
<span data-ttu-id="46e08-129">Bei erfolgreicher Ausführung gibt die Funktion den `200 OK` Antwortcode und eine Zeichenfolge im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="46e08-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46e08-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46e08-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="46e08-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46e08-131">Request</span></span>
<span data-ttu-id="46e08-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46e08-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

### <a name="response"></a><span data-ttu-id="46e08-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="46e08-133">Response</span></span>
<span data-ttu-id="46e08-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46e08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 50

{
  "value": "Get Encryption Public Key value"
}
```




