## WSL 2(Windows Subsystem for Linux 2)

### 1. PowerShell(관리자)
```
$ dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

### 2. 재부팅

### 3. 가상 머신 플랫폼 옵션 사용: PowerShell(관리지)
```
$ dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

### 4. 리눅스 커널 업데이트 패키지
https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi

### 5. 재부팅

### 6. WSL2를 기본 버전으로 설정: PowerShell
```
$ wsl --set-default-version 2
```

### 7. 리눅스 배포판 설치: Microsoft 스토어
Ubuntu 20.04. LTS

### 8. Ubuntu 20.04. LTS
Enter new UNIX username: pc
New password:

```
$ sudo apt update && sudo apt upgrade
```

### 9. 배포 버전을 WSL2로 설정
```
$ wsl --list --verbose
  NAME            STATE           VERSION
* Ubuntu-20.04    Stopped         2
$ wsl --set-default-version 2
```
