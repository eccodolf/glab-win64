# glab for Windows x64

Официальные сборки [GitLab CLI (`glab`)](https://gitlab.com/gitlab-org/cli) **v1.115.0** для Windows x86_64,
скачанные без изменений с официального релиза GitLab и проверенные по SHA256.

| Файл | Что это | Размер |
| --- | --- | --- |
| `glab_1.115.0_windows_amd64.zip` | Портативный архив с `bin/glab.exe` | 17.5 MB |
| `glab_1.115.0_Windows_x86_64_installer.exe` | Установщик под Windows | 15.0 MB |
| `checksums.txt` | Официальный список SHA256 для всех артефактов релиза | 3.4 KB |

## Происхождение

- Релиз: <https://gitlab.com/gitlab-org/cli/-/releases/v1.115.0> (опубликован 2026-08-25)
- Источник загрузки: `https://gitlab.com/api/v4/projects/gitlab-org%2Fcli/packages/generic/glab/1.115.0/`

## Проверка контрольных сумм

```powershell
Get-FileHash glab_1.115.0_windows_amd64.zip -Algorithm SHA256
Get-FileHash glab_1.115.0_Windows_x86_64_installer.exe -Algorithm SHA256
```

Ожидаемые значения:

```
4a58f7ce5003d33d8dd58e31534b215a26a1c0c31bd0fc51cd09a339a56a7ecb  glab_1.115.0_windows_amd64.zip
5d5d4ae9770d77b6fa9bac755b9c7ee22658552dcdb1c7e7a3cd02d52de2c3b2  glab_1.115.0_Windows_x86_64_installer.exe
```

## Установка

**Портативно:** распакуйте zip и добавьте папку `bin` в `PATH`.

```powershell
Expand-Archive glab_1.115.0_windows_amd64.zip -DestinationPath C:\Tools\glab
C:\Tools\glab\bin\glab.exe --version
```

**Установщиком:** запустите `glab_1.115.0_Windows_x86_64_installer.exe`.

## Лицензия

`glab` распространяется по лицензии MIT — см. `LICENSE` внутри архива и
<https://gitlab.com/gitlab-org/cli/-/blob/main/LICENSE>. Этот репозиторий —
лишь зеркало официальных артефактов, код не изменялся.
