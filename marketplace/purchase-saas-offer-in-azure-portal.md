---
title: Как приобрести предложение SaaS в портал Azure
description: Узнайте, как найти и приобрести предложение SaaS в портал Azure.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: a124e4c5bb31a1fbb744bf2c5e1ea65a356bdd54
ms.sourcegitcommit: 1d09ccaaa54f167b0c63e99761172ebe84e89f2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2021
ms.locfileid: "113221446"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Приобретите предложение SaaS в портал Azure

В этой статье описываются различные варианты и требования для поиска, попыток и приобретения предложения "программное обеспечение как услуга" (SaaS) из портал Azure.

## <a name="create-a-saas-subscription"></a>Создание подписки SaaS

Чтобы приобрести подписку SaaS, вам потребуется учетная запись пользователя Azure с доступом к соответствующей подписке Azure. Эта подписка будет использоваться для выставления счетов, а также для обособление приобретенных облачных ресурсов. Дополнительные сведения о подписках Azure см. в статье [Создание дополнительной подписки Azure](/azure/cost-management-billing/manage/create-subscription).

В портал Azure выберите нужное предложение SaaS в разделе **Marketplace** .

Подписка "программное обеспечение как услуга" предоставляет право на использование службы в течение заданного периода времени через интерактивную подписку, а не локальную установку на отдельных компьютерах. Подписка — это соглашение об использовании одной или нескольких облачных платформ или служб, для которых взимается плата за использование лицензий на пользователя или на потребление ресурсов на основе облака. Организация может иметь несколько подписок SaaS.

К ограничениям на подписки SaaS относятся:

- Нет подписок на учащихся.
- нет подписки Visual Studio Enterprise.
- Нет бесплатных кредитных подписок.
- Для платных предложений требуется платежное средство.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS предлагает обнаружение в портал Azure

После портал Azure вы найдете несколько способов сузить область поиска, чтобы сосредоточиться на предложениях SaaS.

### <a name="narrowing-your-search"></a>Ограничение поиска

На домашней странице в разделе **службы Azure** выберите **+ создать ресурс** или **Marketplace**. Или используйте сочетание **G + N** в любом месте платформы.

- Ограничьте результаты до предложений SaaS, используя фильтр **типа предложения** , а затем выбрав **SaaS**.
- Используйте глобальную панель поиска в верхней области навигации, чтобы найти конкретное предложение SaaS.

Для поиска [частного предложения SaaS](/marketplace/private-offers) выберите баннер в верхней части домашней страницы **Marketplace** . Не все предложения или планы доступны во всех регионах, и некоторые из них могут отображаться только для определенных клиентов.

Отфильтрованное представление показывает каждое доступное предложение SaaS, представленное заголовком. Выберите один из них, чтобы просмотреть страницу сведений о продукте. Который включает в себя следующие разделы:

- Обзор — сведения о службе, маркетинговых и учебных материалах
- Планы + цены — каждое предложение будет включать по крайней мере один план с разными условиями и ценами для выставления счетов.
- сведения об использовании + поддержка — включает идентификатор Publisher, идентификатор предложения и идентификатор плана
- Оценка и обзоры конкретного предложения SaaS

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Доступные модели выставления счетов (планы/SKU) для предложений SaaS

Каждое предложение SaaS будет иметь один или несколько планов. С каждым предложением связана модель ценообразования: фиксированная ставка или на пользователя. Каждая Цена плана является повторяющейся платой, которая может равняться нулю (любые указанные цены относятся только к примеру и не рассчитаны на отображение фактических затрат). Это плата с фиксированным тарифом или ценой на пользователя. Доступные типы планов:

- **Ежемесячные планы** — периодическая ежемесячная плата; Ежемесячная плата за фиксированный объем или на пользователя, выплачиваемая ежемесячно. По окончании срока действия план будет продлен автоматически.
- **Ежегодные планы** — период ежегодной оплаты; Ежегодная или ежемесячная плата за каждый пользователь, которая оплачивается в течение ежегодного повторения. По окончании срока действия план будет продлен автоматически.
- **Пользовательские счетчики** . Вместе с повторяющимися платами тарифный план также может включать необязательные настраиваемые измерения для чрезмерного использования, не включенные в фиксированную ставку. Каждое измерение представляет оплачиваемую единицу. Это переменные затраты, которые изменяются в соответствии с использованием единиц измерения, таких как пропускная способность, билеты или обработка электронной почты. За использование этих измерений ежемесячно будет взиматься оплата. Обратите внимание, что превышение потребления начинается только при использовании всех единиц измерения, включенных в фиксированную ставку.
- **Бесплатная пробная версия** . в некоторых случаях план включает пробный период в один месяц, в течение которого можно бесплатно использовать программное обеспечение.  По истечении пробного периода вы получите оплату в соответствии с планом. Предложения по пробной версии не совместимы с пользовательскими счетчиками.

Эти модели ценообразования доступны как для общедоступных, так и для частных планов.

## <a name="saas-purchase-experience"></a>Опыт приобретения SaaS

