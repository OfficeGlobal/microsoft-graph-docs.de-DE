---
title: Ressourcentyp educationSynchronizationConnectionSettings
description: 'Stellt die Einstellungen für die Anbieter-Verbindung dar. Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden. '
ms.openlocfilehash: 27cdd377318d3294be9802b7cf28e940d0ada31c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062404"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="893f9-104">Ressourcentyp educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="893f9-104">educationSynchronizationConnectionSettings resource type</span></span>

> <span data-ttu-id="893f9-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="893f9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="893f9-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="893f9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="893f9-107">Stellt die Einstellungen für die Anbieter-Verbindung dar.</span><span class="sxs-lookup"><span data-stu-id="893f9-107">Represents the provider connection settings.</span></span> <span data-ttu-id="893f9-108">Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden.</span><span class="sxs-lookup"><span data-stu-id="893f9-108">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="893f9-109">**Hinweis:** Dieser komplexe Typ ist abstrakt.</span><span class="sxs-lookup"><span data-stu-id="893f9-109">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="893f9-110">Verweisen Sie auf die bestimmten Arten von Verbindungseinstellungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="893f9-110">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="893f9-111">Abgeleitete Typen</span><span class="sxs-lookup"><span data-stu-id="893f9-111">Derived types</span></span>
| <span data-ttu-id="893f9-112">Typ</span><span class="sxs-lookup"><span data-stu-id="893f9-112">Type</span></span> | <span data-ttu-id="893f9-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="893f9-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="893f9-114">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="893f9-114">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="893f9-115">Verwenden Sie diesen Typ OAuth1 Verbindungseinstellungen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="893f9-115">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="893f9-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="893f9-116">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="893f9-117">Verwenden Sie diesen Typ OAuth2 Client Anmeldeinformationen Grant-Verbindungseinstellungen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="893f9-117">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="893f9-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="893f9-118">Properties</span></span>

| <span data-ttu-id="893f9-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="893f9-119">Property</span></span> | <span data-ttu-id="893f9-120">Typ</span><span class="sxs-lookup"><span data-stu-id="893f9-120">Type</span></span> | <span data-ttu-id="893f9-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="893f9-121">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="893f9-122">**clientId**</span><span class="sxs-lookup"><span data-stu-id="893f9-122">**clientId**</span></span> | <span data-ttu-id="893f9-123">String</span><span class="sxs-lookup"><span data-stu-id="893f9-123">String</span></span> |  <span data-ttu-id="893f9-124">Client-ID für die Verbindung an den Anbieter verwendet.</span><span class="sxs-lookup"><span data-stu-id="893f9-124">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="893f9-125">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="893f9-125">**clientSecret**</span></span> | <span data-ttu-id="893f9-126">String</span><span class="sxs-lookup"><span data-stu-id="893f9-126">String</span></span> |  <span data-ttu-id="893f9-127">Geheimer Clientschlüssel zum Authentifizieren der Verbindungs an den Anbieter.</span><span class="sxs-lookup"><span data-stu-id="893f9-127">Client secret to authenticate the connection to the provider.</span></span> |