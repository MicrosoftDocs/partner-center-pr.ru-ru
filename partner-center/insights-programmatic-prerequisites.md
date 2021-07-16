---
title: Предварительные требования для программного доступа к данным аналитики
description: Предварительные требования для программного доступа к данным аналитики
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375864"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Предварительные требования для программного доступа к данным аналитики

**Соответствующие роли:** Глобальный администратор | Администратор MPN

Прежде чем можно будет получить доступ к данным аналитики Partner Insights программным способом, необходимо выполнить следующие требования.

## <a name="mpn-program-enrollment"></a>Регистрация программы MPN

Чтобы получить доступ к данным аналитики Partner Insights программным способом, необходимо зарегистрироваться в программе MPN и получить учетную запись центра партнеров. Дополнительные сведения см. в статье [Создание учетной записи MPN в центре партнеров](mpn-create-a-partner-center-account.md) .

## <a name="create-azure-active-directory-aad-application"></a>создание приложения Azure Active Directory (AAD)

обычные учетные данные пользователя нельзя использовать для программного доступа к данным аналитики партнеров Аналитика. для доступа к api программного доступа необходимо создать приложение Azure Active Directory (AAD) вместе с секретом (доступ приложения и пользователя). сведения о создании приложения и секрета AAD см. в разделе [краткое руководство. регистрация приложения в платформа удостоверений Майкрософт.](/azure/active-directory/develop/quickstart-register-app)   Для доступа к Microsoft Partner API требуется разрешение. Чтобы узнать, как добавить разрешение, ознакомьтесь со статьей [Проверка подлинности партнерского API-партнера](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Назначить пользователю роль средства просмотра отчетов руководителя (ЕРВ)

Чтобы получить доступ к данным аналитики Partner Insights программным способом, необходимо иметь средство просмотра отчетов с руководителем (ЕРВ). чтобы узнать, как назначить роль ерв для пользователя, см. статью [центр партнеров Аналитика доступ на основе ролей в центре партнеров](insights-roles.md) .

## <a name="generate-an-aad-token"></a>Создание токена AAD

Необходимо создать токен AAD с помощью идентификатора приложения (клиента), секрета клиента, идентификатора пользователя и пароля. См.   [инструкции по созданию](insights-programmatic-first-api-call.md#token-generation) токена AAD.

> [!Note]
> Каждый маркер действителен в течение одного часа.

## <a name="next-steps"></a>Следующие шаги
[Парадигма программного доступа](insights-programmatic-access-paradigm.md)