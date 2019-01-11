---
title: Ressourcentyp educationSynchronizationConnectionSettings
description: 'Stellt die Einstellungen für die Anbieter-Verbindung dar. Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 17fedb5094016bd3df3bd8262390eaa7eeb37537
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841769"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="acdbe-104">Ressourcentyp educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="acdbe-104">educationSynchronizationConnectionSettings resource type</span></span>

> <span data-ttu-id="acdbe-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="acdbe-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acdbe-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="acdbe-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="acdbe-107">Stellt die Einstellungen für die Anbieter-Verbindung dar.</span><span class="sxs-lookup"><span data-stu-id="acdbe-107">Represents the provider connection settings.</span></span> <span data-ttu-id="acdbe-108">Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden.</span><span class="sxs-lookup"><span data-stu-id="acdbe-108">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="acdbe-109">**Hinweis:** Dieser komplexe Typ ist abstrakt.</span><span class="sxs-lookup"><span data-stu-id="acdbe-109">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="acdbe-110">Verweisen Sie auf die bestimmten Arten von Verbindungseinstellungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="acdbe-110">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="acdbe-111">Abgeleitete Typen</span><span class="sxs-lookup"><span data-stu-id="acdbe-111">Derived types</span></span>
| <span data-ttu-id="acdbe-112">Typ</span><span class="sxs-lookup"><span data-stu-id="acdbe-112">Type</span></span> | <span data-ttu-id="acdbe-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acdbe-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="acdbe-114">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="acdbe-114">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="acdbe-115">Verwenden Sie diesen Typ OAuth1 Verbindungseinstellungen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="acdbe-115">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="acdbe-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="acdbe-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="acdbe-117">Verwenden Sie diesen Typ OAuth2 Client Anmeldeinformationen Grant-Verbindungseinstellungen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="acdbe-117">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="acdbe-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="acdbe-118">Properties</span></span>

| <span data-ttu-id="acdbe-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="acdbe-119">Property</span></span> | <span data-ttu-id="acdbe-120">Typ</span><span class="sxs-lookup"><span data-stu-id="acdbe-120">Type</span></span> | <span data-ttu-id="acdbe-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acdbe-121">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="acdbe-122">**clientId**</span><span class="sxs-lookup"><span data-stu-id="acdbe-122">**clientId**</span></span> | <span data-ttu-id="acdbe-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acdbe-123">String</span></span> |  <span data-ttu-id="acdbe-124">Client-ID für die Verbindung an den Anbieter verwendet.</span><span class="sxs-lookup"><span data-stu-id="acdbe-124">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="acdbe-125">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="acdbe-125">**clientSecret**</span></span> | <span data-ttu-id="acdbe-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="acdbe-126">String</span></span> |  <span data-ttu-id="acdbe-127">Geheimer Clientschlüssel zum Authentifizieren der Verbindungs an den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="acdbe-127">Client secret to authenticate the connection to the provider.</span></span> |
