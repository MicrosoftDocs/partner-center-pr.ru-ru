---
title: Поля для CSV-файла для импорта нескольких пользователей для учетной записи клиента
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Чтобы добавить нескольких пользователей в учетную запись клиента, создайте файл значений с разделителями-запятыми (CSV) с соответствующими полями.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441427"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="44a4b-103">Добавление нескольких пользователей в учетную запись клиента путем создания CSV-файла</span><span class="sxs-lookup"><span data-stu-id="44a4b-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="44a4b-104">**Соответствующие роли**</span><span class="sxs-lookup"><span data-stu-id="44a4b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="44a4b-105">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="44a4b-105">Global admin</span></span>

<span data-ttu-id="44a4b-106">Одновременное добавление нескольких пользователей в учетную запись клиента путем отправки файла данных в формате файла с разделителями-запятыми (CSV) в центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="44a4b-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="44a4b-107">Вы можете скачать образец файла данных из центра партнеров, а затем изменить его для использования или создать новый файл данных, используя модель данных, определенную ниже.</span><span class="sxs-lookup"><span data-stu-id="44a4b-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="44a4b-108">Требования к файлу данных</span><span class="sxs-lookup"><span data-stu-id="44a4b-108">Data file requirements</span></span>

<span data-ttu-id="44a4b-109">Чтобы добавить нескольких пользователей в учетную запись клиента с помощью процесса групповой отправки, необходимо выполнить следующие требования.</span><span class="sxs-lookup"><span data-stu-id="44a4b-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="44a4b-110">у вас должны быть разрешения глобального администратора для учетной записи клиента;</span><span class="sxs-lookup"><span data-stu-id="44a4b-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="44a4b-111">у каждого пользователя должен быть уникальный электронный адрес в почтовом домене пользователя;</span><span class="sxs-lookup"><span data-stu-id="44a4b-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="44a4b-112">одновременно можно передавать до 100 записей.</span><span class="sxs-lookup"><span data-stu-id="44a4b-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="44a4b-113">Если вам необходимо добавить более 100 пользователей, создайте и загрузите дополнительные файлы данных;</span><span class="sxs-lookup"><span data-stu-id="44a4b-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="44a4b-114">все пользователи должны быть в одном географическом **регионе**;</span><span class="sxs-lookup"><span data-stu-id="44a4b-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="44a4b-115">вводите только данные, описанные ниже.</span><span class="sxs-lookup"><span data-stu-id="44a4b-115">Enter only the data described below.</span></span> <span data-ttu-id="44a4b-116">Лишние данные приведут к ошибке отправки.</span><span class="sxs-lookup"><span data-stu-id="44a4b-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="44a4b-117">Введите следующие данные в файле данных:</span><span class="sxs-lookup"><span data-stu-id="44a4b-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="44a4b-118">**Имя столбца**</span><span class="sxs-lookup"><span data-stu-id="44a4b-118">**Column name**</span></span> | <span data-ttu-id="44a4b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="44a4b-119">**Description**</span></span>  | <span data-ttu-id="44a4b-120">**Ограничения**</span><span class="sxs-lookup"><span data-stu-id="44a4b-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="44a4b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="44a4b-121">First name</span></span>  | <span data-ttu-id="44a4b-122">Имя пользователя (необязательное поле)</span><span class="sxs-lookup"><span data-stu-id="44a4b-122">User's first name (optional field)</span></span>  | <span data-ttu-id="44a4b-123">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="44a4b-123">50-character limit</span></span>  |
| <span data-ttu-id="44a4b-124">Фамилия</span><span class="sxs-lookup"><span data-stu-id="44a4b-124">Last name</span></span>  | <span data-ttu-id="44a4b-125">Фамилия пользователя (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="44a4b-125">User's last name (optional field)</span></span>  | <span data-ttu-id="44a4b-126">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="44a4b-126">50-character limit</span></span>  |
| <span data-ttu-id="44a4b-127">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="44a4b-127">Display name</span></span>    | <span data-ttu-id="44a4b-128">Имя, отображаемое в центре партнеров (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="44a4b-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="44a4b-129">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="44a4b-129">50-character limit</span></span>                         |
| <span data-ttu-id="44a4b-130">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="44a4b-130">Email</span></span>   | <span data-ttu-id="44a4b-131">Рабочий адрес электронной почты пользователя в клиентской компании (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="44a4b-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="44a4b-132">Каждый пользователь должен иметь уникальный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="44a4b-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="44a4b-133">Обновление состояния</span><span class="sxs-lookup"><span data-stu-id="44a4b-133">Status update</span></span>   | <span data-ttu-id="44a4b-134">Используется для указания, успешно ли создана новая запись пользователя</span><span class="sxs-lookup"><span data-stu-id="44a4b-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="44a4b-135">\*\*Оставить пустым\*\*</span><span class="sxs-lookup"><span data-stu-id="44a4b-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="44a4b-136">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="44a4b-136">Next steps</span></span>

- [<span data-ttu-id="44a4b-137">Как добавить нескольких пользователей для клиента</span><span class="sxs-lookup"><span data-stu-id="44a4b-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)