---
contentSidebar: true
sidebarDepth: 0
---

# NoneBot.utils 模块


## `escape_tag(s)`


* **说明**

    用于记录带颜色日志时转义 `<tag>` 类型特殊标签



* **参数**

    
    * `s: str`: 需要转义的字符串



* **返回**

    
    * `str`



## `run_sync(func)`


* **说明**

    一个用于包装 sync function 为 async function 的装饰器



* **参数**

    
    * `func: Callable[..., Any]`: 被装饰的同步函数



* **返回**

    
    * `Callable[..., Awaitable[Any]]`



## _class_ `DataclassEncoder`

基类：`json.encoder.JSONEncoder`


* **说明**

    在JSON序列化 `Message` (List[Dataclass]) 时使用的 `JSONEncoder`



## `logger_wrapper(logger_name)`


* **说明**


用于打印 adapter 的日志。


* **Log 参数**



* `level: Literal['WARNING', 'DEBUG', 'INFO']`: 日志等级


* `message: str`: 日志信息


* `exception: Optional[Exception]`: 异常信息
