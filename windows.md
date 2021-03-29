# windows

## techniques

### outdated software

### windows kernel

### vulnerable applications

### insecure services

#### weak service executable or config file permissions

#### unquoted service paths

#### weak service permissions

#### dll hijacking
- `Find-ProcessDLLHijack`
- `Find-PathDLLHijack`
- `Write-HijackDLL`

#### weak registry key permissions

### insecure credentials

#### cleartext passwords
- configuration files
  - `findstr /si password passwd *.txt`
  - `findstr /si password passwd *.xml`
  - `findstr /si password passwd *.ini`
  - `findstr /si password passwd *.dat`
- registry
  - `reg query HKU /f password /t REG_SZ /s`
  - `reg query HKLM /f password /t REG_SZ /s`
  - `reg query HKCU /f password /t REG_SZ /s`
  - `reg query HKU /f passwd /t REG_SZ /s`
  - `reg query HKLM /f passwd /t REG_SZ /s`
  - `reg query HKCU /f passwd /t REG_SZ /s`

## tools

### auditing

### powerup

## references
- [Windows Privilege Escalation: An approach for penetration testing](https://sec-consult.com/blog/detail/windows-privilege-escalation-an-approach-for-penetration-testers/)
