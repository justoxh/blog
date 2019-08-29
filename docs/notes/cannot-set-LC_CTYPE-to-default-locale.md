## Locale 报错

```bash
locale: Cannot set LC_CTYPE to default locale: No such file or directory
locale: Cannot set LC_ALL to default locale: No such file or directory
/usr/bin/locale: Cannot set LC_CTYPE to default locale: No such file or directory
/usr/bin/locale: Cannot set LC_ALL to default locale: No such file or directory
```
- 解决方法

```bash
export LC_ALL=C.UTF-8
sudo update-locale LANG=C.UTF-8 LC_CTYPE=C.UTF-8
. /etc/default/locale

```