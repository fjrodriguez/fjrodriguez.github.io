# Configurar RAMDisk in Windows

* Ver este video de Youtube: [Protege tu SSD con un RAMDISK](https://www.youtube.com/watch?v=_f5SlCHQIA4&t=923s)

## Configurar navegador Brave

Los comandos para configurar el navegador Brave son:

{% highlight  Batchfile%}
REM Kill al processes of Brave Browser
taskkill /F /IM brave.exe
rd /S /Q "%USERPROFILE%\AppData\Local\BraveSoftware\Brave-Browser\User Data\Default\Cache\Cache_Data"
rd /S /Q "%USERPROFILE%\AppData\Local\BraveSoftware\Brave-Browser\User Data\Default\Code Cache"
rd /S /Q "%USERPROFILE%\AppData\Local\BraveSoftware\Brave-Browser\User Data\Default\Service Worker"
md "Z:\Browsers\Brave-Browser\User Data\Default\Cache\Cache_Data"
md "Z:\Browsers\Brave-Browser\User Data\Default\Code Cache"
md "Z:\Browsers\Brave-Browser\User Data\Default\Service Worker"
md "C:\RAMDisk\Browsers\Brave-Browser\User Data\Default\Cache\Cache_Data"
md "C:\RAMDisk\Browsers\Brave-Browser\User Data\Default\Code Cache"
md "C:\RAMDisk\Browsers\Brave-Browser\User Data\Default\Service Worker"
mklink /D "%USERPROFILE%\AppData\Local\BraveSoftware\Brave-Browser\User Data\Default\Cache\Cache_Data" "Z:\Browsers\Brave-Browser\User Data\Default\Cache\Cache_Data"
mklink /D "%USERPROFILE%\AppData\Local\BraveSoftware\Brave-Browser\User Data\Default\Code Cache" "Z:\Browsers\Brave-Browser\User Data\Default\Code Cache"
mklink /D "%USERPROFILE%\AppData\Local\BraveSoftware\Brave-Browser\User Data\Default\Service Worker" "Z:\Browsers\Brave-Browser\User Data\Default\Service Worker"
REM Reboot system
{% endhighlight %}