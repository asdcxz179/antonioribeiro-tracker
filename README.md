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
#### 查看發生錯誤的請求
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
#### 查看發生事件
```php
Tracker::events($minutes, $results = true)
//$minutes 查看幾分鐘內的事件
//$results 是否取得結果
```

```json
[
    {
        "id":1,
        "name":"auth.login"//事件名稱,
        "total":"17"//次數
    }
]   
```
#### 取得AgentId
```php
Tracker::getAgentId()
//對應tracker_agents.id
```
```
1(Int)
```
#### 取得Tracker設定
```php
Tracker::getConfig($key)
//對應config/tracker.php key
```
#### 取得CookieId
```php
Tracker::getCookieId()
//對應tracker_cookies.id
```
```
1(Int)
```
#### 取得DeviceId
```php
Tracker::getDeviceId()
//對應tracker_devices.id
```
```
1(Int)
```
#### 取得LanguageId
```php
Tracker::getLanguageId()
//對應tracker_languages.id
```
```
1(Int)
```
#### 取得DomainId
```php
Tracker::getDomainId()
//對應tracker_domains.id
```
```
1(Int)
```
#### 取得GeoIpId
```php
Tracker::getGeoIpId()
//對應tracker_geoip.id
```
```
1(Int)
```
#### 取得LogData
```php
Tracker::getLogData()
//對應tracker_geoip.id
```
```json
{
    "session_id":7,
    "method":"GET",
    "path_id":1,
    "query_id":null,
    "referer_id":null,
    "is_ajax":false,
    "is_secure":false,
    "is_json":false,
    "wants_json":false
}
```
#### 取得紀錄logger Provider
```php
Tracker::getLogger()
//對應本地laravel log
```
#### 取得PathId
```php
Tracker::getPathId()
//對應tracker_paths.id
```
```
1(Int)
```
#### 取得QueryId
```php
Tracker::getQueryId()
//對應tracker_queries.id
```
```
1(Int)
```
#### 取得RefererId
```php
Tracker::getRefererId()
//對應tracker_referers.id
```
```
1(Int)
```
#### 取得RoutePathId
```php
Tracker::getRoutePathId()
//對應tracker_route_paths.id
```
```
1(Int)
```
#### 取得SessionId
```php
Tracker::getSessionId()
//對應tracker_sessions.id
```
```
1(Int)
```
#### 取得UserId
```php
Tracker::getUserId()
//對應members.rowid
```
```
1(Int)
```
#### 使否開啟追蹤功能
```php
Tracker::isEnabled()
```
```boolean
false
```
#### 是否為爬蟲機器人
```php
Tracker::isRobot()
```
```boolean
false
```
#### 是否有符合所需的追蹤資訊
```php
Tracker::isTrackable()
```
```boolean
true
```
#### 是否為可追蹤的環境
```php
Tracker::isTrackableEnvironment()
```
```boolean
true
```
#### 是否有可追蹤的IP
```php
Tracker::isTrackableIp()
```
```boolean
true
```
#### 取得要追蹤的route name
```php
Tracker::logByRouteName($name,$minutes = null)
//$name route名
//$minutes 查看幾分鐘內的事件
```
#### 取得要追蹤事件
```php
Tracker::logEvents()
```
#### LOG是否開啟
```php
Tracker::logIsEnabled()
```
#### 取得追蹤總頁數
```php
Tracker::pageViews($minutes, $results = true)
//$minutes 查看幾分鐘內的事件
//$results 是否取得結果
```
```json
[
    {
        "date":"2022-08-22",
        "total":"56"
    }
]
```
#### 取得國家追蹤總頁數
```php
Tracker::pageViewsByCountry($minutes, $results = true)
//$minutes 查看幾分鐘內的事件
//$results 是否取得結果
```
```json
[
    {
        "label":"Japan",
        "value":"58"
     }
]
```
#### 是否開啟artisan指令
```php
Tracker::allowConsole()
```
```boolean
true
```
#### 是否開啟正則匹配
```php
Tracker::parserIsAvailable()
```
```boolean
true
```
#### 使否使用相同已存在資料庫的route
```php
Tracker::routerMatched($log)
```
```boolean
1(Int)
```
#### 取得該uuid 的session紀錄
```php
Tracker::sessionLog($uuid, $results = true)
//$uuid 對應tracker_sessions.uuid
//$results 是否取得結果
```
```boolean
[
    {
        "session_id":7,
        "method":"GET",
        "path_id":1,
        "query_id":null,
        "referer_id":null,
        "is_ajax":false,
        "is_secure":false,
        "is_json":false,
        "wants_json":false
    }
]
```
#### 取得該uuid 的session紀錄
```php
Tracker::sessions($minutes, $results = true)
//$minutes 查看幾分鐘內的session
//$results 是否取得結果
```
```boolean
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
