---
title: GetEncryptionPublicKey-Funktion
description: Rufen Sie einen öffentlichen Schlüssel zum Verschlüsseln des Apple Gerät Registrierung Programms token ab
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eb373b862dc39d9636e59bf32ba00b84b7bf5563
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807630"
---
# <a name="getencryptionpublickey-function"></a><span data-ttu-id="21cad-103">GetEncryptionPublicKey-Funktion</span><span class="sxs-lookup"><span data-stu-id="21cad-103">getEncryptionPublicKey function</span></span>

> <span data-ttu-id="21cad-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="21cad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21cad-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21cad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21cad-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="21cad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21cad-107">Rufen Sie einen öffentlichen Schlüssel zum Verschlüsseln des Apple Gerät Registrierung Programms token ab</span><span class="sxs-lookup"><span data-stu-id="21cad-107">Get a public key to use to encrypt the Apple device enrollment program token</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21cad-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21cad-108">Prerequisites</span></span>
<span data-ttu-id="21cad-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21cad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21cad-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21cad-111">Permission type</span></span>|<span data-ttu-id="21cad-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21cad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21cad-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21cad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21cad-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="21cad-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="21cad-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21cad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21cad-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21cad-116">Not supported.</span></span>|
|<span data-ttu-id="21cad-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21cad-117">Application</span></span>|<span data-ttu-id="21cad-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21cad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21cad-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21cad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

## <a name="request-headers"></a><span data-ttu-id="21cad-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21cad-120">Request headers</span></span>
|<span data-ttu-id="21cad-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="21cad-121">Header</span></span>|<span data-ttu-id="21cad-122">Wert</span><span class="sxs-lookup"><span data-stu-id="21cad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21cad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21cad-123">Authorization</span></span>|<span data-ttu-id="21cad-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21cad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21cad-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="21cad-125">Accept</span></span>|<span data-ttu-id="21cad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21cad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21cad-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21cad-127">Request body</span></span>
<span data-ttu-id="21cad-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="21cad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21cad-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="21cad-129">Response</span></span>
<span data-ttu-id="21cad-130">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="21cad-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21cad-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21cad-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="21cad-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21cad-132">Request</span></span>
<span data-ttu-id="21cad-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21cad-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

### <a name="response"></a><span data-ttu-id="21cad-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="21cad-134">Response</span></span>
<span data-ttu-id="21cad-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21cad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 50

{
  "value": "Get Encryption Public Key value"
}
```





