## Locale 报错

```bash
perl: warning: Setting locale failed.
perl: warning: Please check that your locale settings:
	LANGUAGE = (unset),
	LC_ALL = (unset),
	LC_CTYPE = "zh_CN.UTF-8",
	LANG = "en_US.utf8"
    are supported and installed on your system.
perl: warning: Falling back to a fallback locale ("en_US.utf8").
locale: Cannot set LC_CTYPE to default locale: No such file or directory
locale: Cannot set LC_ALL to default locale: No such file or directory
```
- 解决方法

```bash
export LC_ALL=C.UTF-8
sudo update-locale LANG=C.UTF-8 LC_CTYPE=C.UTF-8
. /etc/default/locale

```