1. На странице продукт выберите план, который соответствует вашим потребностям, и продолжайте **настройку подписки** .
2. В рамках процесса покупки вы будете перенаправлены на вкладку " **основы** ", и вам потребуется:
    1. Укажите, какую *подписку* вы хотите использовать для выставления счетов. Для подписки Azure, которую вы используете, должен быть определен допустимый метод покупки. У вас должен быть нужный уровень разрешений или группа ресурсов в подписке с нужным уровнем разрешений. Кроме того, в качестве страны выставления счетов следует использовать страну, в которой предложение доступно для приобретения. Подписки Azure без допустимого способа оплаты (например, подписки MSDN) можно использовать только для приобретения бесплатных планов.
    1. Выберите или создайте **группу ресурсов* , к которой будет принадлежать ресурс SaaS.
    1. Введите *имя* подписки SaaS, которое будет легко распознать позже. После приобретения вы не сможете изменить имя.
    1. В разделе **план** вы увидите план, выбранный на странице подробное описание продукта (PDP). Если вы еще не сделали активным выделение в PDP, вы увидите план по умолчанию. Вы можете изменить выбор, выбрав ссылку **изменить план** . Выберите соответствующий срок выставления счетов, а затем выберите другой план. Вы можете изменить план после покупки, если издатель его поддерживает. Однако вы не сможете изменить этот термин с ежемесячного на годовой или с ежегодного на месяц.
    1. В случаях, когда используется модель ценообразования *для каждого пользователя*, может потребоваться указать число *пользователей*. Отображаемая цена будет изменяться в зависимости от выбранной подписки, плана и выбранного термина.
3. Перейти к вкладкам **тегов** . *теги* — это определяемые пользователем пары "ключ-значение", которые можно разместить непосредственно в ресурсе или группе ресурсов. С помощью тегов можно легко найти свой ресурс SaaS позже. Сейчас в Azure поддерживается до 50 тегов на ресурс или группу ресурсов. Теги можно добавлять к ресурсу во время его создания или к уже существующему ресурсу.
4. Продолжайте **Просмотр и подпишитесь** , чтобы просмотреть сведения о предложении и плане.
    1. Проверка *условия использования*, поправки и *политики конфиденциальности* *издателя, а* также для Azure Marketplace
    1. Возможно, вам будет предложено добавить контактные данные.
    1. Обзор *основных* сведений и *тегов*
5. После подтверждения выберите **подпишите**.

## <a name="saas-subscription-and-configuration"></a>Подписка и конфигурация SaaS

При выборе подписки выводится сообщение "Ваша подписка SaaS выполняется". Этот процесс займет несколько минут, не закрывайте окно, пока оно не будет завершено.

После завершения подписки появится сообщение о том, что подписка на SaaS завершена, и вы должны настроить учетную запись для начала работы с покупкой. Вы также получите электронное сообщение с запросом на активацию новой подписки. Если вы не настроили учетную запись SaaS, перешлите это сообщение соответствующему человеку.

Чтобы завершить процесс и приступить к использованию SaaS, вам необходимо приступить к настройке подписки. Нажав кнопку **настроить учетную запись** , вы перейдете на веб-сайт издателя.

Вы также можете проверить состояние подписки, щелкнув значок колокольчика в правом верхнем углу заголовка.

Если вы не завершите процесс настройки в течение *30 дней*, эта подписка SaaS будет автоматически *удалена*. Выставление счетов начнется после настройки учетной записи на веб-сайте издателя.

Сообщения об ошибках, которые могут возникнуть в процессе:

- Имя плана *выбранного плана* не может быть приобретено в бесплатной подписке.
  - Обновление учетной записи. Дополнительные сведения см. в разделе https://aka.ms/UpgradeFreeSub .

- Не удалось выполнить покупку, так как не удалось найти допустимую кредитную карту или метод оплаты, связанный с вашей подпиской Azure.
  - Используйте другую подписку Azure или адд\упдате текущую кредитную карту или метод оплаты для этой подписки и повторите попытку.

- *Название плана, выбранное* для предложения имя предложения с *именем* издателя Publisher *предложения* , недоступно для приобретения согласно правилам, заданным ИТ-администратором.
  - Обратитесь к ИТ администратора.

- *Название плана, выбранное* для плана предложения, *выбранного* в параметре издатель *предложения* , недоступно для покупки из-за личных параметров Marketplace, сделанных вашим администратором вашего клиента.
  - Обратитесь к ИТ – администратору

- Не удалось выполнить покупку, так как запрошенный срок выставления счетов пуст или недопустим.
  - Попробуйте приобрести другой план или срок выставления счетов.

- Не удалось выполнить покупку, так как не удалось проверить подписанное соглашение.
  - Повторная попытка. Если ошибка повторится, попробуйте сделать покупку с помощью другой подписки Azure или обратитесь в службу поддержки.

- Не удалось приобрести предложение *offerID* by Publisher *PublisherID* . В настоящее время это предложение недоступно для приобретения.
  - Повторите попытку позже. Если через час вы продолжаете получать это сообщение об ошибке, обратитесь в службу поддержки.  

- Не удалось приобрести план *planID* предложения *offerID* по издателю *PublisherID* . Этот план сейчас недоступен для покупок.
  - Повторите попытку позже. Если через час вы продолжаете получать это сообщение об ошибке, обратитесь в службу поддержки. 

- *Адрес электронной почты* клиента с идентификатором объекта *ObjectID* не имеет авторизации для выполнения действия *деплойментвалидатионактион* над областью *ResourceGroup; Деплойментскопе* или Недопустимая область.  
  - Вы получите это сообщение, если у вас нет нужных разрешений в подписке или группе ресурсов Azure.  
    Если доступ был недавно предоставлен, обновите учетные данные.  
    Для развертывания ресурсов в группе ресурсов необходимо иметь по крайней мере права участника. Проверьте состояние доступа в разделе **группы ресурсов** , а затем щелкните **Управление доступом**. Это показывает, кто является владельцем, которому можно попросить назначить вас как участника.

- Подписка, используемая для этой покупки, не допускает покупки в Marketplace.  
  - Используйте другую подписку или попросите администратора изменить определение для этой подписки и повторите попытку.

## <a name="next-steps"></a>Дальнейшие действия

- Если вы уже приобрели предложение в Marketplace, выберите [счет и выставление](/marketplace/billing-invoicing) счетов.
- Кроме того, вы можете узнать больше о вариантах [частных планов](/marketplace/private-offers) .
