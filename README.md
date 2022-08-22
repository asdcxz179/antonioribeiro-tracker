# Tracker 套件
## Function
#### 取得全部Tracker Session
```php
Tracker::currentSession()
```
```json
    [
        {
            "id":7,
            "uuid":"51a0a114-7fa0-4232-a2fc-beb0171bfdda",
            "user_id":"453",
            "device_id":"1",
            "agent_id":"1",
            "client_ip":"13.78.85.146"//使用者IP, 
            "referer_id":"2",
            "cookie_id":"10",
            "geoip_id":"1",
            "is_robot":"0",
            "created_at":"2022-08-22 09:08:01",
            "updated_at":"2022-08-22 09:30:06",
            "language_id":"1",
            "device":{
                "id":1,
                "kind":"Computer"//使用裝置,
                "model":"WebKit",
                "platform":"Windows"//使用作業系統,
                "platform_version":"10"//作業系統版本,
                "is_mobile":"0"//是否為移動裝置,
                "created_at":"2022-08-19 16:02:34",
                "updated_at":"2022-08-19 16:02:34"
            },
            "user":null,
            "log":[
                {
                    "id":129,
                    "session_id":"7",
                    "path_id":"1",
                    "query_id":null,
                    "method":"GET",
                    "route_path_id":"1",
                    "is_ajax":"0",
                    "is_secure":"0",
                    "is_json":"0",
                    "wants_json":"0",
                    "error_id":"16",
                    "created_at":"2022-08-22 09:25:39",
                    "updated_at":"2022-08-22 09:25:39",
                    "referer_id":null
                }
            ],
            "language":{
                "id":1,
                "preference":"zh-tw"//使用語系,
                "language-range":"zh-tw,zh-cn,zh,en-us,en",
                "created_at":"2022-08-19 16:02:34",
                "updated_at":"2022-08-19 16:02:34"
            },
            "agent":{
                "id":1,
                "name":"Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/104.0.0.0 Safari\/537.36",
                "browser":"Chrome"//使用瀏覽器,
                "browser_version":"104.0.0"//瀏覽器版本,
                "created_at":"2022-08-19 16:02:34",
                "updated_at":"2022-08-19 16:02:34",
                "name_hash":"b2bd210f94c4a45e0c0b5604ba7b3fea21a1c339e7f72a0db98d8244b451d197"
            },
            "referer":{
                "id":2,
                "domain_id":"1",
                "url":"http:\/\/twhome.henryegg8.com\/logintw",
                "host":"twhome.henryegg8.com",
                "created_at":"2022-08-19 16:06:34",
                "updated_at":"2022-08-19 16:06:34",
                "medium":null,
                "source":null,
                "search_terms_hash":null
            },
            "geo_ip":{
                "id":1,
                "latitude":"35.6893"//使用者經度,
                "longitude":"139.6899"//使用者緯度,
                "country_code":"JP"//使用者國家,
                "country_code3":null,
                "country_name":"Japan"//使用者國家名,
                "region":"AS"//使用者地區,
                "city":"Tokyo"//使用者城市,
                "postal_code":"102-0082"//郵遞區號,
                "area_code":null,
                "dma_code":null,
                "metro_code":null,
                "continent_code":"AS",
                "created_at":"2022-08-19 16:04:16",
                "updated_at":"2022-08-19 16:04:16"
            },
            "cookie":{
                "id":10,
                "uuid":"933466ff-e6bc-4866-b4d2-65f9b4f783d6",
                "created_at":"2022-08-22 09:08:07",
                "updated_at":"2022-08-22 09:08:07"
            }
        }
    ]
```
#### 檢查當前使用者
```php
Tracker::checkCurrentUser()
```
```boolean
false
```
#### 當前Session
```php
Tracker::currentSession()
```
```json
    {
        "id":7,
        "uuid":"51a0a114-7fa0-4232-a2fc-beb0171bfdda",
        "user_id":"453",
        "device_id":"1",
        "agent_id":"1",
        "client_ip":"13.78.85.146"//使用者IP, 
        "referer_id":"2",
        "cookie_id":"10",
        "geoip_id":"1",
        "is_robot":"0",
        "created_at":"2022-08-22 09:08:01",
        "updated_at":"2022-08-22 09:30:06",
        "language_id":"1",
        "device":{
            "id":1,
            "kind":"Computer"//使用裝置,
            "model":"WebKit",
            "platform":"Windows"//使用作業系統,
            "platform_version":"10"//作業系統版本,
            "is_mobile":"0"//是否為移動裝置,
            "created_at":"2022-08-19 16:02:34",
            "updated_at":"2022-08-19 16:02:34"
        },
        "user":null,
        "log":[
            {
                "id":129,
                "session_id":"7",
                "path_id":"1",
                "query_id":null,
                "method":"GET",
                "route_path_id":"1",
                "is_ajax":"0",
                "is_secure":"0",
                "is_json":"0",
                "wants_json":"0",
                "error_id":"16",
                "created_at":"2022-08-22 09:25:39",
                "updated_at":"2022-08-22 09:25:39",
                "referer_id":null
            }
        ],
        "language":{
            "id":1,
            "preference":"zh-tw"//使用語系,
            "language-range":"zh-tw,zh-cn,zh,en-us,en",
            "created_at":"2022-08-19 16:02:34",
            "updated_at":"2022-08-19 16:02:34"
        },
        "agent":{
            "id":1,
            "name":"Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/104.0.0.0 Safari\/537.36",
            "browser":"Chrome"//使用瀏覽器,
            "browser_version":"104.0.0"//瀏覽器版本,
            "created_at":"2022-08-19 16:02:34",
            "updated_at":"2022-08-19 16:02:34",
            "name_hash":"b2bd210f94c4a45e0c0b5604ba7b3fea21a1c339e7f72a0db98d8244b451d197"
        },
        "referer":{
            "id":2,
            "domain_id":"1",
            "url":"http:\/\/twhome.henryegg8.com\/logintw",
            "host":"twhome.henryegg8.com",
            "created_at":"2022-08-19 16:06:34",
            "updated_at":"2022-08-19 16:06:34",
            "medium":null,
            "source":null,
            "search_terms_hash":null
        },
        "geo_ip":{
            "id":1,
            "latitude":"35.6893"//使用者經度,
            "longitude":"139.6899"//使用者緯度,
            "country_code":"JP"//使用者國家,
            "country_code3":null,
            "country_name":"Japan"//使用者國家名,
            "region":"AS"//使用者地區,
            "city":"Tokyo"//使用者城市,
            "postal_code":"102-0082"//郵遞區號,
            "area_code":null,
            "dma_code":null,
            "metro_code":null,
            "continent_code":"AS",
            "created_at":"2022-08-19 16:04:16",
            "updated_at":"2022-08-19 16:04:16"
        },
        "cookie":{
            "id":10,
            "uuid":"933466ff-e6bc-4866-b4d2-65f9b4f783d6",
            "created_at":"2022-08-22 09:08:07",
            "updated_at":"2022-08-22 09:08:07"
        }
    }
```
#### 查看所有發生錯誤的請求
```php
Tracker::errors($minutes, $results = true)
//$minutes 查看幾分鐘內的錯誤
//$results 是否取得結果
```
```json
    [
        {
            "id":161,
            "session_id":"8",
            "path_id":"1",
            "query_id":null,
            "method":"GET"//請求方法,
            "route_path_id":"1",
            "is_ajax":"0",
            "is_secure":"0",
            "is_json":"0",
            "wants_json":"0",
            "error_id":"16",
            "created_at":"2022-08-22 09:57:54",
            "updated_at":"2022-08-22 09:57:54",
            "referer_id":null,
            "error":{
                "id":16,
                "code":"8",
                "message":"iconv(): Detected an illegal character in input string"//錯誤訊息,
                "created_at":"2022-08-19 17:31:18",
                "updated_at":"2022-08-19 17:31:18"
            },
            "session":{
                "id":8,
                "uuid":"3879bbf6-0d6d-48aa-bd13-2884164e2c16",
                "user_id":null,"device_id":"1",
                "agent_id":"1",
                "client_ip":"13.78.85.146",
                "referer_id":null,
                "cookie_id":"22",
                "geoip_id":"1",
                "is_robot":"0",
                "created_at":"2022-08-22 09:55:09",
                "updated_at":"2022-08-22 09:57:55",
                "language_id":"2"
            },
            "path":{
                "id":1,
                "path":"test"//網址PATH,
                "created_at":"2022-08-19 16:02:34",
                "updated_at":"2022-08-19 16:02:34"
            }
        }
    ]
```
