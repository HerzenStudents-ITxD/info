# info
## Бекэнд
Для тех, у кого не получается сделать нормальный бекэнд, можно использовать инструмент его эмулирования:
* Сначала узнаём номер своей команды (owner): GET https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owners;
* Потом смотрите список существующих типов json, которые существуют в команде: GET https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owner/1/types;
* Если не находите нужного, придумываете его название, например (product);
* Сохранить json для product: POST https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owner/1/type/product/items, сам json в body складываете,
на вход принимается только валидный json;
* Получить все json для product: GET https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owner/1/type/product/items; 
* Получить конкретный json по его id: GET https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owner/1/type/product/items/17;
* Изменить конкретный json по его id: PATCH https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owner/1/type/product/items/17, сам json в body складываете,
на вход принимается только валидный json.
