
------------------------------------------------------------------------


报这个错误


  PS D:\files\using\Web\web_toutiao_SS_P> py  .\app.py
Traceback (most recent call last):
  File "D:\files\using\Web\web_toutiao_SS_P\app.py", line 10, in <module>
    from playwright.sync_api import sync_playwright
  File "C:\Users\windy2\AppData\Local\Programs\Python\Python312\Lib\site-packages\playwright\sync_api\__init__.py", line 25, in <module>
    import playwright.sync_api._generated
  File "C:\Users\windy2\AppData\Local\Programs\Python\Python312\Lib\site-packages\playwright\sync_api\_generated.py", line 42, in <module>
    from playwright._impl._assertions import (
  File "C:\Users\windy2\AppData\Local\Programs\Python\Python312\Lib\site-packages\playwright\_impl\_assertions.py", line 25, in <module>
    from playwright._impl._connection import format_call_log
  File "C:\Users\windy2\AppData\Local\Programs\Python\Python312\Lib\site-packages\playwright\_impl\_connection.py", line 42, in <module>
    from playwright._impl._greenlets import EventGreenlet
  File "C:\Users\windy2\AppData\Local\Programs\Python\Python312\Lib\site-packages\playwright\_impl\_greenlets.py", line 17, in <module>
    import greenlet
  File "C:\Users\windy2\AppData\Local\Programs\Python\Python312\Lib\site-packages\greenlet\__init__.py", line 29, in <module>    
    from ._greenlet import _C_API # pylint:disable=no-name-in-module
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
ImportError: DLL load failed while importing _greenlet: 找不到指定的模块。
PS D:\files\using\Web\web_toutiao_SS_P> 


------------------------------------------------

卸载greenlet  安装这个版本

pip install greenlet==3.0.3
